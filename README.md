# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: your name:R.surothaamsn   
RegisterNumber: 23008504
'''
def selection_sort(arr):
    n = len(arr)
    for i in range(n):
        min_idx = i
        for j in range(i + 1, n):
            if arr[j] < arr[min_idx]:
                min_idx = j
        arr[i], arr[min_idx]=arr[min_idx],arr[i]
    return arr
    
list_of_nums = eval(input())
sorted_list = selection_sort(list_of_nums)
print(sorted_list)


```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: your name
RegisterNumber: 
'''
def insertion_sort(nums):
    for i in range(1, len(nums)):
        key = nums[i]
        j = i - 1
        while j >= 0 and key < nums[j]:
            nums[j + 1] = nums[j]
            j -= 1 
        nums[j + 1] = key
    return nums
    
list_of_nums = eval(input())
sorted_list = insertion_sort(list_of_nums)
print(sorted_list)




```

## Output:
![Screenshot (92)](https://github.com/surothaaman/Sorting-Algorithm/assets/133313653/4ae458ac-fad4-4602-9432-82b0b8dbc833)
![Screenshot (93)](https://github.com/surothaaman/Sorting-Algorithm/assets/133313653/a1537567-b52d-407c-af23-f974baaae51f)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
