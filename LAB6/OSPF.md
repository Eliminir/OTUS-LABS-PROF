
# Лабораторная работа: OSPF.



### Маршрутизаторы R14-R15 находятся в зоне 0 - backbone
### Маршрутизаторы R12-R13 находятся в зоне 10. Дополнительно к маршрутам должны получать маршрут по-умолчанию
### Маршрутизатор R19 находится в зоне 101 и получает только маршрут по умолчанию
### Маршрутизатор R20 находится в зоне 102 и получает все маршруты, кроме маршрутов до сетей зоны 101
### Настройка для IPv6 повторяет логику IPv4

#### Схема сегмента сети:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/1.JPG)


Настройку OSPF произведем на примере маршрутизатора R14. На нем настроим процесс OSPF, на R15 настройки аналогичные

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/2.JPG)

Конфигурация R12, R13

Настройку OSPF произведем на примере маршрутизатора R12. Настроим процесс OSPF. На R13 настройки аналогичные

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/3.JPG)

Конфигурация R19

R19 находится в area 101 и получает маршрут по умолчанию следовательно эта зона является totally stub

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/4.JPG)

Конфигурация R20

По заданию R20 должен получать все маршруты, кроме маршрутов до area 101 . Для этого на R15 создадим preffix-list, запрещающий прохождение маршрутов до сети network 10.100.1.0 0.0.0.255 и применим его в процессе OSPF на зоне 101


![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/5.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/6.JPG)

Как видно, в таблице маршрутизации на R20 маршрут до сети 10.100.1.0 0.0.0.255 отсутствует

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/7.JPG)

