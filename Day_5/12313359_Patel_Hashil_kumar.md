
- Link - https://neetcode.io/problems/linked-list-cycle-detection/question

```python
class Solution:
    def hasCycle(self, head: Optional[ListNode]) -> bool:
        seen = set()
        x = head
        while x:
            if x in seen:
                return True
            seen.add(x)
            x = x.next
        return False
```