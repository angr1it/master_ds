# Проект 0. Угадай число

## Оглавление  
[1. Описание проекта](README.md#Описание-проекта)  
[2. Какой кейс решаем?](README.md#Какой-кейс-решаем)  
[3. Этапы работы над проектом](README.md#Результат)  
[4. Результат](README.md#Этапы-работы-над-проектом)  
[5. Запуск](README.md#Комментарии-к-решению-ДЗ)  
[6. Комментарии к решению ДЗ](README.md#Комментарии-к-решению-ДЗ)  
[7. Выводы](README.md#Выводы)  

### Описание проекта    
Угадать загаданное компьютером число за минимальное число попыток.


### Какой кейс решаем?    
Нужно написать программу, которая угадывает число за минимальное число попыток

**Условия соревнования:**  
- Компьютер загадывает целое число от 0 до 100, и нам его нужно угадать. Под «угадать», подразумевается «написать программу, которая угадывает число».
- Алгоритм учитывает информацию о том, больше ли случайное число или меньше нужного нам.

**Метрика качества**     
Результаты оцениваются по среднему количеству попыток при 1000 повторений

**Что практикуем**     
Учимся писать хороший код на python


### Этапы работы над проектом  

Решил задачу методом двух указателей.


### Результат

Алгоритм угадывает число в среднем за 5 попыток / циклов (x2 вызовов сравнений со скрытым числом).


### Запуск

**Запуск через Docker**  
```
docker compose build
docker compose run --rm guess_num python -m game
```
тесты:
```
docker compose run --rm guess_num pytest
```
Также доступен запуск через devcontainer в vscode.

**Запуск при наличии python==3.11**  
```
pip install -r requirements.txt
python -m game
```
тесты:
```
pytest
```

**Notebooks**  
Также доступен запуск через jupyter: 'notebooks/game.ipynb' (devcontainer настроен для запуска jupyter через vscode).


### Комментарии к решению ДЗ

**Docker**  
Использую всегда, т.к. на локальную машину не ставлю ничего под разработку.  

**Jupyter/Colab**   
Использовать notebooks\baseline.ipynb, т.к. не содержит импортов.


### Выводы

Реализованный алгоритм работает в соответствии с условием.

:arrow_up:[к оглавлению](README.md#Оглавление)