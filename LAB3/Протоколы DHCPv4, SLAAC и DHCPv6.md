## Реализация DHCPv4/6

### Реализация DHCPv4

### *Топология сети*

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/1.JPG)

### *Таблица адресации*

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/2.JPG)

### *Таблица VLAN*

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/3.JPG)




Шаг 1.	Создание схемы адресации

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/4.JPG)

Шаг 2.	Создаем сеть согласно топологии

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/5.JPG)


Шаг 3.	Производим базовую настройку маршрутизаторов

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/6.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/7.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/8.JPG)

Шаг 4.	Настройка маршрутизации между сетями VLAN на маршрутизаторе R1



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/9.JPG)




![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/10.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/11.JPG)

Шаг 5.	Настраиваем G0/1 на R2, затем G0/0/0 и статическую маршрутизацию для обоих маршрутизаторов



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/12.JPG)



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/13.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/14.JPG)



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/15.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/16.JPG)


![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/17.JPG)


![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/18.JPG)



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/19.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/20.JPG)

Шаг 7.	Создаем сети VLAN на коммутаторе S1



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/21.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/22.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/23.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/24.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/25.JPG)

Шаг 8.	Назначаем сети VLAN соответствующим интерфейсам коммутатора



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/26.JPG)



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/27.JPG)



Шаг 9.	Вручную настраиваем интерфейс S1 F0/5 в качестве транка 802.1Q



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/28.JPG)



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/29.JPG)



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/30.JPG)





![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/32.JPG)


Если бы пк не был подключен к сети с помощью DHCP, он бы автоматически себе бы сам настроийл IP в диапозоне 169.254.x.x

## Часть 2.	Настройка и проверка двух серверов DHCPv4 на R1

Шаг 1.	Настраиваем R1 с пулами DHCPv4 для двух поддерживаемых подсетей



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/33.JPG)



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/34.JPG)



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/35.JPG)



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/36.JPG)


![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/37.JPG)



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/38.JPG)



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/39.JPG)


	Попытка получить IP-адрес от DHCP на PC-A



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/42.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/43.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/44.JPG)

___

### Часть 3.	Настройка и проверка DHCP-ретрансляции на R2

Шаг 1.	Настройка R2 в качестве агента DHCP-ретрансляции для локальной сети на G0/0/1



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/45.JPG)



![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/46.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/47.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/48.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/49.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/50.JPG)


## Реализация DHCPv6

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/51.JPG)


Базовые настройки и прочее мы делали ранее так что пропускаем данные шаги) Едиснтвенное активируем IPv6-маршрутизацию командой на обоих роутерах  ipv6 unicast-routing

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/52.JPG)



Шаг 4. Настройка интерфейсов и маршрутизации для обоих маршрутизаторов




![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/53.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/54.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/55.JPG)

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/56.JPG)


## Часть 2. Проверка назначения адреса SLAAC от R1

Через несколько минут результаты команды ipconfig должны показать, что PC-A присвоил себе адрес из сети 2001:db8:1::/64

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/57.JPG)

Откуда взялась часть адреса с идентификатором хоста? }{ост сам себе генерирует случайный 64-битный адрес

### Часть 3. Настройка и проверка сервера DHCPv6 на R1

Шаг 1. Более подробно изучаем конфигурацию PC-A

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/58.JPG)


Шаг 2. Настраиваем R1 для предоставления DHCPv6 без состояния для PC-A


a.	Создаем пул DHCP IPv6 на R1 с именем R1-STATELESS. В составе этого пула назначаем адрес DNS-сервера как 2001:db8:acad: :1, а имя домена — как stateless.com

b.	Настраиваем интерфейс G0/0/1 на R1, чтобы предоставить флаг конфигурации OTHER для локальной сети R1 и указываем только что созданный пул DHCP в качестве ресурса DHCP для этого интерфейса

c.	Сохраняем текущую конфигурацию в файл загрузочной конфигурации

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/59.JPG)

d.	Перезапускаем PC-A

e.	Проверяем вывод ipconfig /all и обратите внимание на изменения

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/60.JPG)

f.	Тестируем подключения с помощью пинга IP-адреса интерфейса G0/1 R2


### Часть 4. Настройка сервера DHCPv6 с сохранением состояния на R1

a.	Создаем пул DHCPv6 на R1 для сети 2001:db8:acad:3:aaa::/80. Это предоставит адреса локальной сети, подключенной к интерфейсу G0/0/1 на R2. В составе пула задаем DNS-сервер 2001:db8:acad: :254 и задаем доменное имя STATEFUL.com.

b.	Назначаем только что созданный пул DHCPv6 интерфейсу g0/0/0 на R1

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/61.JPG)


### Часть 5. Настройка и проверка ретрансляции DHCPv6 на R2

Шаг 1. Включаем PC-B и проверьте адрес SLAAC, который он генерирует

![alt text](https://github.com/Eliminir/OTUSLABS/blob/Labs/LAB8/62.JPG)





  
