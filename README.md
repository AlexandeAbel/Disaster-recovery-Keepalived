# Disaster-recovery-Keepalived

# Задание 1
**Дана схема для Cisco Packet Tracer, рассматриваемая в лекции.**

**На данной схеме уже настроено отслеживание интерфейсов маршрутизаторов Gi0/1 (для нулевой группы)**

**Необходимо аналогично настроить отслеживание состояния интерфейсов Gi0/0 (для первой группы).**

**Для проверки корректности настройки, разорвите один из кабелей между одним из маршрутизаторов и Switch0 и запустите ping между PC0 и Server0.**

## Router-1
![Router-1](https://github.com/AlexandeAbel/Disaster-recovery-Keepalived/blob/main/img/1.1.jpeg)

## Router-2
![Router-2](https://github.com/AlexandeAbel/Disaster-recovery-Keepalived/blob/main/img/1.2.jpeg)

# Задание 2
**Запустите две виртуальные машины Linux, установите и настройте сервис Keepalived как в лекции, используя пример конфигурационного файла.**

**Настройте любой веб-сервер (например, nginx или simple python server) на двух виртуальных машинах**

**Напишите Bash-скрипт, который будет проверять доступность порта данного веб-сервера и существование файла index.html в root-директории данного веб-сервера.**

![Check](https://github.com/AlexandeAbel/Disaster-recovery-Keepalived/blob/main/img/2.1.jpeg)

**Настройте Keepalived так, чтобы он запускал данный скрипт каждые 3 секунды и переносил виртуальный IP на другой сервер, если bash-скрипт завершался с кодом, отличным от нуля (то есть порт веб-сервера был недоступен или отсутствовал** **index.html). Используйте для этого секцию vrrp_script**

![Check](https://github.com/AlexandeAbel/Disaster-recovery-Keepalived/blob/main/img/2.2.jpeg)

**На проверку отправьте получившейся bash-скрипт и конфигурационный файл keepalived, а также скриншот с демонстрацией переезда плавающего ip на другой сервер в случае недоступности порта или файла index.html**

![Check](https://github.com/AlexandeAbel/Disaster-recovery-Keepalived/blob/main/img/2.3.jpeg)

![Check](https://github.com/AlexandeAbel/Disaster-recovery-Keepalived/blob/main/img/2.4.jpeg)

![Check](https://github.com/AlexandeAbel/Disaster-recovery-Keepalived/blob/main/img/2.5.jpeg)

