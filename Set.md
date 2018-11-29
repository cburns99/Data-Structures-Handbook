<h1> Set </h1>
<p1>A set is an unordered data structure that is immutable. Sets do not allow duplicates and are heterogeneous. It is a built in data structure for Python, its syntax is as follows "mySet = {}"</p1>
<h2> Memory </h2>
<img src="setimage.png">
<h2>Operations</h2>
<UL>
  
<LI>  Add - Adds items to the set.  O(1) constant time as it is the same as an array.
<LI> Remove - Removes item from a set. O(1) constant time as it is the same as an array.
<LI> in - checks to see if element is in the Set. This is an O(n) operation as sets have different types of data types, so it must check every element.
  </UL>
<h2>Use Cases </h2>
Sets are good for storing values when you can not have duplicates. Although arrays are better for a bunch of elements when there are duplicates.
<h2>Example</h2>
mySet = {1, 'dog', 60}</br>
'dog' in mySet</br>
mySet.add(4)</br>
mySet.remove('dog')</br>
print(mySet)<br/>
output ---><br/> 
True<br/>
{1,60,4}
