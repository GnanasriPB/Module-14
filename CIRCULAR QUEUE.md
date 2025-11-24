# Exp No: 36  
## Circular Queue 
---

### AIM  
To write a Python program with a function to insert float values into a Circular Queue.

---

### ALGORITHM

1. Start  
2. Check if the Circular Queue is full  
   - If `size == max_size`, print `"Queue is full"` and exit the function  
3. If the queue is not full:  
   - Read the element to be inserted  
   - Convert it to float  
   - Insert the element at the `tail` position  
   - Update tail using: `tail = (tail + 1) % max_size` (circular increment)  
   - Increment `size` by 1  
4. End

---

### PROGRAM

```
# Queue simply works in FIFO
class Queue:
    def __init__(self, size):
        self.items = [0] * size
        self.max_size = size
        self.head, self.tail, self.size = 0, 0, 0

    def enqueue(self, item):
        if self.is_list_full():
            print(f'Queue is full')
            return
        self.items[self.tail] = item
        self.tail = (self.tail + 1) % self.max_size
        self.size += 1
    def dequeue(self):
        item = self.items[self.head]
        self.head = (self.head + 1) % self.max_size
        self.size -= 1

        return item
   

    def is_list_full(self):
        if self.size == self.max_size:
            return True
        return False

    def is_empty(self):
        if self.size == 0:
            return True
        return False

size=int(input())
queue = Queue(size)
fl=float(input())
fl1=float(input())
fl2=float(input())
queue.enqueue(fl)
queue.enqueue(fl1)
queue.enqueue(fl2)

    
print(queue.items)



```

### OUTPUT

<img width="451" height="283" alt="image" src="https://github.com/user-attachments/assets/b538142a-4f64-4f76-b8b5-cf5d7271e2d8" />

### RESULT
Thus, a Python program with a function to insert float values into a Circular Queue was implemented successfully.
