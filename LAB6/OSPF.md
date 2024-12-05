
# Лабораторная работа: OSPF  :earth_americas::earth_americas::earth_americas:


### Задание
#### 1.Маршрутизаторы R14-R15 находятся в зоне 0 - backbone
#### 2.Маршрутизаторы R12-R13 находятся в зоне 10. Дополнительно к маршрутам должны получать маршрут по-умолчанию
#### 3.Маршрутизатор R19 находится в зоне 101 и получает только маршрут по умолчанию
#### 4.Маршрутизатор R20 находится в зоне 102 и получает все маршруты, кроме маршрутов до сетей зоны 101
#### 5.Настройка для IPv6 повторяет логику IPv4

#### Схема сегмента сети:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/1.JPG)

#### Конфигурация R14, R15

Настройку OSPF произведем на примере маршрутизатора R14. На нем настроим процесс OSPF, на R15 настройки аналогичные

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/2.JPG)

#### Конфигурация R12, R13

Настройку OSPF произведем на примере маршрутизатора R12. Настроим процесс OSPF. На R13 настройки аналогичные

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/3.JPG)

#### Конфигурация R19

R19 находится в area 101 и получает маршрут по умолчанию следовательно эта зона является stub

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/4.JPG)

#### Конфигурация R20

По заданию R20 должен получать все маршруты, кроме маршрутов до area 101 . Для этого на R15 создадим preffix-list, запрещающий прохождение маршрутов до сети network 10.100.1.0 0.0.0.255 и применим его в процессе OSPF на зоне 101 :cop:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/5.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/6.JPG)

Как видно, в таблице маршрутизации на R20 маршрут до сети 10.100.1.0 0.0.0.255 отсутствует :heavy_check_mark:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB6/7.JPG)

