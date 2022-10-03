# Первое задание
Сборка контейнера с виртуалкой
```shell
docker build -t custom-server .
```

Запуск контейнера
```shell
docker run -it --rm -p 80:80 -p 22:22  custom-server 
```

Проверка доступа
```shell
ssh test@localhost
```

Установите ansible на macos
```shell
brew install ansible@2.9
```

Запуск плейбука
```shell
ansible-playbook -i inventory ./playbook.yml -K
```
Проверка сайта
```shell
ansible-playbook -i inventory ./playbook.yml -K --tags "check"
```

