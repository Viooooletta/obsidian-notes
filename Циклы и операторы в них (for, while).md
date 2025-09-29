#### For - цикл
**range** - перебирает числа
**Любая строка это список из множества символов**
```
`for i in range(6):`
	`print(i)`
```
Получим:  0    1 2 3 4 5 
         (0) (1) ...     (5)

```
`for i in range(1, 6):`
	`print(i)`
```
Получим: 1 2 3 4 5 

```
`for i in range(1, 6, 2):`
	`print(i)`
```
Получим: 1 3 5 (потому что третья переменная в range это шаг)

```
word = 'Hello'
for i in word:
	print(i)
```
Получим: 
H
e
l
l
o

```
count = 0
word = 'Hello'
for i in word:
	if i == "l":
		count ++
		print("I fount a part of love!")
print("Count: ", count)
```


#### While
```
i = 7
while i < 13:
	print(i)
	i++
```
В цикле While пока условие будет истинным программа будет выполняться ```while True```  бесконечный цикл 



#### Операторы 
https://youtu.be/z_2AdMZW53I?si=pHCbsEnP2yxsJPL5
**break** - преждевременный выход из цикла 
```
for i in range(1, 6):
	if i == 4:
		break
```

**continue** - преждевременно переходит к новой итерации 
**pass** - глушит то что мы хотели выйти из цикла (несмотряна условия мы продолжаем)