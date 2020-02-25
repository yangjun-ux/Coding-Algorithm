> # Find Harshad Number

> ### DO
>
> This code will find Harshad Number
>
> Harshad Number : In mathematics, a harshad number (or Niven number in a given number base is an integer that is divisible by the sum of its digits when written in that base.

> ## Code
>
> ```python
> def solution(x):
>     ls = list(str(x))
>     num2 = 0
>     for num in ls:
>         num1 = int(num)
>         num2 += num1
>         if x % num2 == 0:
>             answer = True
>         else:
>             answer = False
>         
>     return answer
> ```
>
> 

> ### Example
>
> INPUT : 34
>
> 3 + 4 = 7
>
> 34 / 7 = 4 ... 6
>
> **return False**