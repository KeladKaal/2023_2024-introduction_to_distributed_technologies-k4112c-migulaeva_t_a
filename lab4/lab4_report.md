University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2023/2024
Group: K4112c
Author: Migulaeva Tatyana Alekseevna
Lab: Lab2
Date of create: 24.09.2023
Date of finished: 

1. Запускаем миникуб с подключенным плагином калико и двумя нодами.
  ![telegram-cloud-photo-size-2-5224497630623682030-y](https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/4228a3e6-8959-4197-893d-0ca31e45878b)

2. Проверяем наличие подов калико.
   ![telegram-cloud-photo-size-2-5224497630623682104-y](https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/4bebcd50-239d-4a8d-a52c-fe270858af0f)

3. Проверяем наличие двух разных нод.
   ![telegram-cloud-photo-size-2-5224497630623682105-y](https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/aee729dd-0ac1-47cc-bc4a-a812cf5860d5)

4. Ставим нодам лейблы.
   ![telegram-cloud-photo-size-2-5224497630623682125-y](https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/42dac82e-888b-420c-b22d-caf2ba4b8148)

5. Удаляем существующий дефолтный ippool, проверяем, что больше никаких не осталось.
    ![telegram-cloud-document-2-5224497630167445884](https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/f48d8f39-e820-49d5-acdc-86c6d07dbd07)

6. Создаём наши созданные ippool. Ещё у меня видимо слишком свежая версия calicoctl, но работе это не помешало.
    ![telegram-cloud-photo-size-2-5224497630623682130-y](https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/144b1fb7-2767-4417-bc63-fcc400ea5e43)

7. Проверяем, что наши ippool создались и с ними всё верно.
    ![telegram-cloud-photo-size-2-5224497630623682131-y](https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/c0a2b28e-9c42-4e6b-941c-b3446f7080e9)

8. Разорачиваем приложение с сервисом. Проверяем, какие айпи адреса были ему назначены. Адреса из тех ippool которые мы создавали, следовательно, всё настроено верно.
    ![telegram-cloud-photo-size-2-5224497630623682136-y](https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/8d05262c-8948-4c70-9156-18adb864093c)

9. Подключаемся к одному из подов, пингуем соседний. Пинг идёт, связь между ними есть.
    ![telegram-cloud-photo-size-2-5224497630623682142-y](https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/6751a40c-7924-4720-a2b8-84939d91f375)

10. Пробрасываем порты сервиса, открываем приложение в браузере. Всё отображается корректно.
    ![telegram-cloud-photo-size-2-5224497630623682143-y](https://github.com/KeladKaal/2023_2024-introduction_to_distributed_technologies-k4112c-migulaeva_t_a/assets/64036217/5c7a1629-83c9-40b5-99ce-cefec8fbdb32)



