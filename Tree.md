<h1>BST</h1>
<p1> A binary search tree relies on the property that keys that are less than the parent are found in the left subtree, and keys that are greater than the parent are found in the right subtree. </p1>
<h2>Memory</h2>
<h2>Operations</h2>
<p1>Insert, deletion an access are all O(logn) operations. This is because it checks left where the smaller values are and then checks right. It depends on the size of the tree as well. Traversal is done a few different ways. Post order (checks left, checks right, checks initial node) pre order(checks initial node, checks left, checks right) or in order ( checks left, initial node, and finally the right) Tree insertion inserts smaller values to the left, and larger to the right. Deletion is quite a bit more complex, the node deleted must be replaced by a node that makes sense and keeps the Binary search trees structure. Trees have parents, children, and leaves, this goes for other types of trees as well. 
<h2>Use cases</h2>
  <p1>The most common use is to store data that can be accessed and searched quickly, and efficiently.
<h2>Example</h2>
    <p1>
class BinarySearchTree:
	def __init__(self, value = None):
		self.value = value
		self.left = None
		self.right = None

	def insert(self, insertee):
   		if self.value is None: 
   			self.value = insertee 
 
   		elif insertee < self.value:
   			if self.left is None:
   				self.left = BinarySearchTree(insertee)
   			else:
   				self.left.insert(insertee)
   		else:
   			if self.right is None:
   				self.right = BinarySearchTree(insertee)
   			else: 
   				self.right.insert(insertee)
   	
	def find(self, item):  
		if self.value is None:
			return None
		elif self.value is item: 
			return self.value
		elif self.value > item: 
			return self.right.find(item)
		elif self.value < value:
			return self.left.find(item)

	def post_order(self):
		post_order_list = []
		if self.left:
			post_order_list.extend(self.left.post_order())
		if self.right:
			post_order_list.extend(self.right.post_order())
		post_order_list.append(self.value)
		return post_order_list

	def in_order(self):
		in_order_list = []
		if self.left:
			in_order_list.extend(self.left.in_order())
		if self.right:
			in_order_list.extend(self.right.in_order())
		in_order_list.append(self.value)
		return in_order_list

	def pre_order(self):
		pre_order_list = [self.value]
		if self.left:
			pre_order_list.extend(self.left.pre_order())
		if self.right:
			pre_order_list.extend(self.right.pre_order())
		return pre_order_list
</p1>
