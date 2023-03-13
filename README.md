# Solution: detect-whether-a-linked-list-contains-a-cycle

```java
 static boolean hasCycle(SinglyLinkedListNode head) {
        Set<SinglyLinkedListNode> set = new HashSet<>();
        while(head.next != null){
            if(set.add(head) == false) return true;    
            head = head.next;            
        }
        return false;
    }
```
