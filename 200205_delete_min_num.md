# Delete Minimum number

### DO
1. input array (ex: [3, 4, 5, 6, 7)
2. This code delete array's minimum number
3. Output (ex: [4, 5, 6, 7])

```
def solution(arr):
if len(arr) == 1:
    arr = [-1]
else:
    arr_1 = arr.copy()
    arr_1.sort()
    arr.remove(arr_1[0])
answer = arr
return answer
```

### Example
- input : [4, 9, 8, 7, 15, 20]
- output : [9, 8, 7, 15, 20]
