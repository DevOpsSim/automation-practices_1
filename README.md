# automation-practices_1

1.) Установка docker ubuntu 20.04

-  обновляем репозиторий:
    
  $ sudo apt update

-  затем установим несколько необходимых пакетов, которые позволяют apt использовать пакеты через HTTPS:
    
  $ apt install docker.io make dpkg-repack sudo apt install apt-transport-https ca-certificates curl software-properties-common

-  добавляем ключ GPG для официального репозитория Docker в нашу систему: 
    
  $ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

-  добавляем репозиторий Docker в источники APT: 
    
  $ sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"

- потом обновляем базу данных пакетов и добавляем в нее пакеты Docker из недавно добавленного репозитория: 
    
  $ sudo apt update

-  непосредственно установка: 
    
  $ docker sudo apt install docker-ce

-  проверяем что docker запустился:
    
  $ sudo systemctl status docker

2.) Создание докер контейнера
 
- созданим контейнер с именем Project_1:
    
  $ sudo docker build -t Project_1

 - запускаем docker-контейнер: 
    
  $ sudo docker run Project_1

4.) Генерируем rsa-ключи:
    
  $ ssh-keygen -t rsa

5.)
