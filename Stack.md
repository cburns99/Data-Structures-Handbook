<h1>Stack</h1>
<p1>A Stack is an ordered data structure of elements that are all inserted on top of each other just like a stack of cards. This makes it LIFO(last in, first out).  </p1>
<h2>Memory</h2>
<h2>Operations</h2>

* **insert**: "push"
  * this is a O(1) operation.This is because it is a simple operation to just simpily add an element to the top of the stack.

* **remove**: "pop"
  * O(1), constant time. This operation is constant thanks to the stack pointer being based at the top of the stack. The only work the pop operation must do is simply return the value stored at the stack pointer. We don't need to peek inside to return it, which is why it isn't O(n).

* **access**: "peek"
  * This is a O(n) operation. It simply returns the top item from the stack but does not remove it.
<h2>Use cases</h2>
<p1> Stacks are used to backtrack to see history in programs. A web browser history is a good example of a stack in use.
<h2>Example</h2>
  <p1>
  class Stack:
     
     def __init__(self):
         self.items = []

     def isEmpty(self):
         return self.items == []

     def push(self, item):
         self.items.append(item)

     def pop(self):
         return self.items.pop()

     def peek(self):
         return self.items[len(self.items)-1]

     def size(self):
         return len(self.items)
</p1>
