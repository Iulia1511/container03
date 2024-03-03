# Лабараторная работа №2
## Цель работы
* Данная лабораторная работа призвана напомнить основные команды ОС Debian/Ubuntu. Также она позволит познакомиться с Docker и его основными командами.
## Задание
* Запустить контейнер Ubuntu, установить Web-сервер Apache и вывести в браузере страницу с текстом "Hello, World!".
## Описание выполнения работы с ответами на вопросы.
### Создайте репозиторий containers03 и склонируйте его себе на компьютер.
![a1](https://github.com/Iulia1511/container03/assets/159126852/c3386a41-75bd-4b46-a1eb-1399805c6aa9)
### Откройте терминал в папке containers03 и выполните команду:
![A2](https://github.com/Iulia1511/container03/assets/159126852/cc84a8e5-ae8f-4849-933a-6b3cadf3c12d)
### В открывшемся окне выполните следующие команды и объясните их назначение:apt updateapt; install apache2 -y; service apache2 start.
![A3](https://github.com/Iulia1511/container03/assets/159126852/55810a29-dc65-41f3-8817-ff65ce299638)
![A4](https://github.com/Iulia1511/container03/assets/159126852/8be6c786-399b-43e9-af25-0d074a127dff)
![A5](https://github.com/Iulia1511/container03/assets/159126852/4d606f18-0028-4967-b266-2ad730ed6148)
![A6](https://github.com/Iulia1511/container03/assets/159126852/8e19ee39-dbf0-4acc-bb03-ba398fdbc35c)
![A7](https://github.com/Iulia1511/container03/assets/159126852/b382fb75-728c-4d2c-9225-631dec87b3dc)
* apt update: Обновляет список доступных пакетов.
* apt install apache2 -y: Устанавливает веб-сервер Apache.
* service apache2 start: Запускает веб-сервер Apache.
### Откройте браузер и введите в адресной строке http://localhost:8000. Что вы видите?
![A8](https://github.com/Iulia1511/container03/assets/159126852/518a67fb-7e1a-44bb-8cb7-96e0e8c5fcd8)
### Выполните следующие команды: ls -l /var/www/html/; echo '< h1>Hello, World!</ h1>' > /var/www/html/index.html
![A9](https://github.com/Iulia1511/container03/assets/159126852/0bc478c2-4b29-4ff9-bd28-3bc374eabb96)
* ls -l /var/www/html/ - это команда для вывода списка файлов и папок в директории /var/www/html/ с дополнительной информацией о каждом файле или папке.
* echo '< h1>Hello, World!</ h1>' > /var/www/html/index.html - это команда, которая создает файл index.html в директории /var/www/html/ и записывает в него текст < h1 >Hello, World!</ h1 >.
### Обновите страницу в браузере. Что вы видите?
![A10](https://github.com/Iulia1511/container03/assets/159126852/7b0cccb9-1db0-4985-9a9d-d5bf27e05e53)
### Выполните следующие команды:cd /etc/apache2/sites-enabled/; cat 000-default.conf
![A11](https://github.com/Iulia1511/container03/assets/159126852/33818ea8-eaa0-4bc2-a652-bfa83b0a8007)
* cd /etc/apache2/sites-enabled/ - переходит в директорию, где хранятся файлы конфигурации виртуальных хостов веб-сервера Apache.
* cat 000-default.conft - выводит содержимое файла 000-default.conft на экран. 
## Просмотрите список контейнеров: docker ps -a
![A12](https://github.com/Iulia1511/container03/assets/159126852/1dab768c-e130-4919-964d-6b852aa02aff)






