class MyClass:
    def func(self,n):
        self.n=n
        if self.n==1:
            return True
        else:
            return self.n*MyClass.func(self,self.n-1)

unittest.....
import unittest
import test1

obj=test1.MyClass()

class test(unittest.TestCase):
    def test_factTest(self):
        
        obj=test1.MyClass()
        result= obj.func(6)
        self.assertTrue(result,720)

    def test_factTest2(self):
        
        obj=test1.MyClass()
        result = obj.func(4)
        self.assertFalse(result,0)

if __name__ == '__main__':
    unittest.main()


stack.....

class stack:

    def __init__(self):
       self.items = []

# Stack is empty when stack size is 0
    def isEmpty(self,stack):
        print "Stack is empty"
        return self.items == []

# Function to add an item to stack. It increases size by 1
    def push(self, item):
        self.items.append(item)
        print("pushed to stack " + item)

# Function to remove an item from stack. It decreases size by 1
    def pop(self):
        if (isEmpty(self)):
            print "Stack underflow"
            
        else:
            return str(-maxsize -1) #return minus infinite

        return stack.pop()

    def display(self):
        return self.items[len(self.items) - 1]

# Driver program to test above functions
s = stack()
s.push('1')
s.push('1')
print (s.display())
print (s.pop())
print (s.display())


