## Выполнено ДЗ №23

 - Основное ДЗ

## В процессе сделано:

 - Выполнил установку Prometheus с помощью Helm
 - Рассмотрели готовый набор targets для сбора метрик + включили сбор метрик с помощью node_exporter
 - Выполнил установку Grafana с помощью Helm
 - Произвел настройку Prometheus и Grafana для мониторинга k8s + добавил дашборды
 - Выполнил установку Kibana и произвел настройку EFK для сбора логов 

## Как проверить работоспособность:
По ссылке:
```
https://travis-ci.com/otus-devops-2019-05/azarkinivan_microservices
```
## PR checklist
Выставил label - Kubernetes и kubernetes-5


## Выполнено ДЗ №22

 - Основное ДЗ

## В процессе сделано:

 - Установили и ознакомились с возможностями Helm 
 - Разработали Chart-ы для компонентов: ui, post, comment 
 - Наполнили Chart-ы шаблонами манифестов Kubernetes
 - Установили плагин tiller и рассмотрели его работу
 - Подготовили GKE кластер для Gitlab. Установили Gitlab
 - Создали проекты и настроили ci/cd конвеер

## Как проверить работоспособность:
По ссылке:
```
https://travis-ci.com/otus-devops-2019-05/azarkinivan_microservices
```
## PR checklist
Выставил label - Kubernetes и kubernetes-4



## Выполнено ДЗ №21

 - Основное ДЗ

## В процессе сделано:

 - Произвели настройку и более подробно рассмотрели работу ClusterIP, NodePort и LoadBalancer
 - Настроили Ingress правила внутри кластера
 - Добавили Secrets в кластер + Ingress правило для приема https трафика
 - Настроили сетевые ограничения между узлами приложения с помощью Network Policy
 - Разобрались с вопросом хранения данных. Подключили хранилища к Pod-ам
 - Ознакомились и настроили динамическое выделение Volume 

## Как запустить проект:
```
kubectl apply -f <filename>
```
## Как проверить работоспособность:
По ссылке:
```
https://travis-ci.com/otus-devops-2019-05/azarkinivan_microservices
```
## PR checklist
Выставил label - Kubernetes и kubernetes-3


## Выполнено ДЗ №20

 - Основное ДЗ

## В процессе сделано:

 - Развернул локальное окружение для работы с Kubernetes: kubectl, minikube
 - Произвел настройку модулей приложения: comment, post, mongodb + объекты Services
 - Ознакомился с minikube
 - Развернул Kubernetes в GKE
 - Запустил приложение в Kubernetes

## Как запустить проект:
```
kubectl apply -n dev -f <filename>
```
## Как проверить работоспособность:
По ссылке:
```
https://travis-ci.com/otus-devops-2019-05/azarkinivan_microservices
```
## PR checklist
Выставил label - Kubernetes и kubernetes-2


## Выполнено ДЗ №19

 - Основное ДЗ

## В процессе сделано:

 - Произвел ручную конфигурацию kubernetes по THW

## Как запустить проект:
```
kubectl apply -f <filename>
```
## Как проверить работоспособность:
По ссылке:
```
https://travis-ci.com/otus-devops-2019-05/azarkinivan_microservices
```
## PR checklist
Выставил label - Kubernetes и kubernetes-1


## Выполнено ДЗ №18

 - Основное ДЗ

## В процессе сделано:

 - Пересобрали образы приложений
 - Подготовили окружение с помощью docker-machine
 - Настроили и протестировали Fluentd и стек EFK 
 - Произвели сбор структурированных логов 
 - Сконфигурировали Kibana согласно слайдам + фильтры 
 - Произвели  парсинг неструктурированных логов 
 - Внедрили Zipkin и рассмотрели распределенный трейсинг запросов

## Как запустить проект:
```
docker-compose up -d
docker-compose -f docker-compose-logging.yml up -d
```
## Как проверить работоспособность:
По ссылке:
```
https://travis-ci.com/otus-devops-2019-05/azarkinivan_microservices
```
## PR checklist
Выставил label - logging-1 и Logging



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

