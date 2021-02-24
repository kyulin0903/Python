# repl.it
```
import math

def abs_sign(a): #절대값 함수
  if a>=0:
    return a
  else:
    return -a

def abs_square(a): #제곱근 함수
  b = a * a
  return math.sqrt(b)

#print(abs_sign(4))
#print(abs_square(4))

def sum_n(n):
  s = 0
  for i in range(1, n+1):
    s = s + i
  return s
#print(sum_n(5))

def sum_nn(n):
  return n*(n+1)//2 
print(sum_nn(5))
```

```
a = [1, 2, 3, 4, 5]
print(len(a))
print("="*20)

a.append(6)
print(a)
print("="*20)

a.append(10)
print("="*20)
print(a)

a.insert(3, 50)
print("="*20)
print(a)

a.pop(3)
print("="*20)
print(a)

a.pop()
print("="*20)
print(a)

a.clear()
print("="*20)
print(a)
```

```
def find_max(a):
  n = len(a)
  max_v = a[0]
  for i in range(1, n):
    if(a[i] > max_v):
      max_v = a[i]
  return max_v

v = [17, 92, 18, 33, 58, 7, 33, 42]
print(find_max(v))
```

```
def find_max(a):
  n = len(a)
  max_v = a[0]
  max_p = 0
  for i in range(1, n):
    if(a[i] > max_v):
      max_v = a[i]
      max_p = i
  return max_p

v = [17, 92, 18, 33, 58, 7, 33, 42]
print(find_max(v))
```

```
def find_max_idx(a):
  n = len(a)
  max_idx = 0
  for i in range(1, n):
    if(a[i] > a[max_idx]):
      max_idx = i
  return max_idx

v = [17, 92, 18, 33, 58, 7, 33, 42]
print(find_max_idx(v))
```

len(a) : 리스트 길이(자료 개수)를 구함

append(x) : 자료 x를 리스트의 맨 뒤에 추가

insert(i,x) : 리스트의 i번 위치에 x를 추가

pop(i) : i번 위치에 있는 자료를 리스트에서 제거
단, 지정하지 않으면 마지막값 추출

clear() : 리스트의 모든 자료를 지움, 초기화

x in a : 어떤 자료 x가 리스트 a 안에 있는지 확인
반대결과 (x not in a)
