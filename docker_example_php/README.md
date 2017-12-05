# Docker Template

Sie können Docker nativ auf Ihrem System nutzen oder innerhalb einer virtuellen Maschine. Die virtuelle Maschine können Sie selbst erstellen oder die beiliegende Vagrant-Datei nutzen. Damit wird eine Ubuntu-VM mit Docker aufgesetzt.

## Benutzung von Vagrant

Sie können die VM mit folgendem Befehl starten:
```
vagrant up
```

Anschließend können Sie sich per SSH auf die Maschine verbinden oder die Maschine als Dockerhost nutzen und über Ihre native Docker Installation ansteuern. Für die SSH Verbindung bietet Vagrant direkt einen Befehl:
```
vagrant ssh
```

Um die VM als Dockerhost zu setzen, führen sie folgendes aus:
```
export DOCKER_HOST=192.168.56.10:2375
```

## Benutzung von Docker

Die Docker Container können Sie mit folgendem Befehl starten:
```
docker-compose up
```
Dies behält die Container im Vordergrund und diese können mit Ctrl+C wieder gestoppt werden. Sie können die Container mit dem `-d` Flag auch im Detached Mode starten, sodass diese im Hintergrund laufen. Um die Containter zu stoppen führen Sie folgendes aus:
```
docker-compose stop
```

## Links
- https://docs.docker.com/get-started/
- https://hub.docker.com/
- https://www.vagrantup.com/
- https://app.vagrantup.com/boxes/search
