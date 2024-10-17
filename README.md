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
<summary><strong><font size="+1">Introduction & mise en contexte</font></strong></summary>

> Dans le monde actuel, il est nécessaire de pouvoir se prémunir des dangers et des intrusions de la manière la plus efficace possible.<br>
Ce projet nous a permit de voir la vulnérabilité d'un réseau et nous a appris à comment se protéger et détecter les intrusions.
 
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
Pour plus de détail, allez au chapitre **Installation des postes clients** de la documentation pour les administrateurs.

### Machine serveur
Security Onion dispose de son propre système d'exploitation.<br>
Il sera de type Linux CentOS.

</details>

<HR>

<details>
<summary><strong><font size="+1">Les difficultés rencontrées</font></strong></summary>
<br>

### Difficultés personnelle
Ci-dessous, une liste des difficultés rencontrées :
1. Utilisation du Markdown pour structurer la documentation et l'implémenter.
2. Appliquer la méthode agile SCRUM.
3. En raison de la complexité du projet et du fait d'être une équipe de deux, nous nous sommes concentrés sur la recherche et documentation. De ce fait, nous n'avons pas pu procéder à l'ensemble des tests techniques et approfondis pour une utilisation intégrale du logiciel Security Onion.

### Difficultés concernant Security Onion
1. En raison de la complexité du logiciel et du fait qu'il propose un large spectre d'outils, la machine où sera installé Security Onion devra être assez puissante.  
   Cela rajoute une problématique de coût. Or le client a choisi Security Onion du fait, le logiciel en lui même, qu'il est peu coûteux.
2. Pour poursuire sur le large spectre d'outils que propose Security Onion, sans documentation ou tutoriel, il est vite facile de s'y perdre.

</details>

<HR>

<details>
<summary><strong><font size="+1">Les solutions trouvées</font></strong></summary>
<br>

Dans le chapitres **Les difficultés rencontrées**, nous avons parlé de la difficulté à trouver de la documentation sur Security Onion.<br>
En poursuivant nos recherches, nous avons trouvés un [dépôt](https://github.com/Security-Onion-Solutions/securityonion/tree/2.4/main) GitHub de Security Onion avec toute la documentation officielle.<br>
Cela nous a permis d'approfondir notre compréhension du sujet et d'améliorer notre présentation.

</details>

<HR>

<details>
<summary><strong><font size="+1">Les améliorations possibles</font></strong></summary>

### La méthode agile Scrum
Pour mettre en œuvre la méthode agile Scrum de manière efficace, l'utilisation d'outils spécialisés tel que Trello pourrait optimiser la gestion des tâches et la coordination au sein de l'équipe.<br>
Cela facilite le suivi de l'avancement du projet et favorise une collaboration harmonieuse.<br<

### Suivi des mises à jour de la documentation officielle :
 
  Avec les changements rapides qui caractérisent le domaine de l’informatique, il est primordial de rester 
  continuellement à jour sur les dernières actualisations logicielles et la documentation officielle de chaque 
  outil (comme Zeek, Suricata, Kibana, ElasticSearch). Cela permettra d'intégrer rapidement les nouvelles 
  fonctionnalités pour améliorer l'expérience utilisateur
  


</details>
<HR>
