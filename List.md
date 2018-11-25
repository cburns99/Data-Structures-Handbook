<h1> List</h1>
<p1> A List is a data structure that holds a collection of items. Each of these items holds a position relative to the others. There are singly and doubly linked lists. Doubly liked lists point both forwards and backwards, while singly only points forward.  </p1>
<h2> Memory </h2>
<h2>Operations</h2>
<p1>Access and search are both o(n) operations. This is because in order to traverse through the list we must go element by element until we come to the value we are searching for, or accessing. <br/> Insertion and deletion on the other hand are both o(1) operations. As insertion requires making the node previous to the insertee point to insertee. And make insertee point to previouses next. Deletion is just the opposite of insertion. </p1>
<h2>Use cases</h2>
<p1> Linked lists are very useful data structures and they are very easily changed. Inserting and deleting is a very quick and easy procedure. </p1>
<h2> Example<h2>
  <p1>
class Node:<br/>
    def __init__(self,initdata):<br/>
    
        self.data = initdata <br/>
        self.next = None <br/>

    def getData(self): <br/>
        return self.data<br/>

    def getNext(self):<br/>
        return self.next<br/>

    def setData(self,newdata):<br/>
        self.data = newdata<br/>

    def setNext(self,newnext):<br/>
        self.next = newnext<br/>
class List:
    def __init__(self):
        self.head = None
        
    def add(self,item):
        temp = Node(item)
        temp.setNext(self.head)
        self.head = temp

    def search(self,item):
        current = self.head
        found = False
        while current != None and not found:
            if current.getData() == item:
                found = True
            else:
                current = current.getNext()
        return found

    def remove(self,item):
        current = self.head
        previous = None
        found = False
        while not found:
            if current.getData() == item:
                found = True
            else:
                previous = current
                current = current.getNext()
        if previous == None:
            self.head = current.getNext()
        else:
            previous.setNext(current.getNext())
            </p1>
