<div align="center"><h1>Plateforme de surveillance de sécurité</h1></div>
<div align="center"><h2>Guide de l'utilisateur</h2></div>
<br>
<br>
<br>

<details>
<summary><strong><font size="+1">Security Onion ou Wireshark ?</font></strong></summary>

### Security Onion
[Security Onion](https://securityonionsolutions.com/) est un outils pour détecter, surveiller et réagir immédiatement aux incidents de sécurité sur votre réseau.

### Wireshark
[Wireshark](https://www.wireshark.org/) est un outils de surveillance réseau. Il capture les flux en direct et permet de les analyser ensuite. Il prend en charge les principaux protocoles de chiffrement, afin de pouvoir comprendre les flux malgré les dispositifs de sécurité en place.

### Finalité
Contrairement à Security Onion où tout est automatisé, un employé doit constamment être besoin pour l'utilisation de Wireshark pour pouvoir analyser le flux. <br>
C'est pourquoi pour notre projet, nous utiliserons Security Onion pour plus de practicité.

</details>
<HR>




<details>
<summary><strong><font size="+1">Utilisation de base : Comment utiliser les fonctionnalités clés</font></strong></summary>
<br>
   pour rappel security onion  c’est un ensemble d’outils de surveillance et détection avec une suite d’action qui ce suit et se complet .

<br>

 1 – Surveillance du réseau avec l’outil kibana  et qui integrer avec security onion qui permet de surveiller le réseau                                                                                                                                                    
<br>                                                                                                                                                                                                                                                                          
 2- Détection d’intrusion avec Snort/Suricata /IDS qui joue le rôle de la détection                                                                                                                                                                                        
<br>                                                                                                                                                                                                                                                                         
3- analyse du réseau avec zeek (anciennement Bro) : Il s'agit d'un dispositif d'analyse réseau qui collecte et sauvegarde des données détaillées concernant le trafic réseau, permettant ainsi une vue d'ensemble pour des analyses approfondies des activités. 

<br>
 
4-Gestion de la réponse à l'incident à travers TheHive.                                                                                                            
<br>
5-Analyse post-incident avec NetworkMiner et CyberChef pour renforcer les défenses et prévenir de futures attaques

<HR>






<details>
<summary><strong><font size="+1">Utilisation avancée : Comment utiliser aux mieux les options</font></strong></summary>                                                                                                                                                                                                        


  **1-Personnalisation des règles de détection d'intrusion (IDS)**                                                                                                 snort et Suricata sont hautement personnalisables. Vous pouvez affiner les règles pour adapter la détection à le besoin spécifique de votre réseau. Également 
  désactiver des règles inutiles pour réduire les fausses alertes. Utilisez des groupes de règles adaptés à votre secteur d’activité pour surveiller des menaces 
  spécifiques. (par exemple, une tentative de connexion SSH non autorisée ou un scan de port
<br> 
                                                                                                                                                                    **2-Désactivation des règles**: Enlevez ou désactivez les règles inutiles afin de minimiser les fausses alertes.                                             <br>                                                                                                                                                  
                                                                                                                                                                  
  **3-Faire des règles adapter** : Grâce aux groupes de règles adaptés, il est possible d'utiliser des ensembles de règles particuliers à votre secteur pour identifier les menaces les plus pertinentes. Cela réduit les fausses alertes et améliore l’efficacité de la surveillance.                                         

<br>
 **https://www.snort.org/**                                                                                                                                                                                                                                                                                                          **https://suricata.io/**                                                                                                                                                                                                                                                                                                                                                                                                    

                                                                   
                                                           



<HR>







<details>
<summary><strong><font size="+1">La Foire Aux Questions !</font></strong></summary>
TEXTE
  
</details>
<HR>
