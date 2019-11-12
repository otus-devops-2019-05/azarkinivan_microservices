## Выполнено ДЗ №17

 - Основное ДЗ

## В процессе сделано:

 - Развернут cAdvisor для мониторинга контейнеров
 - Разделены docker-compose конфигурации на app и monitoring
 - Развернута Grafana, построены дашборды
 - Произведен мониторинг работы приложений и бизнес-метрик
 - Развернут Alertmanager, настроен алертинг и  интеграция со Slacл
 - Запушили полученные образы в docker hub

## Как запустить проект:
```
docker-compose up -d
docker-compose -f docker-compose-monitoring.yml up -d
```
## Как проверить работоспособность:
По ссылке:
```
https://travis-ci.com/otus-devops-2019-05/azarkinivan_microservices
```
## Образы
```
https://cloud.docker.com/u/azarkinivan/repository/list
```

## PR checklist
Выставил label - monitoring и monitoring-2



## Выполнено ДЗ №16

 - Основное ДЗ

## В процессе сделано:

 - Развернута ВМ с использованием docker-machine
 - Запустили и ознакомились с Prometheus. Создали образ
 - Запустили микросервисы. Создали образы
 - Провели корректировку docker-compose под Prometheus. Добавили aliases для DB
 - Поэкспериментировали с мониторингом
 - Развернули node_exporter. Собрали метрики.
 - Запушили полученные образы в docker hub

## Как запустить проект:
```
docker-compose up -d
```
## Как проверить работоспособность:
По ссылке:
```
https://travis-ci.com/otus-devops-2019-05/azarkinivan_microservices
```
## Образы
```
https://cloud.docker.com/u/azarkinivan/repository/list
```

## PR checklist
Выставил label - monitoring и monitoring-1


## Выполнено ДЗ №15

 - Основное ДЗ

## В процессе сделано:

 - Развернута ВМ с использованием docker-machine
 - Установили GitLab CI с помощью docker-compose
 - Создана группа, проект и pipeline
 - Зарегистрирован и запущен Runner и pipeline
 - Добавлено тестирование для reddit
 - Описали окружения: dev, stage, production
 - Добавили ручной запуск для окружений: stage и production + ограничение на запуск явно заданных версий
 - Сконфигурировали динамическое определение окружений 

## Как запустить проект:
```
docker-compose up -d
```
## Как проверить работоспособность:
По ссылке:
```
https://travis-ci.com/otus-devops-2019-05/azarkinivan_microservices
```
## PR checklist
Выставил label - GitlabCI и gitlab-ci-1


## Выполнено ДЗ №14

 - Основное ДЗ

## В процессе сделано:

- Рассмотрели разновидности  сетей в Docker: none,host, bridge
- Установили docker-compose
- Описали контейнеры и запустили модули приложения reddit с помощью docker-compose
- Параметризовали модули и вынесли параметры в отдельный файл
- Базовое имя проекта обраузется из названия папки + название сервиса

## Как запустить проект:
```
docker network create reddit --driver bridge
./docker-compose up -d
```
## Как проверить работоспособность:
По ссылке:
```
https://travis-ci.com/otus-devops-2019-05/azarkinivan_microservices
```
## PR checklist
Выставил label - docker и docker-4

## Выполнено ДЗ №13

 - Основное ДЗ

## В процессе сделано:

 - Запущен ранее созданный docker-host 
 - Подготовили отдельные части приложения 
 - Описали Dockerfile для каждого сервиса. Скорректировали Dockerfile для сервиса post-py 
 - Создали образы, запустили контейнеры сервисов и объединили в сеть
 - Создали volume для хранения данных и пересобрали контейнер с БД

## Как запустить проект:
```
docker run 
```
## Как проверить работоспособность:
По ссылке:
```
https://travis-ci.com/otus-devops-2019-05/azarkinivan_microservices
```
## PR checklist
Выставил label - docker-3

## Выполнено ДЗ №12

 - Основное ДЗ

## В процессе сделано:

 - Установлен Docker
 - Поэкспериментировали с командами docker
 - Создан и настроен новый проект в GCP, активирован GCE API
 - Установлен docker-machine. Создан хост в GCP
 - В контейнере развернуто приложение + DB. Создан образ
 - Регистрация на docker hub. Экспорт собственного образа

## Как запустить проект:
```
docker build -t reddit:latest .
```
## Как проверить работоспособность:
По ссылке:
```
https://travis-ci.com/otus-devops-2019-05/azarkinivan_microservices
```
## PR checklist
Выставил label - docker и docker-2

