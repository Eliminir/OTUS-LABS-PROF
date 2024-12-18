## EIGRP

#### Цель:
Настроить EIGRP в С.-Петербург; Использовать named EIGRP


### Описание выполнения домашнего задания:
 В офисе С.-Петербург настроить EIGRP.

R32 получает только маршрут по умолчанию.

R16-17 анонсируют только суммарные префиксы.

Использовать EIGRP named-mode для настройки сети.

### Схема

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB8/1.JPG)


### Выполнение:

R18:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB8/2.JPG)

R17:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB8/3.JPG)

R16:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB8/4.JPG)

В задании указано, что R16-17 анонсируют только суммарные префиксы, для этого необходимо проделать следующие настройки:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB8/9.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB8/10.JPG)



Рассмотрим, что видно после настройки EIGRP на R32

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB8/5.JPG)

Как пример посмотрим, что сети доступны с R18

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB8/11.JPG)













