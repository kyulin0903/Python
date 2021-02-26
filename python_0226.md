# repl.it

#### 집합

add(x) : 집합에 자료 x를 추가
discard(x) : 집합에 자료 x가 들어있다면 삭제
clear() : 집합의 모든 자료를 지움

x in s : 어떤 자료 x가 집합 s에 들어있는지 확인
x not in s : 반대

```
def find_same_name(a): # 동명이인 찾는 함수
  n = len(a)
  result = set()
  for i in range(0, n-1):
    for j in range(i+1, n):
      if a[i] == a[j]:
        result.add(a[i])
  return result
  
name = ["Tom", "Jenny", "Mike", "Tom"]

name2 = ["Tom", "Jenny", "Mike", "Tom", "Mike"]

print(find_same_name(name))
print(find_same_name(name2))
```

```
def fact(n): # 팩토리얼
  f = 1
  for i in range(1, n+1):
    f = f * i
  return f

print (fact(5))
```

```
def fact(n): # 팩토리얼 재귀함수
  if n <= 1:
    return 1
  return n * fact(n-1)

print(fact(3))
```
