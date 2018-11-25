<h1>Deque</h1>
<p1>A Deque is very similar to a Queue. The difference is that Deques are open ended, which means that they are neither LIFO, or FIFO. You can add or remove from both the front and rear.</p1>
<h2>Memory</h2>
<h2>Operations</h2>
<h2>Use cases</h2>
<h2>Example</h2>
<p1>class Deque:
  
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
