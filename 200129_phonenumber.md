1. input phonenumber
2. This code changes number to "*" except last 4 numbers
3. return change numbers

`
def solution(phone_number):
    data = str(phone_number)
    answer = data_1.replace(data[:-4], "*"*(len(data)-4))
    return answer
`
input / output example
input: 01022776533
output: *******6533
