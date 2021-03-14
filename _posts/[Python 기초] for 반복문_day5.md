### for 반복문
- 리스트, 문자열 등등 순회 가능한 객체를 순회하면서 값을 처리할 때 사용


```python
# for 반복 변수 in 반복 범위:
#     코드 블록

# for 반복 변수 in a:
#     코드 블록
```

- i는 매번 수행될 때마다 a의 아이템으로 순차적으로 변경
- 모든 아이템이 순회되면 for 블록 종료


```python
list1 = ['a', 'b', 'c', 'd']

num = 0

while True:
    print(list1[num])
    num += 1
    
    if num == 4:
        break
        
```

    a
    b
    c
    d
    


```python
for i in list1:
    print(i)
```

    a
    b
    c
    d
    


```python
tuple1 = (1, 2, 3, 4)

for t in tuple1:
    print(t)
```

    1
    2
    3
    4
    


```python
str1 = "efgh"

for s in str1:
    print(s)
```

    e
    f
    g
    h
    


```python
hi = "안녕하세요"
for s in hi:
    print(s)
```

    안
    녕
    하
    세
    요
    


```python
tuple_food = ("햄버거", "치킨", "피자")
for food in tuple_food:
    print(food)
```

    햄버거
    치킨
    피자
    


```python
score_list = [90, 45, 70, 60, 55]
num = 0

for s in score_list:
    num += 1
    if s >= 60:
        print("{}번 학생은 합격 입니다.".format(num))
    else:
        print("{}번 학생은 불합격 입니다.".format(num))    
```

    1번 학생은 합격 입니다.
    2번 학생은 불합격 입니다.
    3번 학생은 합격 입니다.
    4번 학생은 합격 입니다.
    5번 학생은 불합격 입니다.
    


```python
score_list = [90, 45, 70, 60, 55]
num = 0

for s in range(len(score_list)):
    num += 1
    if score_list[s] >= 60:
        print("{}번 학생은 합격 입니다.".format(num))
    else:
        print("{}번 학생은 불합격 입니다.".format(num))    
```

    1번 학생은 합격 입니다.
    2번 학생은 불합격 입니다.
    3번 학생은 합격 입니다.
    4번 학생은 합격 입니다.
    5번 학생은 불합격 입니다.
    


```python
import math
score_list = [90, 45, 70, 60, 55]

sum(score_list)
```




    320




```python
score_list = [90, 45, 70, 60, 55]
num = 0

for i in score_list:
    num += 1
    if i >= 60:
        print("{}번 학생은 합격입니다.".format(num))
    else:
        print("{}번 학생은 불합격입니다.".format(num))
```

    1번 학생은 합격입니다.
    2번 학생은 불합격입니다.
    3번 학생은 합격입니다.
    4번 학생은 합격입니다.
    5번 학생은 불합격입니다.
    

### range() 함수
- range(시작할 숫자, 종료할 숫자, 증가량)


```python
for i in range(1, 10):
    print(i, end = " ")
```

    1 2 3 4 5 6 7 8 9 


```python
for i in range(1, 10):
    print("a", end = " ")
```

    a a a a a a a a a 


```python
for i in range(97, 76, -1):
    print(i, end = " ")
```

    97 96 95 94 93 92 91 90 89 88 87 86 85 84 83 82 81 80 79 78 77 


```python
for i in range(23, 41):
    print(i, end = " ")
```

    23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 


```python
start = int(input("첫 번째 정수 입력 >>"))
end = int(input("두 번째 정수 입력 >>"))

for i in range(start, end+1):
    print(i, end = " ")
```

    첫 번째 정수 입력 >>10
    두 번째 정수 입력 >>30
    10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 


```python
total = 0

for i in range(3, 101, 3):
    total += i

print(total)
```

    1683
    


```python
sum = 0

for e in range(1,100):
    if e%3 == 0:
        sum += e
        
print(sum)        
```

    1683
    


```python
for b in range(1, 10):
    for a in range(2, 7):
        print("{} * {} = {}".format(a, b, a*b), end = "\t")
    print()
```

    2 * 1 = 2	3 * 1 = 3	4 * 1 = 4	5 * 1 = 5	6 * 1 = 6	
    2 * 2 = 4	3 * 2 = 6	4 * 2 = 8	5 * 2 = 10	6 * 2 = 12	
    2 * 3 = 6	3 * 3 = 9	4 * 3 = 12	5 * 3 = 15	6 * 3 = 18	
    2 * 4 = 8	3 * 4 = 12	4 * 4 = 16	5 * 4 = 20	6 * 4 = 24	
    2 * 5 = 10	3 * 5 = 15	4 * 5 = 20	5 * 5 = 25	6 * 5 = 30	
    2 * 6 = 12	3 * 6 = 18	4 * 6 = 24	5 * 6 = 30	6 * 6 = 36	
    2 * 7 = 14	3 * 7 = 21	4 * 7 = 28	5 * 7 = 35	6 * 7 = 42	
    2 * 8 = 16	3 * 8 = 24	4 * 8 = 32	5 * 8 = 40	6 * 8 = 48	
    2 * 9 = 18	3 * 9 = 27	4 * 9 = 36	5 * 9 = 45	6 * 9 = 54	
    
