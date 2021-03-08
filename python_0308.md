```
list = {3, 100, 23, 44}
for i in list:
  if i % 3 == 0:
    print(i)
```
```
user_input_a = input("정수입력> ")

if user_input_a.isdigit():
  number_input_a = int(user_input_a)
  
  print("원의 반지름 : ", number_input_a)
  print("원의 둘레 : ", 2 * 3.14 * number_input_a)
  print("원의 넓이 : ", 3.14 * number_input_a * number_input_a)
else:
  print("error")
```
```
try :
  user_input_a = input("정수입력> ")
  number_input_a = int(user_input_a)
  
  print("원의 반지름 : ", number_input_a)
  print("원의 둘레 : ", 2 * 3.14 * number_input_a)
  print("원의 넓이 : ", 3.14 * number_input_a * number_input_a)
except:
  print("error")
```
```
list_input_a = ["52", "273", "32", "스파이", "103"]

for i in list_input_a:
  try:
    list_a.append(int(i))
    print(list_a)
  except:
    pass
```
```
list_input_a = ["52", "273", "32", "스파이", "103"]
list_a = []

for i in list_input_a:
  try:
    list_a.append(int(i))
  except:
    pass

print(list_a)
```
