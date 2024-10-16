<div align="center"><h1>Plateforme de surveillance de sécurité</h1></div>
<div align="center"><h2>Documentation pour les administrateurs</h2></div>
<br> 
<br>
<br>

<details>
<summary><strong><font size="+1">Pré-requis technique</font></strong></summary>

### Généralités
Disposer de :
  * Une machine serveur sous un OS Linux serveur CentOS où se trouvera Security Onion.
  * Machine clientes sous n'importe quel OS.
    Nous avons fait le choix de partir sous deux machines clientes avec deux OS différents.
    Cela nous permettra de mieux visualiser les différences entre les OS suivant ce que souhaite le client.

### Security Onion
Cliquez [ici](https://docs.securityonion.net/en/2.4/hardware.html), pour voir les spécificités requises pour une machine Security Onion. <br>
Cette documentation indiquera :
  * Configuration matérielle requise
  * Architecture du processeur
  * Spécificité minimum pour la RAM, la DATA, le nombre de cœur de CPU, ...
  * Et bien d'autres informations supplémentaires.

</details>
<HR> 

<details>
<summary><strong><font size="+1">Installation du poste client</font></strong></summary>
<br>

Le poste client peut être sur n'importe quel type d'OS, qu'il soit sous Linux ou Windows.<br>
Ci-dessous, vous verrez les différentes configuration sous Ubuntu puis sous Windows.
<br>
<img src="https://raw.githubusercontent.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/refs/heads/main/Images/1175077.webp" width="10%"/>

  * Nom : **CLILIN01**
  * Compte utilisateur : **wilder**
  * Mot de passe : **Azerty1***
  * Adresse IP fixe : **172.16.10.20/24**
<br>
<img src="https://github.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/blob/main/Images/Windows_10_Logo.svg.png" width="20%"/>

  * Nom : **CLIWIN01**
  * Compte utilisateur : **wilder**
  * Mot de passe : **Azerty1***
  * Adresse IP fixe : **172.16.10.21/24**


</details>
<HR>

<details>
<summary><strong><font size="+1">Installation du poste serveur Linux CentOS de Security Onion</font></strong></summary>

### Security Onion
[Security Onion](https://securityonionsolutions.com/) est un outils pour détecter, surveiller et réagir immédiatement aux incidents de sécurité sur votre réseau.

Voici le [lien installation](https://docs.securityonion.net/en/2.4/installation.html) & ci-dessous, vous trouverez les différentes étapes d'installations du logiciel qui a son propre OS : Linux Serveur CentOS.
<div align="center"><img src="https://raw.githubusercontent.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/refs/heads/main/Images/01_grub.webp" width="50%"/></div>
<br>

1. Téléchargez et vérifiez l'image ISO avec son image [ISO](https://docs.securityonion.net/en/2.4/download.html#download)
2. Démarrez l'ISO sur une machine qui répond aux spécifications matérielles minimales.
3. Une fois la machine lancé, suivre les étapes d'installation du logiciel qui est directif.
4. Vous pourriez avoir à retirer l'image ISO ou à ajuster les paramètres de démarrage de votre machine pour pouvoir démarrer avec le nouvel OS que vous avez installé.
5. Après cela, il suffit de se connecter avec le nom d'utilisateur et le mot de passe prédéfinis dans le cadre du processus d'installation.
6. L'installation de Security Onion démarre automatiquement.  
   Dans le cas où vous seriez amené à quitter l'installation, il vous suffit juste de vous déconnecter de votre compte, de vous reconnecter et l'installation démarrera d'elle-même.
   Si cela ne fonctionne pas, vous pouvez l'exécuter manuellement comme suit dans un terminal de commande :
   > sudo SecurityOnion/setup/so-setup iso

</details>

<HR>

<details>
<summary><strong><font size="+1">Configuration & Installation du système</font></strong></summary>

### Configuration
Security Onion est conçu pour de nombreux cas d'utilisation différentes.<br>
<div align="center"><img src="https://github.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/blob/main/Images/grafik-18.png" width="50%"/></div>
<br>

Voici le [lien de configuration](https://docs.securityonion.net/en/2.4/configuration.html#configuration) et ci-dessous vous trouverez quelques exemples de configuration :
  * Import
    > L'une des façons les plus simples de démarrer avec Security Onion consiste à l'utiliser pour analyser de manière médico- légale les fichiers *pcap* et les fichiers journaux.
    > Sélectionnnez simplement l'**IMPORT** option, suivez les instructions, puis importez les fichiers pcap ou les journaux d'évènements à l'aide de la page **Grid**. <br>
<div align="center"><h3>PCAP</h3></div>
<div align="center"><img src="https://github.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/blob/main/Images/62_pcap.png" width="75%"/></div>
<div align="center"><h3>GRID</h3></div>
<div align="center"><img src="https://github.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/blob/main/Images/75_grid.png" width="75%"/></div>
    
  * Evaluation
    > Le mode *Evaluation* est idéal pour les salles de classe ou les petits laboratoires. Le mode d'éaluation n'est **pas** conçu pour une utilisation en production. Choisissez l'option **EVAL**, suivez les instructions puis passez au chapitre **Installation**.
    
  * Production Server - Standalone
    > Le mode *Standalone* est similaire au mode *Evaluation* dans la mesure où il nécessite qu'une seule boîte, mais le mode *Standalone* est plus adapté à une utilisation en production. Choisissez l'option **STANDALONE**, suivez les instructions puis passez au chapitre **Installation**.
<br>

### Installation
Suivant la configuration choisi, il faut maintenant poursuivre sur l'installation.
1. Ajuster les règles de pare-feu
2. Vérifier que tous les services sont fonctionnels grâce à la page **Grid**  
3. Il est possible de configurer une connection SSH si l'utilisateur ne souhaite pas utiliser la console de Security Onion.
4. Allez dans *Administration* puis dans *Configuration* pour voir certaines options que vous souhaiteriez peut-être configurer.
<div align="center"><img src="https://github.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/blob/main/Images/87_config.png" width="75%"/></div>

5. Toujours sur la page *Administration*, vous pouvez configurer votre serveur NTP si vous en avez un.
6. Les analystes peuvent se connecter au système avec leur console dédié de **Security Onion Desktop**.
7. Tout système IDS/NSM doit être réglé en fonction du réseau qu'il surveille. Cela permettra une meilleur *Détections d'intrusion*.
<br>

Voilà votre système configuré et installé. Vous pouvez dès maintenant allez sur les pages **Dashboards** & **Alerts** pour visualiser la sécurité de votre réseau!
<div align="center"><h3>Dashboard</h3></div>
<div align="center"><img src="https://github.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/blob/main/Images/53_dashboards.png" width="75%"/></div>
<div align="center"><h3>Alerts</h3></div>
<div align="center"><img src="https://github.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/blob/main/Images/50_alerts.png" width="75%"/></div>

<br>
</details>
<HR>

<details>
<summary><strong><font size="+1">La Foire Aux Questions !</font></strong></summary>
<br>

***Questions : Qu'est-ce qu'un PCAP ?***<br>
*Réponse*<br>
Un PCAP (*paquet de capture*) est une interface de programmation permettant de capturer les paquets transitant sur le réseau. Les versions récentes permettent également de transmettre des paquets sur la couche de liaison.<br>
<br>
***Questions : Qu'est-ce qu'un fichier de journaux ?***<br>
*Réponse*<br>
Les fichiers de journaux sont des fichiers générés par des logigiels et contenant des informations sur les opérations, les activités et les modèles d'utilisation d'une application, d'un serveur ou d'un système informatique.<br>
<br>
***Questions : Qu'est-ce qu'un serveur NTP?***<br>
*Réponse*<br>
NTP signifie : **N**etwork **T**ime **P**rotocol, parfois appelé protocolede synchronisation de réseau. C'est un protocole qui permet de synchroniser, via un réseau infomatique, l'horloge locale d'ordinateurs sur une référence d'heure.<br>
<br>
***Questions : Qu'est-ce qu'un système IDS/NSM?***<br>
*Réponse*<br>
IDS signifie : **I**ntrusion **D**etection **S**ystem, également appelé système de détection intrusion, il est chargé d'identifier les attaques et les techniques et est souvent déployé hors bande en mode écoute seule afin qu'il puisse analyser tout le trafic et générer des évènements d'intrusion à partir du trafic supect ou malveillant. <br>
NSM signifie : **N**etwork **S**ecurity **M**onitoring, également appelé gestion des système sen réseau est la gestion combinée des fonctions informatiques et des réseaux au sein d'une organisation.

</details>
<HR>
