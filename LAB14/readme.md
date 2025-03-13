
## IPSec over DmVPN

Цель:

Настроить GRE поверх IPSec между офисами Москва и С.-Петербург

Настроить DMVPN поверх IPSec между офисами Москва и Чокурдах, Лабытнанги

Дополнительно: Для IPSec использовать CA и сертификаты.

## GRE поверх IPSec между офисами MOSCOW и PITER

У нас уже есть созданные Tunnel1000 и Tunnel1001 (поднимали в прошлой лабе), буду настраивать IPSec на них.

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB14/1.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB14/2.JPG)

Подобно настраиваем и шифрование Tunnel1001

### Настраиваем DMVPN поверх IPSec между Москва и Чокурдах, Лабытнанги.

DMVPN между Москва и Чокурдах, Лабытнанги (поднимали в прошлой лабе) нужно сверху накрутить IPSec, используем тот же профиль что и выше

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB14/3.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB14/4.JPG)

## Настраиваем CA и сертификаты

План:

1) Настроить CA
2) Запросить выдачу сертификатов и предоставить сертификаты
3) Прикрутить к IPSec работу через сертификаты

Параметры сертов:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB14/5.JPG)

Настройка CA

Роль CA будет выполнять R15

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB14/7.JPG)

Настройка клиента

На всех железках, участвующих в VPN, выполняем

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB14/8.JPG)

Настройка trust point:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB14/9.JPG)

Настройка IPSec

Далее настройки IPSec и применение профиля делаем по аналогии описанного выше, единственное тип аутентификации меняется с authentication pre-share на authentication rsa-sig.

