## BGP Основы :space_invader::space_invader::space_invader::space_invader::space_invader:




Настраиваем eBGP между офисом Москва и двумя провайдерами - Киторн и Ламас.

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB9/1.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB9/2.JPG)

Настраиваем eBGP между провайдерами Киторн и Ламас.

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB9/3.JPG)


Настраиваем eBGP между Ламас и Триада.

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB9/4.JPG)


Настраиваем eBGP между офисом С.-Петербург и провайдером Триада.

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB9/5.JPG)

Организовываем IP доступность между пограничным роутерами офисов Москва и С.-Петербург, проверяем корректность c помощью ping с R14 на R18 и наоборот

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB9/6.JPG)

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB9/7.JPG)

Как пример правильности проведенных работ, вывод команды show ip route на R21, из него видим что как и задуманно анонсируються два наших маршрута из московской и питерской сети

![alt text](https://github.com/Eliminir/OTUS-LABS-PROF/blob/main/LAB9/8.JPG)
