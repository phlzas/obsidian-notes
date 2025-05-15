# Cycle Detection Mastery

## Method Comparison
| Technique | Time | Space | Use Case |
|-----------|------|-------|----------|
| Floyd's | O(n) | O(1) | Linked Lists |
| Visited Set | O(n) | O(n) | Graphs |

## Real-World Applications
➜ [[blockchain-analysis]] transaction loops
➜ [[compiler-design]] infinite recursion detection

## Detection Workflow
```mermaid
graph LR
  Start --> CheckNodes
  CheckNodes -->|Duplicate| FoundCycle
  CheckNodes -->|Unique| Continue
  Continue --> CheckNodes
```
## Core Patterns

### [[floyds-tortoise-hare]]
| Metric | Performance |
|--------|-------------|
| Space | O(1) |
| Detection Speed | 2.1x vs Hash |

### [[union-find-pattern]]
```mermaid
graph TB
  A[Init] --> B[Find]
  B --> C[Union]
  C --> D[Path Compression]
```