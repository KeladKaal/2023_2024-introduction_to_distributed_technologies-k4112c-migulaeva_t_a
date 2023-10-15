University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2023/2024
Group: K4112c
Author: Migulaeva Tatyana Alekseevna
Lab: Lab3
Date of create: 23.09.2023
Date of finished: 

1. Создаём ConfigMap со значениями переменных.
<img width="276" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/a3629760-cd4c-4247-bafb-fdf8fe97025e">

   
2. Создаём ReplicaSet, в который передаём указанные переменные.
 <img width="457" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/d4bf7560-1660-45eb-a673-593e4c9f33cf">


3. Создаём tls секрет, в который прописываем созданные приватный и публичный ключ. Вообще, секреты в коде это некрасиво, и по идее нужно использовать, например, external secrets operator и подтягивать секреты из того же волта, развёрнутого в первой работе. Но в рамках учебной работы, где основную сложность представляет скорее настройка ингресса, сочтём за допустимую вольность.
   <img width="252" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/f41af319-583a-43b9-b84f-b35b70bc5c8e">

   
4. Создаём сервис для приложения.
 <img width="189" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/dc5a09f3-008c-4645-b865-e2b2ae517f1d">


5. Создаём ингресс. В него подтягиваем ключи из секрета, созданного ранее, а также указываем путь, по которому будет доступно наше приложение.
   <img width="277" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/6c938ee4-2cb1-4f23-a3b0-ba18c565bba6">

   
6. Деплоим всё вышеуказанное.
<img width="455" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/6f6ac41c-4510-4678-bbd2-fbc5b4d7c3b4">

7. Далее достаточно запустить minikube addons enable ingress, а также minikube tunnel. После этого всё должно работать, но там произошёл подвох - во всей документации сказано, что в hosts надо указывать ip миникуба, однадо это верно только для Линукс. Для MacOS и Windows нужно указывать локалхост.
 <img width="211" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/1c791e87-f4fa-4762-b74b-ce2c7c93b865">

   
8. Переходим в браузер, всё открывается.
   <img width="1156" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/8ced1f08-f1d3-445c-bbdb-48cac2751de1">


9. Сертификат.
<img width="644" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/12d4a024-8992-43a3-a59f-59324d9aa405">

Схема
<img width="953" alt="image" src="https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/c948f024-2ea7-4cc4-965a-d3b6e7c4a898">
