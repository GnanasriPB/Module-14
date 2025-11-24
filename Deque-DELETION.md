# Exp.No:38  
## Deque - DELETION

---

### AIM  
To write a Python program to delete elements at FRONT END of deque using a collection built-in function.

---

### ALGORITHM  

1. Import the `deque` class from the `collections` module.  
2. Create an empty deque.  
3. Define how many elements to input (e.g., 3 inputs as in the example).  
4. Loop through the range of input size:  
   - Read an integer from the user.  
   - Append the integer to the deque.  
5. Remove the front element of the deque using `popleft()`.  
6. Print the final deque after deletion.  

---

### PROGRAM  

```
import collections
  
n1=int(input())
n2=int(input())
n3=int(input())
# initializing deque
de = collections.deque([n1,n2,n3])


de.popleft()


# printing modified deque
print ("The deque after deleting is : ")
print (de)
```

### OUTPUT
<img width="602" height="252" alt="image" src="https://github.com/user-attachments/assets/07b7e645-0200-49ff-a760-f15ac08e969f" />


### RESULT
Thus, a Python program to delete elements at FRONT END of deque using a collection built-in function was implemented successfully.
