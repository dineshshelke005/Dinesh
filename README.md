1.Implement a stack using a list in Python. Include the necessary methods such as push, pop, and isEmpty.

class Stack:
    def __init__(self):
        self.stack = []

    def push(self, item):
        self.stack.append(item)

    def pop(self):
        if not self.isEmpty():
            return self.stack.pop()
        else:
            raise IndexError("Stack is empty. Cannot pop from an empty stack.")

    def isEmpty(self):
        return len(self.stack) == 0


2. Implement a queue using a list in Python. Include the necessary methods such as enqueue, dequeue, and isEmpty.

class Queue:
    def __init__(self):
        self.queue = []

    def enqueue(self, item):
        self.queue.append(item)

    def dequeue(self):
        if not self.isEmpty():
            return self.queue.pop(0)
        else:
            raise IndexError("Queue is empty. Cannot dequeue from an empty queue.")

    def isEmpty(self):
        return len(self.queue) == 0

