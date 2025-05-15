# Database Indexing Strategies

## Index Showdown
| Type | Read Speed | Write Cost | Best For |
|------|------------|------------|----------|
| B-Tree | O(log n) | High | Range queries |
| Hash | O(1) | Low | Exact matches |

## Real-World Impact
➜ [[e-commerce]] product search
➜ [[fintech]] transaction auditing

```mermaid
graph LR
  Data --> Index
  Index -->|Accelerates| Query