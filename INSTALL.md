<div align="center"><h1>Plateforme de surveillance de sécurité</h1></div>
<div align="center"><h2>Documentation pour les administrateurs</h2></div>
<br>  
      

<br>
<br>






<details>
<summary><strong><font size="+1">Pré-requis technique</font></strong></summary>


## installation de security onion 
<br>        avoir 3 Machine 
<br>              1 Machine avec un os windows 
<br>              2 Machine avec un os linux 
<br>              3 Le logiciel Security Onion qui dispose de son propre OS serveur Linux CentOS.

</details>
<HR> 
     










<details>
<summary><strong><font size="+1">Installation des postes clients</font></strong></summary>

## les postes clients

- Poste client sous Linux 
- Accès réseau entre Security Onion et le client
- Adresse IP Statique pour le serveur de Security Onion

</details>
<HR>







<details>
<summary><strong><font size="+1">Installation du poste serveur CentOS de Security Onion</font></strong></summary>

 Dans cette partie, nous expliquons comment installer **Security Onion** sur un serveur tournant sous Linux CentOS :

1. [Configuration et installation de Security Onion](https://securityonion.net/)
2. Installer Security Onion sur un système CentOS.
3. Configuration du serveur :
   - Configurer une adresse IP statique pour le serveur.
   - Sélectionner les composants à installer comme **Elasticsearch/Kibana**, **Suricata**, **Zeek**.
4. Mise en place des outils d'analyse.
</details>

  
</details>
<HR>








<details>
<summary><strong><font size="+1">Configuration du système</font></strong></summary>

1. Configuration des outils Security Onion.
2. Configurer des alertes et des dashboards afin de montrer les notifications en temps réel (Kibana) pour visualiser les logs de manière compréhensible :
- Exemples : graphiques des alertes, logs de connexion.
3. Mettre en place des règles de pare-feu pour interdire l'accès aux adresses IP suspectes.


</details>
<HR>













<details>
<summary><strong><font size="+1">La Foire Aux Questions !</font></strong></summary>
TEXTE

</details>
<HR>
