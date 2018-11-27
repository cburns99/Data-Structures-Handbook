<h1>Deque</h1>
<p1>A Deque is very similar to a Queue. The difference is that Deques are open ended, which means that they are neither LIFO, or FIFO. You can add or remove from both the front and rear.</p1>
<h2>Memory</h2>
<h2>Operations</h2>
<p1> Insertion and deletions Big O complexity depends on wether it is taking place at the front or the rear of the Deque. At the front it is a easy o(1) operation, while it is 0(n) from the rear. This is because it uses the list operators append and insert. insert being an O(n) operation, and append being a O(1) operation.</p1> 
<h2>Use cases</h2>
<p1> A Deque is a useful data structure that is used in programs like Microsoft Word. The undo, and redo buttons are a deque. They can add or remove from both the front and rear. </p1>
<h2>Example</h2>
<p1>
  
  class Deque:
    def __init__(self):<br/>
        self.items = []<br/>
    def isEmpty(self):<br/>
        return self.items == []<br/>
    def addFront(self, item):<br/>
        self.items.append(item)<br/>
    def addRear(self, item):<br/>
        self.items.insert(0,item)<br/>
    def removeFront(self):<br/>
        return self.items.pop()<br/>
    def removeRear(self):<br/>
        return self.items.pop(0)</p1>
