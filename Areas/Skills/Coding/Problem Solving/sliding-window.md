# Sliding Window Mastery

## Pattern Breakdown

| Window Type | Complexity | Ideal For  |
| ----------- | ---------- | ---------- |
| Fixed       | O(n)       | Averaging  |
| Dynamic     | O(2n)      | Substrings |

## Real-World Implementations

➜ [[network-analysis]] packet monitoring
➜ [[genomics]] DNA sequence scanning

## Window Optimization

```mermaid
graph LR
  A[Initialize] --> B[Expand]
  B --> C{Constraint}
  C -->|Yes| D[Process]
  C -->|No| E[Shrink]
```
