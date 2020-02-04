## N numbers spaced by X
Two numbers are entered and the array is printed.

### ex)
- input : [2, 5]
- output : [2, 4, 6, 8, 10]
### or
- input : [n, x]
- output : [n, n*2, n*3, n*4, ... , n*x]

## Code
```
def solution(x, n):
answer = []
for data in range(0, n):
    data_1 = x + x*data
    answer.append(data_1)
return answer
```
