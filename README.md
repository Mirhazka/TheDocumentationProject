<div align="center"><h1>Plateforme de surveillance de sécurité </h1></div>
<div align="center"><h2>Documentation générale</h2></div>
<br>
<br>
<br>

<details>
<summary><strong><font size="+1">Présentation du projet & des objectifs</font></strong></summary>

### _Présentation_
Qu'est-ce que la surveillance de la sécurité du réseau ?<br>
Cela consiste à inspecter le trafic réseau et l'infrastructure informatique à la recherche de signes de problèmes de sécurité. Ces signes peuvent fournir aux équipes informatiques des informations précieuses sur la posture de cybersécurité de l'organisation.<br>
  * **_Exemple_** :  
    Les équipes de sécurité peuvent remarquer des modifications inhabituelles apportées aux politiques de contrôle d'accès. Cela peut entraîner des flux de trafic inattendus entre les systèmes sur site et les applications Web non reconnues. Cela peut permettre d'alerter rapidement en cas de cyberattaque active, ce qui donne aux équipes de sécurité suffisamment de temps pour mener des efforts de correction et empêcher la perte de données.

### _Objectif principal_
Notre objectif principal est d'installer une plateforme de surveillance de sécurité réseau.<br>
A la volonté du client, cette plateforme sera basé sur le logiciel Security Onion.<br>

### _Objectif secondaire_
Notre objectif secondaire est de mettre en place des règles de détection intrusion sur le réseau du client.

### _Les livrables_
Ce projet est livré avec trois documentations :
<dl>
  <dt>README - Documentation Générale</dt>
  <dd>Ce document est une présentation générale de notre projet.</dd>
  <dt>INSTALL - Documentation pour les administrateurs</dt>
  <dd>Ce document est une présentation pour les administrateurs qui devront installés les machines serveurs & clientes.<br>
  Il est livré avec un FAQ.</dd>
  <dt>USER_GUIDE - Documentation pour les utilisateurs</dt>
  <dd>Ce document est une présentation pour les utilisateurs qui décrira comment utiliser le système.<br>
  Il est livré avec un FAQ</dd>
</dl>

</details>

<HR>

<details>
<summary><strong><font size="+1">Présentation du logiciel</font></strong></summary>


 
</details>

<HR>

<details>
<summary><strong><font size="+1">Membres du groupe du projet</font></strong></summary>

#### Le groupe est composé de :
  * Sybill GRIBONVAL
  * Hamza MALKI

##### Scrum Master
Un Scrum Master ficilite l'application du sprint et de ses tâches.

##### Product Owner
Un Product Owner est le porteur de la vision du client et fait en sorte que sa vision soit respecté.

##### Semaine 1

Membre | Rôles | Tâches  
--- | --- | ---
Sybill | Scrum Master | Recherche sur les plateformes de surveillance de sécurité. <br> Création des fichiers Markdown sur GitHub.
Hamza | Product Owner | Recherche sur le logiciel Security Onion. <br> Recherche sur le serveur Linux CentOS pour Security Onion.
  
##### Semaine 2

Membre | Rôles | Tâches  
--- | --- | ---
Sybill | Product Owner | Finaliser le dépôt GitHub. <br> Création de la présentation.
Hamza | Scrum Master | Recherche sur les règles de détection. <br> Installation de la machine virtuelle Security Onion.

</details>

<HR>

<details>
<summary><strong><font size="+1">Nos choix techniques</font></strong></summary>

### Machine cliente
Le client peut être soit sous Ubuntu soit sous Windows avec la configuration suivante :
  * Nom
  * Compte utilisateur
  * Mot de passe
  * Adresse IP Fixe
Le client a souhaité d'avoir ses machines clientes sous Ubuntu.
Pour plus de détail, allez au chapitre **Installation des postes clients** de la documentation pour les administrateurs.

### Machine serveur
Security Onion dispose de son propre système d'exploitation qui basé sur Linux CentOS.  
Lors de l'installation de Security Onion sur une machine virtuelle, nous choisirons l'option *Import* qui est la plus basique et la plus simple version de Security Onion à utiliser.  
Cependant, pour une utilisation approfondie, nous conseillons de prendre l'option *StandAlone* qui sera la plus simple à utiliser mais complète au niveaux de la configuration pour une production.  
Pour plus de détail, allez au chapitre **Configuration & installation** de la documentation pour les administrateurs.

</details>

<HR>

<details>
<summary><strong><font size="+1">Les difficultés rencontrées</font></strong></summary>
<br>

Ci-dessous, une liste des difficultés que nous avons rencontrés lors de ce projet :
  * Utilisation du Markdown pour structurer la documentation et l'implémenter
  * Appliquer la méthode agile SCRUM
  * En raison de la complexité du projet et du fait d'être une équipe de deux, nous nous sommes concentrés sur la recherche et documentation.  
    De ce fait, nous n'avons pas pu procéder à l'ensemble des tests techniques et approfondis pour une utilisation intégrale du logiciel Security Onion.
  * Du fait de la complexité du logiciel et qu'il propose un large spectre d'outils, la machine où sera installé Security Onion devra être assez puissante.
    En conséquence, il faudra avoir un budget financier pour cette machine. Cependant le client a choisi Security Onion car il est OpenSource & **gratuit**.
  * Pour poursuivre sur le large spectre d'outils que propose Security Onion, sans documentation ou tutoriel, il est vite facile de se perdre entre les outils proposés.

</details>

<HR>

<details>
<summary><strong><font size="+1">Les solutions trouvées</font></strong></summary>
<br>

### La méthode agile Scrum
Pour nous aider à appliquer la méthode agile Scrum, nous avons utilisés l'outils Trello qui nous a permit d'optimiser la gestion des tâches et de la coordination au sein de l'équipe.  
Cela facilite le suivi de l'avancement du projet et favorise une collaboration harmonieuse de l'équipe.
<br>

### Documentation Security Onion
Dans le chapitres **Les difficultés rencontrées**, nous avons parlé de la complexité de Security Onion et de son large spectre d'outils qu'il peut proposer.<br>
En poursuivant nos recherches, nous avons trouvés un [dépôt](https://github.com/Security-Onion-Solutions/securityonion/tree/2.4/main) GitHub de Security Onion avec toute la documentation officielle.<br>
Cela nous a permis d'approfondir notre compréhension du sujet et d'améliorer notre présentation.

</details>

<HR>

<details>
<summary><strong><font size="+1">Les améliorations possibles</font></strong></summary>
<br>


### Suivi des mises à jour de la documentation officielle :
 
  Avec les changements rapides qui caractérisent le domaine de l’informatique, il est primordial de rester 
  continuellement à jour sur les dernières actualisations logicielles et la documentation officielle de chaque 
  outil (comme Zeek, Suricata, Kibana, ElasticSearch). Cela permettra d'intégrer rapidement les nouvelles 
  fonctionnalités pour améliorer l'expérience utilisateur
  


</details>
<HR>
