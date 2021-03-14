### 딕셔너리
- Key와 Value를 한 쌍으로 갖는 자료형 


```python
dic1 = {'name' : '최태양', 'age' : 24, 'height' : '179' }

type(dic1)
```




    dict




```python
dic1['weight'] = '80'

print(dic1)
```

    {'name': '최태양', 'age': 24, 'height': '179', 'weight': '80'}
    


```python
dic_test = {'노래제목' : '아무노래'}
dic_test['가수'] = '지코'
dic_test['날짜'] = '2020.01.13'

dic_test
```




    {'노래제목': '아무노래', '가수': '지코', '날짜': '2020.01.13'}




```python
del dic1['name']

dic1
```




    {'age': 24, 'height': '179', 'weight': '80'}




```python
del dic_test['가수']

dic_test
```




    {'노래제목': '아무노래', '날짜': '2020.01.13'}




```python
dic1['height']

# 없을 때 에러 []
```




    '179'




```python
dic1.get('height')

# 없을 때 none .get()
```




    '179'




```python
print(dic1.get("bbb"))
```

    None
    


```python
dic1['name'] = 'A'
```


```python
dic1.keys()
```




    dict_keys(['age', 'height', 'weight', 'name'])




```python
list(dic1.keys())
```




    ['age', 'height', 'weight', 'name']




```python
dic1.values()
```




    dict_values([24, '179', '80', 'A'])




```python
list(dic1.values())
```




    [24, '179', '80', 'A']




```python
dic1.items()
```




    dict_items([('age', 24), ('height', '179'), ('weight', '80'), ('name', 'A')])




```python
list(dic1.items())
```




    [('age', 24), ('height', '179'), ('weight', '80'), ('name', 'A')]




```python
'name' in dic1
```




    True




```python
'age' in dic1
```




    False




```python
dic1.clear()
```


```python
dic1
```




    {}


