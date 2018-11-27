<h1>Queue</h1>
<p1> A Queue is an ordered data structure that contains elements that come in from one end and go out the other. This makes it FIFO (First in first out).</p>
<h2> Memory</h2>
<h2>Operations</h2>
<UL>
   <LI>Access and search are both o(n) operations. As we must continue to send items throught the queue until we are able to access it. Just like a register at the supermarket must check out everyone in front of you before they help you. 
   <LI>Using a list, queues implement operators like "pop" and "insert"
   <LI>Dequeue is a O(1) operation. This is becuase we can simply "dequeue" an element from the end of the queue with one operation.
   <LI>Equeue is a O(n) operation. This is because it must go through the queue before it is at the front of the queue.
</UL>
<h2>Use Cases</h2>
A good use case example is printing queues. Say you and 5 other people have all wanted to print something at around the same time. The program that figures out who clicked "print" first, second, thrid and so on is a queue. Queues are great for quickly dequeueing off elements, but not as good as say stacks for enqueueing elements.
<h2>Examples</h2>
<p1> 
is_empty(self):
enqueue(self, item) # uses insert()<br/>
dequeue(self) # usues pop()<br/>
 </p1>                              
