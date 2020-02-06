# An incomplete Player

### DO

1. input player's name, complete player's name
- ex) [Jane, John, Jun, Emily], [Jane, John, Jun]
2. This code find incomplete player

```
def solution(participant, completion):
for idx in range(len(participant)):
    if completion.count(participant[idx]) != participant.count(participant[idx]):
        return participant[idx]
    else:
        continue
```


