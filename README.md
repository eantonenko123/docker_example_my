# docker_example_my
```shell
docker images (Команда показывает все образы Docker, которые расположены на жестком диске вашего сервера (или локально))
docker ps -a (отображает в терминале все запущенные контейнеры. А при добавлении опции -a в список попадают все контейнеры, созданные в системе)
docker pull ubuntu:18.04
docker build -t test_image:18.05 . ( -t, чтобы задать имя образа (test_image) и тегом 18.05)
docker rm -vf $(docker ps -a -q) (rm  —  удаляет один и более контейнеров)
docker stop $(docker ps -a -q) (останавливает все запущенные контейнеры)
docker rmi -f $(docker images -a -q) (rmi  —  удаляет один и более образов)
docker run -i -t test_image:18.05 /bin/bash
docker run test_image:18.05 (запускает контейнер, на основе указанного образа)
docker history test_image_my:18.05 (Отображает историю конкретного образа)
docker logs --follow my_container (эта команда используется для просмотра логов указанного контейнера. Можно использовать флаг --follow, чтобы следить за логами работающей программы:)
```
