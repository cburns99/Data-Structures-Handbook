<h1>Queue</h1>
<p1> A Queue is an ordered data structure that contains elements that come in from one end and go out the other. This makes it FIFO (First in first out).</p>
<h2> Memory</h2>
<h2>Operations</h2>
<p1> Access and search are both o(n) operations. As we must continue to send items throught the queue until we are able to access it. Just like a register at the supermarket must check out everyone in front of you before they help you. <br/> Insertion and deletion on the other hand are both O(1). This is becuase we can simply "enqueue" or "dequeue" elements from the queue with one operation. Using a list, queues implement operators like "pop" and "insert"</p1>
<h2>Use Cases</h2>
A good use case example is printing queues. Say you and 5 other people have all wanted to print something at around the same time. The program that figures out who clicked "print" first, second, thrid and so on is a queue.
<h2>Examples</h2>
<p1> class Queue:
      def __init__(self):
        self.items = []
      def is_empty(self):
        return self.items == []
      def enqueue(self, item)
        self.items.insert(0,item)
      def dequeue(self):
        return self.items.pop()
