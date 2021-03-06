<h1>Deque</h1>
<p1>A Deque is very similar to a Queue. The difference is that Deques are open ended, which means that they are neither LIFO, or FIFO. You can add or remove from both the front and rear. Which means it is up to you to come up with consistent addition and deletion operators.</p1>
<h2>Memory</h2>
<img src="deque_image.png">
<h2>Operations</h2>
<UL> 
  <LI>add_rear() is O(n)/add_front() is O(1)
  <LI>remove_rear() is O(n)/ remove_front() is O(1)
  <LI>Both addition and removal Big O complexity depends on wether it is taking place at the front or the rear of the Deque. At the front it is a easy o(1) operation, while it is 0(n) from the rear. This is because it uses the list operators append and insert for adding, and pop for removal. Insert being an O(n) operation, and append being a O(1) operation. 
</UL>
<h2>Use cases</h2>
<p1> A Deque is a useful data structure that is used in programs like Microsoft Word. The undo, and redo buttons are a deque. They can add or remove from both the front and rear, which makes them more adaptable than a Queue. </p1>
<h2>Example</h2>
<p1>deque = Deque()<br/> deque.add_rear() #uses insert() function<br/> deque.add_front() #uses appened() function <br/> deque.remove_rear()
  # uses pop(0) function <br/>deque.remove_front() #uses pop() function

