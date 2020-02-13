# abacadaba Student Grading

This code will grade 3 abacadaba students.
and find first grade
# Code!
ls_1 = student 1's pattern
ls_2 = student 2's pattern
ls_3 = student 3's pattern

```
def solution(answers):
    answer = []
    ls_1 = [1, 2, 3, 4, 5]
    ls_2 = [2, 1, 2, 3, 2, 4, 2, 5]
    ls_3 = [3, 3, 1, 1, 2, 2, 4, 4, 5, 5]
    num1 = 0
    num2 = 0
    num3 = 0
    for x in range(len(answers)):
        a = x % 5
        b = x % 8
        c = x % 10
        if ls_1[a] == answers[x]:
            num1 += 1
        if ls_2[b] == answers[x]:
            num2 += 1
        if ls_3[c] == answers[x]:
            num3 += 1
            
    if num1 - num2 > 0 and num1 - num3 > 0:
        answer = [1]
    elif num2 - num1 > 0 and num2 - num3 > 0:
        answer = [2]
    elif num3 - num1 > 0 and num3 - num2 > 0:
        answer = [3]
    elif num1 == num2 == num3:
        answer = [1, 2, 3]
    elif num1 == num2:
        answer = [1, 2]
    elif num1 == num3:
        answer = [1, 3]
    elif num2 == num3:
        answer = [2, 3]

    return answer
```
# Example
- answers = [1, 2, 3, 4, 5] : return : [1]
- answers = [1, 3, 2, 4, 2] : return : [1, 2, 3]
        - if same grade : Ascending
