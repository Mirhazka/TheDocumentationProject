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
Ce n'est pas une obligation d'être sous un OS prédéterminé pour les machines clientes. <br>
Nous avons donc choisi de faire une démonstration sous Linux Ubuntu pour la mahcine utilisateur.

### Machine Ubuntu
  * Nom : **CLILIN01**
  * Compte utilisateur : **wilder**
  * Mot de passe : **Azerty1***
  * Adresse IP fixe : **172.16.10.20/24**

</details>
<HR>

<details>
<summary><strong><font size="+1">Installation du poste serveur Linux CentOS de Security Onion</font></strong></summary>
<div align="center"><img src="https://github.com/WildCodeSchool/TSSR-BDX-0924-P1-G3/blob/main/01_grub.webp" alt="Installation" width="50%"/></div>
<br>

<br> 
1. installation de logiciel Sécurity Onion avec une image Iso 
   https://docs.securityonion.net/en/2.4/download.html#download


<br> 

2.Suivez les instructions, complétez l'installation, puis redémarrez.

<br>
3. Après cela, il suffit de se connecter avec le nom d'utilisateur et le mot de passe prédéfinis dans le cadre du processus d'installation. (voir avec le client) 
<br>
4. L'installation de Security Onion démarre automatiquement. Dans le cas où vous seriez amené à quitter l’installation , il vous suffit juste  de vous déconnecter de votre compte, de vous reconnecter et l’installation démarrera d'elle-même. Si cela ne fonctionne pas, vous pouvez l'exécuter manuellement comme suit :

       [sudo SecurityOnion/setup/so-setup iso]
   


 <br>
     
 [lien installation](https://docs.securityonion.net/en/2.4/installation.html)

 </details>
 
   

<HR>

<details>
<summary><strong><font size="+1">Configuration du système</font></strong></summary>
Explication de la configuration du système après installation des machines.
<br>
 
[Lien de configuration](https://docs.securityonion.net/en/2.4/configuration.html#configuration)

</details>
<HR>

<details>
<summary><strong><font size="+1">La Foire Aux Questions !</font></strong></summary>
TEXTE

</details>
<HR>
