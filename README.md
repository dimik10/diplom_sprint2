# Diplom_sprint1

Спринт 2

ЗАДАЧА

```
Исходники простого приложения можно взять здесь. Это простое приложение на Django с уже написанным Dockerfile. Приложение работает с PostgreSQL, в самом репозитории уже есть реализация docker-compose — её можно брать за референс при написании Helm-чарта.
Необходимо склонировать репозиторий выше к себе в Git и настроить пайплайн с этапом сборки образа и отправки его в любой docker registry. Для пайплайнов можно использовать GitLab, Jenkins или GitHub Actions — кому что нравится. Рекомендуем GitLab.


Описываем приложение в Helm-чарт.
Описываем приложение в виде конфигов в Helm-чарте. По сути, там только два контейнера — с базой и приложением, так что ничего сложного в этом нет. Стоит хранить данные в БД с помощью PVC в Kubernetes.


Описываем стадию деплоя в Helm.
Настраиваем деплой стадию пайплайна. Применяем Helm-чарт в наш кластер. Нужно сделать так, чтобы наше приложение разворачивалось после сборки в Kubernetes и было доступно по бесплатному домену или на IP-адресе с выбранным портом.

Для деплоя должен использоваться свежесобранный образ. По возможности нужно реализовать сборку из тегов в Git, где тег репозитория в Git будет равен тегу собираемого образа.
Например:
Чтобы создание такого тега запускало пайплайн на сборку образа c таким именем hub.docker.com/skillfactory/testapp:2.0.3.

```

Решение задачи:



Результаты выполнения запуска кода на кластере k8s:
