Создаем папку test_volume и в ней файл test.txt для монтирования в контейнер.


![Screenshot from 2023-07-01 21-54-30.png](Screenshots%2FScreenshot%20from%202023-07-01%2021-54-30.png)

Создаем контейнер mytest   hostname:myhost  и монтируем к нему папку test_volume 
в папку data нашего контейнера.
Проверяем создалась ли папка в контейнере.

Монтируем туда же файл test.txt
Проверяем содержимое файла.

![Screenshot from 2023-07-01 21-58-26.png](Screenshots%2FScreenshot%20from%202023-07-01%2021-58-26.png)

Вносим изменения в наш файл в хостовой системе, запускаем койнтейнер
и проверяем изменился ли наш смонтированный туда файл.

![Screenshot from 2023-07-01 22-04-09.png](Screenshots%2FScreenshot%20from%202023-07-01%2022-04-09.png)

Создаем контейнер с базой данных mysql.

![Screenshot from 2023-07-01 22-33-03.png](Screenshots%2FScreenshot%20from%202023-07-01%2022-33-03.png)

Создаем контейнер с phpadmin и связываем его с контейнером mysql через порты 8081:80

![Screenshot from 2023-07-01 22-39-05.png](Screenshots%2FScreenshot%20from%202023-07-01%2022-39-05.png)

Заходим в контейнер и запускаем среду mysql для создания базы данных и таблицы.

![Screenshot from 2023-07-03 07-24-53.png](Screenshots%2FScreenshot%20from%202023-07-03%2007-24-53.png)

Создаем базу данных my_data.

![Screenshot from 2023-07-03 07-31-39.png](Screenshots%2FScreenshot%20from%202023-07-03%2007-31-39.png)

Создаем таблицу data_1.

![Screenshot from 2023-07-03 07-50-34.png](Screenshots%2FScreenshot%20from%202023-07-03%2007-50-34.png)

В браузере открываем phpadmin и проверяем что таблица создана.

![Screenshot from 2023-07-03 07-52-07.png](Screenshots%2FScreenshot%20from%202023-07-03%2007-52-07.png)