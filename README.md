# Домашнее задание к занятию 2 «Кластеризация и балансировка нагрузки» Бетко Алексей

### Задание 1
- Запустите два simple python сервера на своей виртуальной машине на разных портах
- Установите и настройте HAProxy, воспользуйтесь материалами к лекции по [ссылке](2/)
- Настройте балансировку Round-robin на 4 уровне.
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.

файл с настройками 
[haproxy.cfg](files/haproxy.cfg)

перенаправление
<img src = "img/1.png" width = 100%>
<img src = "img/2.png" width = 100%>


### Задание 2
- Запустите три simple python сервера на своей виртуальной машине на разных портах
- Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
- HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

файл с настройками 
[haproxy.cfg](files/haproxy2.cfg)

балансеровка с весами
<img src = "img/3.png" width = 100%>
<img src = "img/4.png" width = 100%>