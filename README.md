![gophish logo](https://raw.github.com/gophish/gophish/master/static/images/gophish_purple.png)

Gophish
=======

Het project is gebaseerd op [Gophish v0.12.1]
(https://github.com/gophish/gophish/releases/tag/v0.12.1)


### Install



De container-image is gehost op [Dockerhub](https://hub.docker.com/layers/lvangestel/gophish/finalconcept/images/sha256-e4931b3c06c74322d9725b30dbfcd33ceeaa87e0271f8615af582c63bdd8ba15?context=explore)

Dit is het laatste concept dat is opgeleverd tijdens de stageperiode. In deze image zijn de concepten van [Evilginx Phishing Infra Setup] (https://github.com/An0nUD4Y/Evilginx-Phishing-Infra-Setup) geïtegreerd om Gophish moeilijker herkenbaar te maken.

Het adminpaneel is verplaatst naar poort 60002.
De phishingserver draait nu op poort 8080.

Om deze container in een omgeving te installeren, hoef je alleen maar naar de repository te verwijzen.


### Setup

Eenmaal de container is gedeployed, is het wachtwoord van het adminpaneel terug te vinden in de logs. Dit ziet er zo uit:
time="2020-07-29T01:24:08Z" level=info msg="Please login with the username admin and the password 4304d5255378177d"


### Docker container bouwen en pushen

De container moet gebouwd worden vanuit de projectmap met het volgende commando:
docker build -t [dockerhub gebruikersnaam]/[image-naam]:[tag] .

Log vervolgens in met een Docker Hub account met het commando: docker login

Eenmaal gebouwd en ingelogd, is het mogelijk om de image te pushen naar dockerhub met het volgende commando:
docker push [dockerhub gebruikersnaam]/[image-naam]:[tag]

### Documentation

Documentation can be found on our [site](http://getgophish.com/documentation). Find something missing? Let us know by filing an issue!
