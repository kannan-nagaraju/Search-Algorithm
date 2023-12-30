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
Developed by:Kannan N
RegisterNumber:23013389 

def linearsearch(array,n,k):
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1        
array = eval(input())
k=int(input())
n=len(array)
array.sort()
result=linearsearch(array,n,k)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
```


ii)	# Find the element in a list using Binary Search(Iterative Method).
```
Developed By:N.Kannan
Reference No:23013389

def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array=eval(input())
array.sort()
k=eval(input())
result=binarySearchIter(array,k,0,len(array)-1)
if (result == -1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
```

iii)	# Find the element in a list using Binary Search (recursive Method).
```
def BinarySearch(arr, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array=eval(input())
array.sort()
k=eval(input())
result=BinarySearch(array,k,0,len(array)-1)
if (result == -1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)

```

## Sample input:
![image](https://github.com/kannan-nagaraju/Search-Algorithm/assets/145742755/a26e4313-d438-435c-8a3b-750c4e33c5f0)
![image](https://github.com/kannan-nagaraju/Search-Algorithm/assets/145742755/742750fc-2288-438d-ae65-f2b11aec0977)
![image](https://github.com/kannan-nagaraju/Search-Algorithm/assets/145742755/b8da0ded-8fdc-43a9-882f-882698943c1d)




## Output:
![image](https://github.com/kannan-nagaraju/Search-Algorithm/assets/145742755/8e303c9e-25e6-4739-854a-3ba26a4a842f)
![image](https://github.com/kannan-nagaraju/Search-Algorithm/assets/145742755/b9135e8c-2777-4193-a0cf-6e4760bd5f95)
![image](https://github.com/kannan-nagaraju/Search-Algorithm/assets/145742755/2102a286-e3f3-4445-8a3f-5c3633665bb4)






## Result
Thus the linear search and binary search algorithm is implemented using python programming.
