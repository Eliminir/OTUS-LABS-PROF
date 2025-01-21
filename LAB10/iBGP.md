### iBGP

### Цель:
 Настроить iBGP в офисе Москва

 Настроить iBGP в сети провайдера Триада

 Организовать полную IP связанность всех сетей

 Описание/Пошаговая инструкция выполнения домашнего задания:

  В этой самостоятельной работе мы ожидаем, что вы самостоятельно:

 Настроите iBGP в офисом Москва между маршрутизаторами R14 и R15.

 Настроите iBGP в провайдере Триада, с использованием RR.
 
 Настройте офиса Москва так, чтобы приоритетным провайдером стал Ламас.

Настройте офиса С.-Петербург так, чтобы трафик до любого офиса распределялся по двум линкам одновременно.

 Все сети в лабораторной работе должны иметь IP связность

### Решение:

Добавим IP адреса 1.1.1.14 и 1.1.1.15 для лупбеков R14 и R15

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB10/1.JPG)

 BGP-сессия попытается установиться между соседями по IP адресам с интерфейса Ethernet 1/0, а не по IP адресам с Loopback, которые мы задавали выше.   Чтобы указать роутеру использовать адрес с другого интерфейса выполняем команду update-source Loopback0

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB10/2.JPG)


Из вывода команды show ip bgp summary видим, что сессия успешно установилась

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB10/3.JPG)


### Настройка iBGP в Триаде

 Настроим R23/24/25/26 по аналогии как R14, R15, Из вывода команды show ip bgp summary видим, что сессия успешно установилась.

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB10/4.JPG)


![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB10/5.JPG)


### Настройка RR в Триаде

Настроим R23 как RR serv:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB10/6.JPG)

Настройка R24/R25/R26

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB10/7.JPG)


### Настройка приоритетного провайдера Ламас для офиса в Москве

Для решения увеличим LP(Local Preference) на R15, таким образом трафик через R21 провайдера Ламас станет приорететным.

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB10/8.JPG)

### Настраиваем офис С.-Петербург так, чтобы трафик до любого офиса распределялся по двум линкам одновременно

Балансировку выполняем с помощью помощи команды: maximum-paths

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB10/9.JPG)

