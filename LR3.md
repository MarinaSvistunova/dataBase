1. Создание таблиц Idols и Groups:
![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/1.jpg)
![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/3.jpg)

2. Наполнение таблиц данными.
   Например, таблица Groups.
   ![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/5.jpg)

3. Результат заполнения таблиц данными:
   ![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/6.jpg)
   ![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/tabIdl.jpg)
   ![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/tabIdl2.jpg)
   
4. Выбор всех столбцов из таблицы Groups:
   Запрос: SELECT * FROM Groups;
   ![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/7.jpg)
   
5. Выбор столбцов Nickname, Last_name, Age, Role таблицы Idols, таких что Last_name = 'Kim' и Age >= 23:
   Запрос: SELECT Nickname, Last_name, Age, Role FROM Idols WHERE Last_name = 'Kim' AND Age >= 23;
   ![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/8.jpg)
   
6. Выбор столбцов Idols.Last_name, Idols.First_name, Idols.Group_name, Groups.Members таблиц Idols и Groups, 
   таких что Idols.Group_name = Groups.Group_name и Role = 'rapper' и Idols.Group_name != 'TXT' и Members = '9':
   Запрос: SELECT Idols.Last_name, Idols.First_name, Idols.Group_name, Groups.Members FROM Idols, Groups
           WHERE Idols.Group_name = Groups.Group_name AND Role = 'rapper' AND Idols.Group_name != 'TXT' AND Members = '9';
   ![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/9.jpg)

7. Выбор столбцов Nickname, Last_name, First_name, Age таблицы Idols, таких что First_name начинается с 'Ta':
   Запрос: SELECT Nickname, Last_name, First_name, Age FROM Idols WHERE First_name LIKE 'Ta%';
   ![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/10.jpg)
   
8. Выбор столбцов Nickname, Last_name, First_name, Group_name, Age таблицы Idols, 
   таких что (Age != '26' и Group_name = 'BTS')или (Age != '23' и Group_name = 'EXO'):
   Запрос: SELECT Nickname, Last_name, First_name, Group_name, Age FROM Idols 
           WHERE (Age != '26' AND Group_name = 'BTS') OR (Age != '23' AND Group_name = 'EXO');
   ![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/11.jpg)
   
9. Изменение записи, где Nickname = 'Yoona':
   Запрос: UPDATE Idols SET Age = '150' WHERE Nickname = 'Yoona';
   ![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/12.jpg)

9. Удаление записи, где Age = '150':
   Запрос: DELETE FROM Idols WHERE Age = '150';
   ![alt text](https://github.com/MarinaSvistunova/dataBase/blob/master/src/13.jpg)
   
   
