<h1>BST</h1>
<p1> A binary search tree relies on the property that keys that are less than the parent are found in the left subtree, and keys that are greater than the parent are found in the right subtree. Trees have parents, children, and leaves, this goes for other types of trees as well.  </p1>
<h2>Memory</h2>
<img src="bstimage.png">
<h2>Operations</h2>
<UI>
  <LI>Insert, deletion and find are all O(logn) operations. <br/>This is because it checks left where the smaller values are and then checks right. It depends on the size of the tree as well. Traversal is done a few different ways. Post order (checks left, checks right, checks initial node) pre order(checks initial node, checks left, checks right) or in order ( checks left, initial node, and finally the right) Tree insertion inserts smaller values to the left, and larger to the right. Deletion is quite a bit more complex, the node deleted must be replaced by a node that makes sense and keeps the Binary search trees structure. This replacement node is called a successor, and is chosen further along in the Tree.
<LI>Deleting a node with no children: simply remove the node from the tree.
<LI>Deleting a node with one child: remove the node and replace it with its child.
<LI>Deleting a node with two children: call the node to be deleted. Do not delete that node. Choose either its predecessor node or successor. Copy the user values of new node to the node that is being deleted. If the new node does not have a child simply remove it from its previous parent. If it has a child, replace it with the child at new the nodes parent. 
<h2>Use cases</h2>
  <p1>The most common use is to store data that can be accessed and searched quickly and efficiently. They are often used for implementing maps or sets. They are much faster for seearching than Binary Heaps, while Heaps have a faster insertion time.
<h2>Example</h2>
    <p1>
bst.insert(self, insertee)<br/>
bst.delete(self)<br/>
bst.find(self, item)<br/>

</p1>
