
```
person = {
	'user_1': {
		 'name': 'Bob',
		 'age': 23,
		 'adress': ('г. Москва', 'ул. Какая-то'),
		 'grades': {
			 'math': 5,
			 'phythics': 4
			 }
	},
	'user_2': {
		'name': 'Joy'}
print (person['user_1'][adress][1])
```


Получим: ул. Какая-то
```
country = {'code': 'BY', 'name': 'Belarus, 'population': 9002002}
print(country['name'])
for key in country:
	print(key)
```

Получим только ключи:
Belarus
code
name
population

Если хотим получить не только ключи, но еще и значения, нужно прописать: 

```
country = {'code': 'BY', 'name': 'Belarus, 'population': 9002002}
print(country.items())
```
Получим:
dict_items([('code', 'BY'), ('name', 'Belarus'), ('population', 9002002)])

```
country = {'code': 'BY', 'name': 'Belarus', 'population': 9002002}  
for key, value in country.items():  
    print(key, value)
```
Получим:
code BY
name Belarus
population 9002002

ИЛИ

```
country = dict(code = 'BY', name = 'Belarus')
print (country['name'])```
```
Получим: Belarus

```
country = {'code': 'BY', 'name': 'Belarus, 'population': 9002002}
for key in country:
	print(key)
```

Получим (то есть вместо 0 1 2 у нас будут выводиться ключи)
code
name
population

##### Вместо 

```
print (country[4])
```

Можно написать:
```
print(country.get('name'))
```

**country.clear()** - очищает наш словарь от всех элементов
**country.pop('name')** - удалит элемент у которого ключ name
**country.popitem()** - удалит последний элемент 
**country.values()** - получим все значения 
**country.items()** - получим список из картежей в которых элементы это ключ и значение соответственно
**country['code'] = 'RU'** - обновление значения 
**country.update({})** - обновление значения 