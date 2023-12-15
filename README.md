# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
Program for linear search method to match the item in a list
Developed by:Piritharaman R
RegisterNumber:23013537
```
def linearSearch(array,n,k):
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1
array = eval(input())
k = eval(input())
n=len(array)
array.sort()
print(array)
result=linearSearch(array,n,k)
if result != -1:
    print(f"Element found at index:  {result}")
else:
    print(f"Element not found ")
```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by:Piritharaman R
RegisterNumber: 23013537
'''
def binarysearchIter(array, k, low, high):
   while low<=high:
       mid=(low+high)//2
       if array[mid]==k:
           return mid
       elif array[mid]<k:
           low=mid+1
       else:
           high=mid-1
   return -1
       
    
array = eval(input())
array.sort()
k = eval(input())
result=binarysearchIter(array,k,0,len(array)-1)
print(array)
if result!=-1:
    print(f"Element found at index:  {result}")
else:
    print(f"Element not found")
```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
Program to find the element in a list using Binary Search (recursive Method).
Developed by:Piritharaman R
RegisterNumber: 23013537
'''
def binarysearch(array, k, low, high):
    while low<=high:
        mid=(low+high)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
    
array=eval(input())
array.sort()
k = eval(input())
result=binarysearch(array,k,0,len(array)-1)
print(array)
if result!=-1:
    print(f"Element found at index:  {result}")
else:
    print(f"Element not found")
```
## Sample Input and Output
![image](https://github.com/ramanpiritha/Search-Algorithm/assets/147084116/d806ef60-cc47-48c7-98f8-3bbad2428764)

##Output
![image](https://github.com/ramanpiritha/Search-Algorithm/assets/147084116/cc8fb4e4-b122-4e2d-8f7b-7969ed627f01).
![image](https://github.com/ramanpiritha/Search-Algorithm/assets/147084116/c440b981-41ae-405e-99d2-f14ceb5a6c41).
![image](https://github.com/ramanpiritha/Search-Algorithm/assets/147084116/758b6e10-ac68-4406-bd95-8697fd84f610).










## Result
Thus the linear search and binary search algorithm is implemented using python programming.
