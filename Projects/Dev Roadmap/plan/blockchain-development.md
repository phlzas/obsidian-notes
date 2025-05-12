# Blockchain Development Guide ⛓️

## Core Concepts

### 1. Blockchain Fundamentals

- Distributed Ledger
- Consensus Mechanisms
- Smart Contracts
- Cryptography Basics

### 2. Key Technologies

- Ethereum
- Solidity
- Web3.js/ethers.js
- IPFS

## Smart Contract Development

### 1. Basic Smart Contract

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract SimpleToken {
    string public name;
    string public symbol;
    uint256 public totalSupply;
    mapping(address => uint256) public balanceOf;

    constructor(string memory _name, string memory _symbol, uint256 _totalSupply) {
        name = _name;
        symbol = _symbol;
        totalSupply = _totalSupply;
        balanceOf[msg.sender] = _totalSupply;
    }

    function transfer(address _to, uint256 _value) public returns (bool success) {
        require(balanceOf[msg.sender] >= _value, "Insufficient balance");
        balanceOf[msg.sender] -= _value;
        balanceOf[_to] += _value;
        return true;
    }
}
```

### 2. Web3 Integration

```typescript
import { ethers } from "ethers";

class Web3Service {
  private provider: ethers.providers.Provider;
  private contract: ethers.Contract;

  constructor(contractAddress: string, abi: any) {
    this.provider = new ethers.providers.Web3Provider(window.ethereum);
    this.contract = new ethers.Contract(contractAddress, abi, this.provider);
  }

  async connectWallet(): Promise<string> {
    const accounts = await window.ethereum.request({
      method: "eth_requestAccounts",
    });
    return accounts[0];
  }

  async getBalance(address: string): Promise<string> {
    const balance = await this.contract.balanceOf(address);
    return ethers.utils.formatEther(balance);
  }
}
```

## DApp Architecture

### 1. Frontend Integration

```typescript
// React component example
const WalletConnect: React.FC = () => {
  const [account, setAccount] = useState<string>("");
  const [balance, setBalance] = useState<string>("0");

  const connectWallet = async () => {
    try {
      const web3 = new Web3Service(CONTRACT_ADDRESS, ABI);
      const account = await web3.connectWallet();
      setAccount(account);
      const balance = await web3.getBalance(account);
      setBalance(balance);
    } catch (error) {
      console.error("Wallet connection failed:", error);
    }
  };

  return (
    <div>
      <button onClick={connectWallet}>Connect Wallet</button>
      {account && (
        <div>
          <p>Account: {account}</p>
          <p>Balance: {balance}</p>
        </div>
      )}
    </div>
  );
};
```

## Smart Contract Security

### 1. Common Vulnerabilities

- Reentrancy Attacks
- Integer Overflow/Underflow
- Front-running
- Access Control Issues

### 2. Security Best Practices

```solidity
// Security pattern example
contract SecureContract {
    mapping(address => uint256) private balances;
    mapping(address => bool) private locked;

    modifier nonReentrant() {
        require(!locked[msg.sender], "Reentrant call");
        locked[msg.sender] = true;
        _;
        locked[msg.sender] = false;
    }

    function withdraw() public nonReentrant {
        uint256 amount = balances[msg.sender];
        require(amount > 0, "No balance");
        balances[msg.sender] = 0;
        (bool success, ) = msg.sender.call{value: amount}("");
        require(success, "Transfer failed");
    }
}
```

## Testing Strategy

### 1. Unit Testing

```javascript
const { expect } = require('chai')
const { ethers } = require('hardhat')

describe('SimpleToken', function () {
    let token
    let owner
    let addr1

    beforeEach(async function () {
        const Token = await ethers.getContractFactory('SimpleToken')
        [owner, addr1] = await ethers.getSigners()
        token = await Token.deploy('Test Token', 'TEST', 1000000)
        await token.deployed()
    })

    it('Should transfer tokens between accounts', async function () {
        await token.transfer(addr1.address, 50)
        expect(await token.balanceOf(addr1.address)).to.equal(50)
    })
})
```

## Development Tools

### 1. Essential Tools

- Hardhat/Truffle
- MetaMask
- Remix IDE
- Etherscan

### 2. Testing Networks

- Ganache
- Testnet (Goerli/Sepolia)
- Local Network

## Deployment Process

### 1. Contract Deployment

```javascript
async function main() {
  const Token = await ethers.getContractFactory("SimpleToken");
  const token = await Token.deploy("My Token", "MTK", 1000000);
  await token.deployed();
  console.log("Token deployed to:", token.address);
}

main()
  .then(() => process.exit(0))
  .catch((error) => {
    console.error(error);
    process.exit(1);
  });
```

### 2. Verification

- Contract verification
- Testing on testnet
- Security audit

## Progress Tracking

- [ ] Smart contract basics
- [ ] Web3 integration
- [ ] Security implementation
- [ ] Testing complete
- [ ] Deployment ready

## Learning Resources

- Solidity Documentation
- Ethereum Developer Portal
- OpenZeppelin Guides
- Web3 University

## Next Steps

→ [[cloud-services]]
→ [[web-security]]
→ [[system-scalability]]
