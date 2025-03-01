###  Основные протоколы сети интернет :globe_with_meridians:

### Цель:

Настроить DHCP в офисе Москва.

Настроить синхронизацию времени в офисе Москва.

Настроить NAT в офисе Москва, C.-Перетбруг и Чокурдах.

### В этой самостоятельной работе мы ожидаем, что вы самостоятельно:

Настроите NAT(PAT) на R14 и R15. Трансляция должна осуществляться в адрес автономной системы AS1001.

Настроите NAT(PAT) на R18. Трансляция должна осуществляться в пул из 5 адресов автономной системы AS2042.

Настроите статический NAT для R20.

Настроите NAT так, чтобы R19 был доступен с любого узла для удаленного управления.

Настроите статический NAT(PAT) для офиса Чокурдах.

Настроите для IPv4 DHCP сервер в офисе Москва на маршрутизаторах R12 и R13. VPC1 и VPC7 должны получать сетевые настройки по DHCP.

Настроите NTP сервер на R12 и R13. Все устройства в офисе Москва должны синхронизировать время с R12 и R13.


### Настраиваем NAT на R14 и R15

Пример настроек R14, на R15 прописываем аналогичное

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/1.JPG)


### Настраиваем NAT на R18(Piter)

В отличие от Московского офиса пул внешних айпи адресов будет из 5 адресов.

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/2.JPG)


### Статический NAT для R20(Moscow)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/3.JPG)


### R19 был доступен с любого узла для удаленного управления :computer:

Настроим подключение на R19 по telnet, для управления:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/4.JPG)

Проверяем:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/5.JPG)

### Настраиваем DHCPv4 на R12 и R13


На R12 выделим пулы адресов 100.0.0.1 - 100.0.0.100 и 100.0.1.1 - 100.0.1.100

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/6.JPG)

На R13 выделим пул адресов 100.0.0.100-100.0.0.255 и 100.0.1.100-100.0.1.255

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/7.JPG)

### Настраиваем NTP сервера :watch:

Так как доступа в интернеты нет, мастер серверами откуда будет подтягиваться NTP служат R12, R13

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/8.JPG)

На необходимых роутерах:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/9.JPG)

На необходимых комуттаторах:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/10.JPG)

Проверка:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/11.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/12.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB12/13.JPG)





