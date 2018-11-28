<h1>Priority Queue </h1>
<p1> A Priority Queue is a data structure that is like a queue and dequeue from the front, but has the hieghest priority at the front and the least at the back.<br/>
Parents are smalller than children. There are two types of Priority Queues, Max Heap which puts the largest key at the front, and Min Heap which puts the smallest key at the front.</p1>
<h2>Memory</h2>
<h2>Operations</h2>
<UL>
<LI> Enqueue and dequeue are both O(logn) operations. Deletion is done by a operation called "perc up" this is when the Queue sends an item up the tree to maintain order. The node that is the minimum on the right will become next.
<LI>Build - Build is a o(n) operation depending on the height of the Heap.
</UI>
<h2>Use Cases</h2>
<p1> Binary Heap has a much faster insertion speed than a BST, while a BST has a faster search speed.
<h2>Examples</h2>
<p1>
bh.insert()<br/>
bh.find_min()<br/>
bh.del_min()
</p1>
