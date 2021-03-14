### 리스트 (list)

- 복수개의 값을 담을 수 있는 데이터 구조
- list: mutable (생성된 후에 변경 가능)


```python
list11 = ['a', 'b', 'c', 'd', 'e', 'f']
list11.index('c')
```




    2




```python
list11 = [1, 2,3, 5, 43, 6]
list11.sort()
list11
```




    [1, 2, 3, 5, 6, 43]




```python
list12 = ['a', 'b', 'c', 'd', 'e', 'f']
list12.pop()
```




    'f'




```python
'a' in list12
```




    True




```python
list12
```




    ['a', 'b', 'c', 'd', 'e']




```python
list12.reverse()
list12
```




    ['e', 'd', 'c', 'b', 'a']




```python
len(list12)
```




    5




```python
list14 = ['a', 'b', 'c', 'd', 'e', 'f']
len(list14)
```




    6




```python
n_list12 = sorted(list12)
print(list12)
print(n_list12)
```

    ['e', 'd', 'c', 'b', 'a']
    ['a', 'b', 'c', 'd', 'e']
    

### 튜플 (tuple)

- 복수개의 값을 담을 수 있는 데이터 구조
- tuple : immutable (생성된 후에 변경 불가능)


```python
t1 = (0, 1, 2, 3, 4,5)
len(t1)

```




    6




```python
tp = ("apple",)
print(type(tp))
```

    <class 'tuple'>
    


```python
5 in t1
```




    True




```python
t2 = (6, 7, 8)

t3 = t1 + t2
t3
```




    (0, 1, 2, 3, 4, 5, 6, 7, 8)




```python
min(t1)
```




    0




```python
t2.count(1)
```




    0




```python
str1 = "파이썬 최고"
"파이썬" in str1
```




    True




```python
"파이썬" not in str1
```




    False




```python
list1 = [77, 38, 10]
33 in list1
```




    False




```python
33 not in list1
```




    True




```python
list1.remove(12)
list1
```




    [38, 10, 12]




```python
list1.append(11)
list1
```




    [38, 10, 12, 11, 11]




```python
list1.append(12)
list1
```




    [38, 10, 12, 11, 11, 12]


