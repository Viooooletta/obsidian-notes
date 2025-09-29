
```
# try:  
#     file = open('text.txt', 'r')  # считывает данные из файла (если его не существует, то выдаст ошибку)  
#     # Ошибка!!!  
#  
#     #Это не выполнелось!  
#     file.read()  
#     file.close()  
# except FileNotFoundError:  
#     print('Файл не найден')  
  
try:  
    with open('text.txt', 'r', encoding='utf-8') as file:  
        print(file.read())  
except FileNotFoundError:  
    print("Файл не найден")
```
Файл был открыт его необходимо закрыть если мы его попытаемся закрыть в блоке finally то не получиться так как file виден в блоке try
Поэтому мы будем использовать менеджер with-as
**with open('text.txt', 'r', encoding='utf-8') as file**
в момент открытия файла мы говорим что этот же файл и будет сам закрываться по завершению его работы поэтому file.close() прописывать не надо