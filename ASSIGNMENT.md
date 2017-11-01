Ansible Workshop 2017 Assignment
================================

### Leuk dat je meedoet met de workshop!
De challenges zijn opgedeeld in levels, te beginnen bij 1 en eindigend bij 4. Ieder level kan 1 of meerdere challenges bevatten. Hoe hoger het level, des te moeilijker de challenges zullen zijn. Aan het einde van de workshop verloten we een aantal gave prijzen onder de mensen die het verst zijn gekomen!

Je mag de challenges samen doen, mocht je bijvoorbeeld niet over een laptop beschikken. Mocht je vastlopen (of je computer ;-)), geef dan een seintje om hulp te krijgen. We zeggen je niets voor, maar helpen je graag op weg!

 1 tip geven we je alvast: [http://docs.ansible.com/ansible/latest/list_of_all_modules.html](http://docs.ansible.com/ansible/latest/list_of_all_modules.html)

### Achtergrond info:

Gefeliciteerd met je nieuwe baan! Als DevOps Engineer bij Klaut Solutions is het jouw taak om het beheer van de servers te moderniseren. De CTO heeft voor jou alvast 1 server neergezet en Ansible geïnstalleerd; Hiermee kun je de webserver configureren en klaarmaken voor de rebranding van Klaut. De login gegevens vind je hieronder:

Om te beginnen moeten we kijken of de webserver ‘Up & Running’  is. Met Ansible kun je naast playbooks ook ad-hoc commando’s uitvoeren, zoals het pingen van een server of het gebruiken van een module om 1 taak uit te voeren:

#### Level 1: Ad-Hoc commands:

Schrijf het commando dat je gebruikt hebt onder de challenge, dus niet het resultaat van je commando.

##### Challenge 1:
Test de connectiviteit met de webserver.

##### Challenge 2:
Gebruik de shell module om de uptime van web01 te weten te komen.

##### Challenge 3:
Gebruik de setup module om te zien welk intern IP adres de machine heeft.


#### Level 2: LAMP Installation Voor dit level heb je playbook.yml nodig

We hebben alvast een deel van het playbook ingevuld, maar als je het playbook probeert te draaien zul je zien dat je wat foutmeldingen krijgt. Er missen nog een aantal variabelen. Aan jou de taak om deze in te vullen en zo je LAMP installatie af te maken.

#### Level 3: Configuring the WordPress website

##### Challenge 3.1:
Maak een taak aan die een andere WordPress thema installeert.
[https://developer.wordpress.org/cli/commands/theme/](https://developer.wordpress.org/cli/commands/theme/)

##### Challenge 3.2:
Maak een taak aan die het externe IP adres van de webserver in een variabele opslaat.
[http://docs.ansible.com/ansible/latest/playbooks_conditionals.html#register-variables](http://docs.ansible.com/ansible/latest/playbooks_conditionals.html#register-variables)

##### Challenge 3.3:
Maak een taak aan die je externe IP post op de website.
[https://developer.wordpress.org/cli/commands/post/create/](https://developer.wordpress.org/cli/commands/post/create/)

#### Level 4: Configuring Backup jobs

##### Challenge 4.1:
Maak een taak aan die een directory creëert waar we backups naartoe kunnen kopieren.

##### Challenge 4.2:
Maak een taak aan die een backup maakt van de webroot (/var/www/html) naar de backup folder.

##### Challenge 4.3:
Maak een taak aan die een backup maakt van de database naar de backup folder
