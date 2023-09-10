University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2023/2024
Group: K4112c
Author: Migulaeva Tatyana Alekseevna
Lab: Lab1
Date of create: 10.09.2023
Date of finished: 

1. Запускаем minikube.
2. Создаём файл деплоймента. 
3. Разворачиваем его в кластере.
4. Создаём сервис. (Командой слишком просто, а кодом красивее, поэтому вот код)
5. Деплоим сервис.
6. Прокидываем порт и волт открывается в браузере.
7. Для получения токена открываем логи пода, там видим его.
8. Волт работает.

Ответы на вопросы:
1. Мы развернули приложение для хранения секретов в кубере. Для этого развернут один деплоймент с двумя подами и 1 сервис для подключения к нему. 
2. Токен для входа в логах пода, там же, где ключ для ансила.