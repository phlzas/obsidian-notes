# Web Security Essentials 🔒

## Security Fundamentals

### 1. OWASP Top 10

- Injection
- Broken Authentication
- Sensitive Data Exposure
- XML External Entities (XXE)
- Broken Access Control
- Security Misconfiguration
- Cross-Site Scripting (XSS)
- Insecure Deserialization
- Using Components with Known Vulnerabilities
- Insufficient Logging & Monitoring

### 2. Security Headers

```typescript
// Example security headers setup
app.use(helmet());
app.use((req, res, next) => {
  res.setHeader("Content-Security-Policy", "default-src 'self'");
  res.setHeader("X-Frame-Options", "DENY");
  res.setHeader("X-Content-Type-Options", "nosniff");
  res.setHeader("Referrer-Policy", "no-referrer");
  next();
});
```

## Implementation Guide

### 1. Authentication

#### JWT Implementation

```typescript
// JWT authentication example
import jwt from "jsonwebtoken";

const generateToken = (user: User): string => {
  return jwt.sign({ id: user.id, email: user.email }, process.env.JWT_SECRET!, {
    expiresIn: "24h",
  });
};

const verifyToken = (token: string) => {
  try {
    return jwt.verify(token, process.env.JWT_SECRET!);
  } catch (error) {
    throw new Error("Invalid token");
  }
};
```

### 2. Authorization

#### Role-Based Access Control

```typescript
const checkRole = (roles: string[]) => {
  return (req: Request, res: Response, next: NextFunction) => {
    if (!req.user) {
      return res.status(401).json({ message: "Unauthorized" });
    }

    if (!roles.includes(req.user.role)) {
      return res.status(403).json({ message: "Forbidden" });
    }

    next();
  };
};
```

## Security Measures

### 1. Input Validation

- Sanitize user input
- Validate data types
- Implement rate limiting
- Use prepared statements

### 2. XSS Prevention

```typescript
// XSS prevention example
import xss from "xss";

app.use((req, res, next) => {
  if (req.body) {
    for (let key in req.body) {
      if (typeof req.body[key] === "string") {
        req.body[key] = xss(req.body[key]);
      }
    }
  }
  next();
});
```

### 3. CSRF Protection

```typescript
import csurf from "csurf";

app.use(csurf());
app.use((req, res, next) => {
  res.locals.csrfToken = req.csrfToken();
  next();
});
```

## Data Protection

### 1. Encryption

```typescript
import crypto from "crypto";

const encrypt = (text: string): string => {
  const cipher = crypto.createCipher(
    "aes-256-cbc",
    process.env.ENCRYPTION_KEY!
  );
  let encrypted = cipher.update(text, "utf8", "hex");
  encrypted += cipher.final("hex");
  return encrypted;
};
```

### 2. Password Hashing

```typescript
import bcrypt from "bcrypt";

const hashPassword = async (password: string): Promise<string> => {
  const salt = await bcrypt.genSalt(10);
  return bcrypt.hash(password, salt);
};
```

## Security Testing

### 1. Penetration Testing

- Automated scanning
- Manual testing
- Vulnerability assessment
- Security audit

### 2. Security Headers Check

```bash
# Example curl command to check security headers
curl -I https://your-api.com
```

## Monitoring & Logging

### 1. Security Logging

```typescript
import winston from "winston";

const securityLogger = winston.createLogger({
  level: "info",
  format: winston.format.json(),
  transports: [new winston.transports.File({ filename: "security.log" })],
});
```

### 2. Intrusion Detection

- Monitor suspicious activities
- Alert on security events
- Track login attempts
- Audit trail

## Best Practices

### 1. General Guidelines

- Keep dependencies updated
- Use security linters
- Implement proper logging
- Regular security audits

### 2. Code Review

- Security-focused reviews
- Dependency checking
- Code analysis tools
- Regular updates

## Progress Tracking

- [ ] Security headers implemented
- [ ] Authentication system secure
- [ ] Input validation complete
- [ ] XSS protection in place
- [ ] CSRF protection active
- [ ] Security logging setup

## Next Steps

→ [[api-design]]
→ [[system-scalability]]
→ [[cloud-native-development]]
