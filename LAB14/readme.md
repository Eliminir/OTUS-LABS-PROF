
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

