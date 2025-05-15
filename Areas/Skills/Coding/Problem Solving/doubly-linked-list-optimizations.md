# Doubly Linked List Optimization

## Advantage Matrix
| Feature | Single | Double |
|---------|--------|--------|
| Reverse Traversal | O(n) | O(1) |
| Deletion | O(n) | O(1) |

## Cache Strategies
1. Page-aware memory allocation
2. Bulk node pre-fetching

## Real-World Uses
➜ [[browser-history]] implementation
➜ [[undo-redo-systems]] state management

```mermaid
graph LR
  X((NULL)) --> A[Node A<br>Prev<br>Data: Value<br>Next]
  A <--> B[Node B<br>Prev<br>Data: Value<br>Next] 
  B --> C((NULL))
```