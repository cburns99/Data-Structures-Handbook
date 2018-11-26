<h1> List</h1>
<p1> A List is a data structure that holds a collection of items. Each of these items holds a position relative to the others. In Python the List acts as a dynamic array.<br/>
  There are also structures called Linkedlists. These come in two different types, singly and doubly linked. Linkedlists contain nodes, these nodes have a value, as well as a pointer. Doubly linked lists point both forwards and backwards, while singly only points forward.  </p1>
<h2> Memory </h2>
<h2>Operations</h2>
<h3> List operations </h3>
<p1> Python list acts exactly like a dynamic array. So go check out that page. <br/>
  [array.md](Array)
<h3> Linkedlist operations </h3>
<p1>Access and search are both o(n) operations. This is because in order to traverse through the list we must go element by element until we come to the value we are searching for, or accessing. <br/> Insertion and deletion on the other hand are both o(1) operations. As insertion requires making the node previous to the insertee point to insertee. And make insertee point to previouses next. Deletion is just the opposite of insertion. </p1>
<h2>Use cases</h2>
<p1> Linked lists are very useful data structures and they are very easily changed. Inserting and deleting is a very quick and easy procedure. </p1>
<h2> Example<h2>
  <p1>
class Node:
    def __init__(self,initdata):
    
        self.data = initdata 
        self.next = None 

    def get_data(self): 
        return self.data

    def get_next(self):
        return self.next

    def set_data(self,newdata):
        self.data = newdata

    def set_next(self,newnext):
        self.next = newnext
class List:
    def __init__(self):
        
        self.head = None
        
    def insert(self,item):
        insertee = Node(item)
        insertee.set_next(self.head)
        self.head = insertee

    def search(self,item):
        current = self.head
        found = False
        while current is not None and not found:
            if current.get_data() is item:
                found = True
            else:
                current = current.get_next()
        return found

    def delete(self,item):
        current = self.head
        previous = None
        found = False
        while not found:
            if current.get_data() is item:
                found = True
            else:
                previous = current
                current = current.get_next()
        if previous is None:
            self.head = current.get_next()
        else:
            previous.set_next(current.get_next())
            
