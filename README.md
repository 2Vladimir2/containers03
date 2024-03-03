## **Лабораторная работа:IWNO3** 
*Использование контейнеров как среды выполнения*
## **Целт работы**
*Данная лабораторная работа призвана напомнить основные команды ОС Debian/Ubuntu. Также она позволит познакомиться с Docker и его основными командами.*
## **Задание**
*Запустить контейнер Ubuntu, установить Web-сервер Apache и вывести в браузере страницу с текстом "Hello, World!".*
## **Выполнение**
*Создайте репозиторий containers03 и склонируйте его себе на компьютер.

Создайте в папке containers03 файл README.md который содержать пошаговое выполнение проекта. Описание проекта должно содержать:*
## **Запуск и тестирование**
*Откройте терминал в папке containers03 и выполните команду:*

*docker run -ti -p 8000:80 --name containers03 ubuntu bash*

*В открывшемся окне выполните следующие команды и объясните их назначение:*

*apt update*

*apt install apache2 -y*

*service apache2 start*

*Откройте браузер и введите в адресной строке http://localhost:8000.*

*Что вы видите?*
*<img width="1440" alt="image" src="https://github.com/2Vladimir2/containers03/assets/159247721/4968db73-88a4-4e6f-9cdf-f0c136b8c9c5">*

*Выполните следующие команды:*
*ls -l /var/www/html/*
*echo '<h1>Hello, World!</h1>' > /var/www/html/index.html*

*Обновите страницу в браузере. Что вы видите?*

*Я вижу надпись "Hello world"*

*Выполните следующие команды:*

*cd /etc/apache2/sites-enabled/
cat 000-default.con*

*Что вы видите на экране?*

*<img width="372" alt="image" src="https://github.com/2Vladimir2/containers03/assets/159247721/4e0afda5-1002-4f31-bd03-b1fa4c4879ef">*

*Закройте окно терминала командой exit.*

*Просмотрите список контейнеров:*

*<img width="794" alt="image" src="https://github.com/2Vladimir2/containers03/assets/159247721/c3c76eba-97ea-4bb0-9362-bd1f8d23dcd6">*

*Удалите контейнер:*

*<img width="421" alt="image" src="https://github.com/2Vladimir2/containers03/assets/159247721/5345663f-26a3-41d9-b24a-2183ab779c76">*









