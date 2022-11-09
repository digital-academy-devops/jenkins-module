# Модуль 4.1 Jenkins

Целью данного модуля является знакомство с [Jenkins](https://www.jenkins.io/). 

В ходе выполнения этого практического задания, мы рассмотрим:
- локальное развертывание Jenkins средствами Docker;
- базовое конфигурирование;
- добавление агентов;
- применение принциов IaaC к Jenkins;
- построение CI конвеера для тестового приложения;

## Предварительные требования

Предполагается, что Вы:

1. Установили `docker` и `docker-compose`. 
1. Выполнили задания по модулям [Docker](https://github.com/digital-academy-devops/docker-module) и [Docker-compose](https://github.com/digital-academy-devops/docker-compose-module) и будете использовать результаты в качестве приложения для реализации CI конвеера.


## Задание
1. При помощи docker-compose, разверните экземпляр Jenkins с использованием [официального образа](https://www.google.com/search?q=jenkins+official+docker+image).
   Экземпляр должен:
   - быть доступен по (http://localhost:8080/)
   - иметь постоянное хранилище.
1. Добавьте контейнер JNLP агента из [официального образа](https://www.google.com/search?q=jenkins+jnlp+slave+official+docker+image) и подключите его к мастеру Jenkins.
   - Агент должен иметь возможность [запускать команды docker](https://www.google.com/search?q=how+to+run+docker+inside+docker+container). Выберите наиболее простой способ реализации данного требования. 
1. Сконфигурируйте возможность [динамического запуска агентов внутри контейнеров](https://www.google.com/search?q=jenkins+use+containers+as+agents). 
1. [Опишите конфигурацию экземпляра кодом](https://www.google.com/search?q=jenkins+how+to+store+configuration+as+code).
1. Создайте [описанный кодом pipeline](https://www.google.com/search?q=jenkins+how+to+code+app+pipeline) для сборки тестового приложения.



