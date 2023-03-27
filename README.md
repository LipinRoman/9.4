# Домашнее задание к занятию 9.4 «Система мониторинга Prometheus» - Липин Роман

Задание 1

Установите Prometheus.
Процесс выполнения

    Выполняя задание, сверяйтесь с процессом, отражённым в записи лекции
    Создайте пользователя prometheus
    Скачайте prometheus и в соответствии с лекцией разместите файлы в целевые директории
    Создайте сервис как показано на уроке
    Проверьте что prometheus запускается, останавливается, перезапускается и отображает статус с помощью systemctl

Требования к результату

    Прикрепите к файлу README.md скриншот systemctl status prometheus, где будет написано: prometheus.service — Prometheus Service Netology Lesson 9.4 — [Ваши ФИО]

![94-01](https://github.com/LipinRoman/9.4/blob/main/img/94-01.png)

Задание 2

Установите Node Exporter.
Процесс выполнения

    Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
    Скачайте node exporter приведённый в презентации и в соответствии с лекцией разместите файлы в целевые директории
    Создайте сервис для как показано на уроке
    Проверьте что node exporter запускается, останавливается, перезапускается и отображает статус с помощью systemctl

Требования к результату

    Прикрепите к файлу README.md скриншот systemctl status node-exporter, где будет написано: node-exporter.service — Node Exporter Netology Lesson 9.4 — [Ваши ФИО]

![94-02](https://github.com/LipinRoman/9.4/blob/main/img/94-02.png)

Задание 3

Подключите Node Exporter к серверу Prometheus.
Процесс выполнения

    Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
    Отредактируйте prometheus.yaml, добавив в массив таргетов установленный в задании 2 node exporter
    Перезапустите prometheus
    Проверьте что он запустился

Требования к результату

    Прикрепите к файлу README.md скриншот конфигурации из интерфейса Prometheus вкладки Status > Configuration
    Прикрепите к файлу README.md скриншот из интерфейса Prometheus вкладки Status > Targets, чтобы было видно минимум два эндпоинта

![94-03](https://github.com/LipinRoman/9.4/blob/main/img/94-03.png)
![94-04](https://github.com/LipinRoman/9.4/blob/main/img/94-04.png)

Дополнительные задания со звёздочкой*

Эти задания дополнительные. Их можно не выполнять. Это не повлияет на зачёт. Вы можете их выполнить, если хотите глубже разобраться в материале.
Задание 4*

Установите Grafana.
Требования к результату

    Прикрепите к файлу README.md скриншот левого нижнего угла интерфейса, чтобы при наведении на иконку пользователя были видны ваши ФИО

Задание 5*

Интегрируйте Grafana и Prometheus.
Требования к результату

    Прикрепите к файлу README.md скриншот дашборда (ID:11074) с поступающими туда данными из Node Exporter

Критерии оценки

    Выполнено минимум 3 обязательных задания
    Прикреплены требуемые скриншоты
    Задание оформлено в шаблоне с решением и опубликовано на GitHub
