```
def find_ins_idx(r,v):
  for i in range(0, len(r)):
    if v < r[i]:
      return i
  return len(r)

def ins_sort(a):
  result = []
  while a:
    value = a.pop(0)
    ins_idx = find_ins_idx(result, value)
    result.insert(ins_idx, value)
  return result

d = [2, 4, 5, 1, 3]
print(ins_sort(d))
```
```
def ins_sort(a): # d를 a에 넣고
  n = len(a) # a의 길이값을 n에 넣는다
  for i in range(1, n): # i는 처음에 1이고 n만큼, 즉 a의 길이값만큼 돈다
    key = a[i] # a[1]부터 key에 넣는다 그리고 a[2], a[3]... 점점 올라간다
    j = i - 1 # j에다가 i-1의 값을 넣는다
    while j >= 0 and a[j] > key: # (j가 0보다 크거나 작을때,) 그리고 a[j] 한마디로 key 보다 하나 전 배열값이 key보다 클때까지 실행
      a[j+1] = a[j] # a[j+1]값에 a[j]값을 넣어준다
      j -= 1 # j에 j = j - 1을 해준다 = 한단계 낮춰준다
    a[j+1] = key # a[j+1]값에 key값을 넣어준다

d = [2, 4, 5, 1, 3]
ins_sort(d)
print(d)
```
```
def merge_sort(a):
  n = len(a)
  
  if n <= 1:
    return a

  mid = n // 2
  g1 = merge_sort(a[:mid])
  g2 = merge_sort(a[mid:])
  
  result = []
  while g1 and g2:
    if g1[0] < g2[0]:
      result.append(g1.pop(0))
    else:
      result.append(g2.pop(0))
  while g1:
    result.append(g1.pop(0))
  while g2:
    result.append(g2.pop(0))
  return result

d = [6, 8, 3, 9, 10, 1, 2, 4, 7, 5]
print(merge_sort(d))
```
