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
   <img width="605" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/55468d67-ad1b-4ec2-bdde-7436abc874dc">

2. Создаём файл деплоймента.  
<img width="605" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/2203aebd-f78d-40da-8ef1-00e9b006270f">

3. Разворачиваем его в кластере.  
  <img width="602" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/2a32e06d-547d-4c5c-bd66-1583725c5395">

4. Создаём сервис. (Командой слишком просто, а кодом красивее, поэтому вот код)  
  <img width="396" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/06d773cf-cfd5-477e-93c1-97644c79d974">

5. Деплоим сервис.  
    <img width="602" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/769adfa1-0401-4e25-8377-778297ece862">

6. Прокидываем порт и волт открывается в браузере.  
    <img width="602" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/2620b909-2e67-4167-a778-ecc557436936">

7. Для получения токена открываем логи пода, там видим его.  
 <img width="605" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/6a2a2703-92a2-4554-bfe4-9101e3252e4d">

8. Волт работает.  
<img width="599" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/b4f95d17-534b-4133-99a5-01f6316dd251">


Ответы на вопросы:  
1. Мы развернули приложение для хранения секретов в кубере. Для этого развернут один деплоймент с двумя подами и 1 сервис для подключения к нему. 
2. Токен для входа в логах пода, там же, где ключ для ансила.

Схема  
<img width="900" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/da9c6f08-3f56-4150-9779-612f7efefcc2">
