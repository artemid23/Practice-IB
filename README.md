# Вариант 11 - CollaboraOnline

Состав команды:

Токарь Артём: проектирование схемы инфраструктуры, развёртывание системы, проверка работоспособности,  работа с БДУ ФСТЭК: таблица негативных последствий, модель нарушителя, модель угроз ИБ.

Тарасов Павел: работа с Mitre ATT&CK.

Описание проекта:

Информационная система "Магазин компьютеров и комплектующих"

Описание места установки системы

Описанная инфраструктура развернута в офисе компании. Системы используется для совместной разработки корпоративной документации и ведения бухгалтерии.

Составные части информационной системы:

1. Терминальная машина(сервер);
2. SSH Service;
3. SSH Client;
4. ПК пользователей.
   
В офисе располагается терминальная машина, на ней запущена виртуальная машина на Linux. В виртуальной машине запущен Docker Container с Collabora Online, к которому можно обратиться по определённому порту. Все хосты пользователей и сервер находятся в одной локальной сети. На сервере (терминальной машине) запущена служба SSH Service, на пользовательских ПК запущена служба SSH Client. Аутентификация происходит по паролю. Чтобы пользователю получить доступ к сервису Collabora Online необходимо:
1. Запустить SSH Client;
2. Подключиться к серверу;
3. Открыть терминальную систему;
4. Открыть браузер;
5. Пройти аутентификацию;
5. Открыть web-приложение.

 
