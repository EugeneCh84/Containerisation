Создаем новую папку test_py_project. В ней создаем Dockerfile, скрипт Python и т.д.

![Screenshot from 2023-07-05 13-37-12.png](Screenshots%2FScreenshot%20from%202023-07-05%2013-37-12.png)

В файл записываем команды для создания контейнера.
Задаем рабочую директорию.
Создаем виртуальную среду и указываем путь к ней.
Копируем файл requirments.txt ( для данного проекта необязательно ).


![Screenshot from 2023-07-05 13-39-01.png](Screenshots%2FScreenshot%20from%202023-07-05%2013-39-01.png)

Создаем образ на основе python согласно командам из Dockerfile.

![Screenshot from 2023-07-05 13-41-42.png](Screenshots%2FScreenshot%20from%202023-07-05%2013-41-42.png)

Создаем контейнер my_proj из образа test1. 
Чтобы иметь возможность впоследствии редактировать проект, монтируем его как Volume.
 -v $(pwd):/app - команда монтирования, pwd - т.к. монтирую из текущей директории.

![Screenshot from 2023-07-05 13-47-42.png](Screenshots%2FScreenshot%20from%202023-07-05%2013-47-42.png)

Исходный код скрипта python.

![Screenshot from 2023-07-05 13-53-37.png](Screenshots%2FScreenshot%20from%202023-07-05%2013-53-37.png)