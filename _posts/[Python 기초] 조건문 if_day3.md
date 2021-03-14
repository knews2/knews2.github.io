### 조건문

- if 문


```python
if True:
    print("실행문장 실행")
```

    실행문장 실행
    


```python
if False:
    print("실행문장 실행")
```


```python
if True:
    print("실행문장 실행")
print("if문 밖에 있는 실행문장")      
```

    실행문장 실행
    if문 밖에 있는 실행문장
    


```python
if False:
    print("실행문장 실행")
print("if문 밖에 있는 실행문장")      
```

    if문 밖에 있는 실행문장
    


```python
money = 11000
if money>10000:
    print("택시를 탄다.")
```

    택시를 탄다.
    


```python
money = 9000 
if money<10000:
    print("버스를 탄다.")
```

    버스를 탄다.
    


```python
money = 11000
if money>= 10000:
    print("택시를 탄다.")
```

    택시를 탄다.
    


```python
money = 9000

if money >= 10000:
    print("택시를 탄다.")
else:
    print("버스를 탄다.")
```

    버스를 탄다.
    


```python
num = int(input("정수 입력 >> "))
if num % 3 == 0 and num % 5 == 0:
    print("3과 5의 배수입니다.")
else:
    print("3과 5의 배수가 아닙니다.")
```

    정수 입력 >> 30
    3과 5의 배수입니다.
    


```python
num1 = int(input("첫 번째 정수 입력 >> "))
num2 = int(input("두 번째 정수 입력 >> "))
if num1 > num2:
    print("첫 번째 정수가 더 큽니다.")
elif num1 < num2:
    print("두 번째 정수가 더 큽니다.")
else:
    print("두 수가 똑같습니다.")
```

    첫 번째 정수 입력 >> 5
    두 번째 정수 입력 >> 3
    첫 번째 정수가 더 큽니다.
    


```python
num1 = int(input("첫 번째 정수 입력 >> "))
num2 = int(input("두 번째 정수 입력 >> "))
if num1 > num2:
    print("첫 번째 정수가 더 큽니다.")
elif num1 < num2:
    print("두 번째 정수가 더 큽니다.")
else:
    print("두 수가 똑같습니다.")
```

    첫 번째 정수 입력 >> 7
    두 번째 정수 입력 >> 13
    두 번째 정수가 더 큽니다.
    


```python
num1 = int(input("첫 번째 정수 입력 >> "))
num2 = int(input("두 번째 정수 입력 >> "))

if num1 > num2:
    print("첫 번째 정수가 더 큽니다.")
elif num1 < num2:
    print("두 번째 정수가 더 큽니다.")
else:
    print("두 수가 똑같습니다.")
```

    첫 번째 정수 입력 >> 7
    두 번째 정수 입력 >> 7
    두 수가 똑같습니다.
    


```python
score = int(input("점수 입력 >> "))
if 90 <= score <= 100:
    r = "A"
elif 80 < score <= 90:
    r = "B"
elif 70 < score <= 80:
    r = "C"
elif 60 < score <= 70:
    r = "D"
elif score < 60:
    r = "F"

print("{}점은 {}학점 입니다.".format(score, r)) 
    
```

    점수 입력 >> 98
    98점은 A학점 입니다.
    


```python
score = int(input("점수 입력 >> "))
if 90 <= score <= 100:
    r = "A"
elif 80 < score <= 90:
    r = "B"
elif 70 < score <= 80:
    r = "C"
elif 60 < score <= 70:
    r = "D"
elif score < 60:
    r = "F"

print("{}점은 {}학점 입니다.".format(score, r)) 
```

    점수 입력 >> 70
    70점은 D학점 입니다.
    


```python
score = int(input("점수 입력 >> "))
if 90 <= score <= 100:
    r = "A"
elif 80 < score <= 90:
    r = "B"
elif 70 < score <= 80:
    r = "C"
elif 60 < score <= 70:
    r = "D"
elif score < 60:
    r = "F"

print("{}점은 {}학점 입니다.".format(score, r)) 
```

    점수 입력 >> 36
    36점은 F학점 입니다.
    


```python
fruit = ['apple', 'banana','melong','grape']
print(fruit[0])
print(fruit[3])
print(fruit[-2])
```

    apple
    grape
    melong
    


```python
fruit = [1,2,['apple', 'banana', 'melong']]
print(fruit)
```

    [1, 2, ['apple', 'banana', 'melong']]
    


```python

```
