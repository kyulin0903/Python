# repl.it
```
array = [273, 32, 103, 57, 52]

for i in range(len(array)):
  print("{}번째 반복 : {}".format(i, array[i]))

for i in range(5):
  print(str(i) + "반복 변수") #i를 str형태로 강제적 형변환해서 출력
print()

for i in range(4, 0-1, -1):
  print("현재 반복 변수 : {}".format(i))
```

```
import time

number = 0

target_tick = time.time() + 5
while time.time() < target_tick:
  number += 1

print("5초동안 {}번 반복했습니다.".format(number))
```

```
numbers = [103, 52, 273, 32, 77]

print(max(numbers))
print(min(numbers))
print(sum(numbers))
numbers_reversed = reversed(numbers)

#print(numbers_reversed) 출력이 안됨
print(list(numbers_reversed)) # =강제적 형변환
```

```
temp = reversed([1, 2, 3, 4, 5, 6])

for i in temp:
  print("첫번째 반복문 : {}".format(i))

for i in temp:
  print("두번째 반복문 : {}".format(i)) #한번만 쓰이기 때문에 두번째 반복문은 작동하지 않는다
```

```#위의 for문을 아래처럼 바꾸면 두번째 반복문도 작동한다
numbers = [1, 2, 3, 4, 5, 6]

for i in numbers:
  print("첫번째 반복문 : {}".format(i))

for i in numbers:
  print("두번째 반복문 : {}".format(i))
  ```
  
  ```
def search_list(a, x):
  for i in range(len(a)): #값 찾는 함수
    if x == a[i]:
      return i
  return -1

v = [17, 92, 18, 33, 58, 7, 33, 42]

print(search_list(v, 18)) #search_list(이름, 값) return Index = -1
```

``` #선택정렬
def search_list(a, x):
  for i in range(len(a)):
    if x == a[i]:
      return i
  return -1

v = [17, 92, 18, 33, 58, 7, 33, 42]

print(search_list(v, 18))

def find_min_idx(a):
  n = len(a)
  min_idx = 0
  for i in range(1, n):
    if a[i] < a[min_idx]:
      min_idx = i
    return min_idx

def sel_sort(a):
  result = []
  while a:
    min_idx = find_min_idx(a)
    value = a.pop(min_idx) #pop : 값을 뽑아내는 것
    result.append(value) #append : 뒤에 추가하는 것
  return result
d = [2, 4, 5, 1, 3]
print(sel_sort(d))
```
