## Лабораторная работа базовая настройка is is


### Задание

  Настроите IS-IS в ISP Триада.

  R23 и R25 находятся в зоне 2222.

  R24 находится в зоне 24.

  R26 находится в зоне 26.

### Схема лабы:
![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB7/1.JPG)


  Выполняем на R23, R24, R25, R26 идентичные настройки, указываем разные AREA


router isis
net 49.2222.5223.0000.0001.00 

  где 49 - указывает тип адреса (у нас – приватный), 2222 - номер зоны, 0000.0000.0000 - ID устройства, 00 - селектор


  На интерфейсах выполняем

(config-if)#ip router isis

  После выполнения настроек видим, что соседство установилось

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB7/2.JPG)

  Маршруты распространились:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB7/3.JPG)


