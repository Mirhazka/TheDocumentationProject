<div align="center"><h1>Plateforme de surveillance de sécurité</h1></div>
<div align="center"><h2>Guide de l'utilisateur</h2></div>
<br>
<br>
<br>

<details>
<summary><strong><font size="+1">Utilisation de base : Découverte des différents outils de Security Onion</font></strong></summary>
<br>
Danse ce chapitre, nous vous parlerons de différents outils vous permettant une meilleur utilisation de SecurityOnion.
<br>
   
Pour rappel, Security Onion est un ensemble d'outils de surveillance et de détection avec une suite d'action qui s'enchaîne et se complète.<br>
1. La surveillance du réseau avec l'outil **[Kibana](https://docs.securityonion.net/en/2.4/kibana.html)** et qui, en complément de Security Onion, permet de surveiller le réseau.
   > Connectez-vous à **Kibana** en utilisant le même nom d'utilisateur et le même mot de passe que ceux que vous utilisez pour Security Onion.  
<div align="center"><img src="https://raw.githubusercontent.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/refs/heads/main/Images/config-item-kibana.webp" width="75%"/></div>

2. La détection d'intrusion avec les outils **[Snort](https://www.snort.org/) / [Suricata](https://docs.securityonion.net/en/2.4/suricata.html) / [ElastAlert2](https://docs.securityonion.net/en/2.4/elastalert.html#elastalert) / [Strelka](https://docs.securityonion.net/en/2.4/strelka.html#strelka)** 
   > Ces outils sont des IDS, *Système de détection intrusion*, c'est un mécanisme déstiné à repérer des activités anormales ou suspectes sur la cible analysée (un réseau ou un hôte).
   > Pour **Snort**, ci-joint une [documentation](https://snort-org-site.s3.amazonaws.com/production/document_files/files/000/003/977/original/Snort_3_GA_on_CentOS_8_Stream.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAU7AK5ITMMOXGB2W5%2F20241017%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20241017T083802Z&X-Amz-Expires=172800&X-Amz-SignedHeaders=host&X-Amz-Signature=3df2f6787807c8e1dfd9864c51bfaeaf771bddc5e5c2eb4f6c7f20564f2a76fb) concernant son installation.
<div align="center"><img src="https://raw.githubusercontent.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/refs/heads/main/Images/config-item-suricata.webp" width="75%"/></div>

3. L'Analyse du réseau avec **[Zeek](https://docs.securityonion.net/en/2.4/zeek.html)** *(anciennement Bro)*
   > Il s'agit d'un dispositif d'analyse réseau qui collecte et sauvegarde des données détaillées concernant le trafic réseau, permettant ainsi une vue d'ensemble pour des analyses approfondies des activités. **Zeek** signale à la fois la perte de paquets et la perte de capture.
<div align="center"><img src="https://raw.githubusercontent.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/refs/heads/main/Images/config-item-zeek.webp" width="75%"/></div>

4. La gestion de la réponse à l'incident à travers **[Cases](https://docs.securityonion.net/en/2.4/cases.html)**.
   > Cet outils permet de faire remonter les journaux des **Alerts**, **Dashboards**, **Hunt** de votre console, puis d'affecter des anlaystes, d'ajouter des commentaires et des pièces jointes, et de suivre les observables. Ci-joint une [vidéo](https://www.youtube.com/watch?v=y_kr_hrtqVc&feature=youtu.be&themeRefresh=1) sur la plateforme YouTube pour une introduction à **Cases**.
<div align="center"><img src="https://raw.githubusercontent.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/refs/heads/main/Images/57_0_cases.webp" width="75%"/></div>

5. L'analyse post-incident avec **[NetworkMiner](https://docs.securityonion.net/en/2.4/networkminer.html)** et **[CyberChef](https://docs.securityonion.net/en/2.4/cyberchef.html)**..  
   > Ces deux outils permettent de renforcer les défenses et et prévenur de futures attaques.
<div align="center"><h3>CyberChef</h3></div>
<div align="center"><img src="https://raw.githubusercontent.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/refs/heads/main/Images/68_cyberchef.webp" width="75%"/></div>

</details>

<HR>

<details>
<summary><strong><font size="+1">Utilisation avancée : Les règles de Security Onion</font></strong></summary>
<br>

### Généralités
Security Onion prend charge trois principaux types de règles :
1. [NIDS](https://docs.securityonion.net/en/2.4/nids.html#nids)
    > Les règles **NIDS** sont chargées dans **[Suricata](https://docs.securityonion.net/en/2.4/suricata.html)** pour surveiller le trafic réseau et détecter toute activité suspecte ou notable.
    > Les règles **NIDS** actives génèrent des alertes qui peuvent être trouvées dans la page *Alerts*.
2. [Sigma](https://docs.securityonion.net/en/2.4/sigma.html)
    > Les règles **Sigma** sont chargées dans **[ElastAlert2](https://docs.securityonion.net/en/2.4/elastalert.html#elastalert)** pour surveiller les journaux entrants afin de détecter toute activité suspecte ou digne d'intérêt.
    > Les règles **Sigma** actives génèrent des alertes qui peuvent être trouvées dans la page *Alerts*.
3. [YARA](https://docs.securityonion.net/en/2.4/yara.html)
    > Les règles **YARA** sont chargées dans **[Strelka](https://docs.securityonion.net/en/2.4/strelka.html#strelka)** pour surveiller les fichiers à la recherche de caractéristiques suspectes ou dignes d'intérêt.
    > Les règles **YARA** actives génèrent des alertes qui peuvent être trouvées dans la page *Alerts*.

<br>

### Le menu des règles de détections
Votre console Security Onion inclut une interface de détection pour gérer toutes vos [règles](https://docs.securityonion.net/en/2.4/detections.html#detections) (voir ci-dessus).  
Ci-joint une [vidéo](https://www.youtube.com/watch?v=DelAmqtU2hg&feature=youtu.be) YouTube qui vous permettra d'apprendre à modifier vos règles de détections.  
<br>
<div align="center"><h3>DETECTIONS</h3></div>
<div align="center"><img src="https://github.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/blob/main/Images/57_detections.png" width="75%"/></div>
<br>

### Ajout de règles de détections
Pour ajouter une nouvelle règle (qu'elle soit NIDS, Sigma ou YARA), accédez à la page principale **DETECTIONS** et cliquez sur le bouton bleu + entre Options et la barre de requête.  
Un formulaire apparaîtra dans lequel vous pourrez : 
  * Cliquez sur le menu déroulant Langue et sélectionner **NIDS** / **Sigma** / **YARA** suivant le type de règle que vous avez besoin de rajouter.
  * Spécifier éventuellement une licence
  * Ajouter la signature
  * Cliquez sur le bouton **CREATE** et la détection devrait se déployer sur votre réseau au prochain cycle de 15 minutes.

### Gestion des règles existantes
Vous pouvez gérer les règles existantes toujour depuis la page **DETECTIONS**, il faut rechercher la règle souhaitée et cliquer sur l'icône des jumelles.  
Une fois cela fait, vous pouvez vérifier le champ *Statut* dans le coin supérieur droit et utiliser le curseur pour activer ou désactiver la détection.
Pour modifier la règle de détection, il faudra cliquer sur l'onglet *Tuning* et cliquez sur le bouton bleu + puis suivre les instructions. 

Il est nécessaire de bien gérer ses règles suivant votre secteur d'activité pour une meilleur surveillance des menaces spécifiques.  
Par exemple :  
  * Tentative de connexion SSH non autorisée
  * Scan de port
  * Etc ...  
  
Bien gérer ses règles, cela permet aussi de minimiser les fausses alertes et donc d'améliorer l'efficacité de la surveillance de otre structure.

</details> 

<HR>

<details>
<summary><strong><font size="+1">La Foire Aux Questions !</font></strong></summary>
<br>

***Questions : Quel est le [mot de passe](https://docs.securityonion.net/en/2.4/passwords.html#passwords) ?***<br>
*Réponse*<br>
Pour les comptes utilisateur du système d'exploitation, lorsque vous installer Security Oniont pour la première fois, vous créez un compte utilisateur OS standard pour vous-même. Si vous devez modifier votre mot de passe utilisateur OS, vous pouvez utiliser la commande *passwd*.<br>
<br>

***Questions : Comment ajouter un nouveau [compte utilisateur](https://docs.securityonion.net/en/2.4/adding-accounts.html#adding-accounts) ?***<br>
*Réponse*<br>
Si vous devez ajouter un nouveau compte utilisateur du système d'exploitation, vous pouvez utiliser la commande *adduser*.<br>
Si vous devez ajouter un nouveau compte utilisateur Security Onion Console, accédez à l'interface d'administration, puis cliquez sur *Users*.<br>
<div align="center"><img src="https://raw.githubusercontent.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/refs/heads/main/Images/81_users.webp" width="75%"/></div>

Cliquez sur le bouton **+**, remplissez les informations nécessaires, puis cliquez sur le bouton **ADD**<br>
<div align="center"><img src="https://raw.githubusercontent.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/refs/heads/main/Images/83_users_add.webp" width="75%"/></div>
<br>

Pour plus de réponses à vos questions, voici le [FAQ](https://docs.securityonion.net/en/2.4/faq.html#) officiel de Security Onion.<br>
  
</details>
<HR>
