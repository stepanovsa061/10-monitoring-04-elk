# # Домашнее задание к занятию 14 «Средство визуализации Grafana»

# Обязательные задания
# Задание 1
Вам необходимо поднять в докере и связать между собой:
1) elasticsearch (hot и warm ноды);
2) logstash;
3) kibana;
4) filebeat.
Logstash следует сконфигурировать для приёма по tcp json-сообщений.

Filebeat следует сконфигурировать для отправки логов docker вашей системы в logstash.

В директории help находится манифест docker-compose и конфигурации filebeat/logstash для быстрого выполнения этого задания.

# Ответ 1

Скриншот docker ps:

![alt text](https://github.com/stepanovsa061/10-monitoring-04-elk/blob/main/1%20docker.PNG)

Welcome:

![alt text](https://github.com/stepanovsa061/10-monitoring-04-elk/blob/main/1.1.PNG)



# Задание 2
Перейдите в меню создания index-patterns в kibana и создайте несколько index-patterns из имеющихся.

Перейдите в меню просмотра логов в kibana (Discover) и самостоятельно изучите, как отображаются логи и как производить поиск по логам.

В манифесте директории help также приведенно dummy-приложение, которое генерирует рандомные события в stdout-контейнера. Эти логи должны порождать индекс logstash-* в elasticsearch. Если этого индекса нет — воспользуйтесь советами и источниками из раздела «Дополнительные ссылки» этого задания.

# Ответ 2

![alt text](https://github.com/stepanovsa061/10-monitoring-04-elk/blob/main/2%20discover.PNG)

Логи из моего приложение отображающиеся в Kibana:

![alt text](https://github.com/stepanovsa061/10-monitoring-04-elk/blob/main/2%20index.PNG)
