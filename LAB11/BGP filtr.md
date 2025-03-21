### BGP. Фильтрация :passport_control::passport_control::passport_control:


Цель:

Настроить фильтрацию для офисе Москва

Настроить фильтрацию для офисе С.-Петербург


### Описание/Пошаговая инструкция выполнения домашнего задания:



Настроить фильтрацию в офисе Москва так, чтобы не появилось транзитного трафика(As-path).

Настроить фильтрацию в офисе С.-Петербург так, чтобы не появилось транзитного трафика(Prefix-list).

Настроить провайдера Киторн так, чтобы в офис Москва отдавался только маршрут по умолчанию.

Настроить провайдера Ламас так, чтобы в офис Москва отдавался только маршрут по умолчанию и префикс офиса С.-Петербург.




### Фильтрация транзитного трафика в Moscow


Напишем на R14 и R15 правила для предотвращения транзита (пример команды был на последней лекции):

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB11/1.JPG)


### Фильтрация транзитного трафика в Piter


Разрешаем анонсить только клиенские сети:


![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB11/2.JPG)


### Настройка Киторн, в Moscow отдается только маршрут по умолчанию


![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB11/3.JPG)


### Настраиваем Ламас так, чтобы в Moscow отдавался только маршрут по умолчанию и префикс от Piter

Пропишем чтобы R21 отправлял R15 маршрут по умолчанию и отбрасывал все префиксы, кроме содержащий в начале пути Piter(AS888):

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB11/4.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB11/5.JPG)


### Настройка фильтрации для входящих анонсов в Moscow



Настроим R15 на прием default и маршрутов из Piter :

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB11/6.JPG)

Настроим R14 на прием только default:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB11/7.JPG)






