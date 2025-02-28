## Настройка VPN. GRE. DmVPN

#### Цель:

Настроить GRE между офисами Москва и С.-Петербург

Настроить DMVPN между офисами Москва и Чокурдах, Лабытнанги

_________________________________________________________________________________________________________

Описание/Пошаговая инструкция выполнения домашнего задания:

Настроите GRE между офисами Москва и С.-Петербург.

Настроите DMVMN между Москва и Чокурдах, Лабытнанги.

## GRE между офисами Москва и С.-Петербург 

Настройка маршрутизаторов в Moscow:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB13/1.JPG)


Настройка маршрутизаторов в Piter:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB13/2.JPG)

С помощью show ip int brief проверяем все ли мы правильно создали

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB13/3.JPG)


## DMVPN между офисами Москва и Чокурдах, Лабытнанги


В нашей будущей виртуальной сети разделим железки по следующим ролям:

Moscow - HUB

Лабынтаги - SPOKE

Чокурдах - SPOKE



Настроим R15 с ролью HUB:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB13/4.JPG)

R14 настраиваем аналогично

Настроим R27 с ролью SPOKE:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB13/5.JPG)


По аналогии настраиваем R28, с помощью ping проверяем работу

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB13/6.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB13/7.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB13/8.JPG)



