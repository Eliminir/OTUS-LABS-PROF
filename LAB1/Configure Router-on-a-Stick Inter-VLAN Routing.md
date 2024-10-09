# Configure Router-on-a-Stick Inter-VLAN :metro:

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/1.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/2.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/3.JPG)

## Configure basic settings for the router

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/4.JPG)

## Configure basic settings for each switch

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/5.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/6.JPG)

## Configure PC hosts

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/7.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/8.JPG)

## Create VLANs and Assign Switch Ports

Create VLANs on both switches

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/9.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/10.JPG)

## Asign VLANs to the corect switch interfaces

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/11.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/12.JPG)


## Configure an 802.1Q Trunk Between the Switches

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/13.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/14.JPG)


Manually configure S1’s trunk interface F0/5

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/15.JPG)


:thought_balloon: Почему F0/5 не отображается в списке?

S1 port 5 не будет отображаться, поскольку интерфейс GigabitEthernet 0/0/1 на маршрутизаторе отключен.

## Configure Inter-VLAN Routing on the Router

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/16.JPG)


Verify Inter-VLAN Routing is Working

Ping from PC-A to its default gateway

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/17.JPG)

Ping from PC-A to PC-B

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/18.JPG)

 Ping from PC-A to S2

 ![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/19.JPG)

## Complete the following test from PC-B

 ![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB1/20.JPG)

 :thought_balloon: Какие промежуточные IP-адреса указаны в результатах?

 192.168.4.1 - Default Gateway PC B int R1 G0/0/1.4


 :ghost::ghost::ghost:


