# detect-whether-a-linked-list-contains-a-cycle

## Problem

https://www.hackerrank.com/challenges/detect-whether-a-linked-list-contains-a-cycle/


## Solution

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

## Tests

![image](https://github.com/Icsuran/detect-whether-a-linked-list-contains-a-cycle/blob/main/Test_case.png)
