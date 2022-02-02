# SuuntoLinkWine

#### Un moyen de synchroniser et de configurer votre montre Suunto sous Linux...

[English version](README.md).

***

### 1 - Installer Wine :

*Vous devez avoir au moins la version **6.6 de Wine** pour povoir installer .NET 4.5*  
*Vous devez avoir aussi une version **Wine-Staging** sans quoi le programme d'installation de SuuntoLink ne voudra pas s'exécuter (erreur de droits administrateur).*

La meilleure façon est d'installer la dernière version de Wine fournie par WINE-HQ : regardez [ici pour les différentes distributions Linux](https://wiki.winehq.org/Download "Wine-HQ for Linux").

*Pour la suite, la méthode expliquée fonctionne sur mon **Ubuntu 20.04**. Vous devrez surement adapter certaines étapes selon votre distribution Linux.*

**Astuce :** la commande `wine --version` retourne la version de Wine installée sur votre système.

***

### 2 - Installer Winetricks :

*Winetricks est un script qui vous facilitera l'installation de certains logiciels sous Wine.*

Une installation rapide (pas très propre) peut être faite par les commandes suivantes :

    wget  https://raw.githubusercontent.com/Winetricks/winetricks/master/src/winetricks
    chmod +x winetricks
    sudo mv winetricks /usr/bin/

**Astuce :** la commande `winetricks --version` retourne la version de Winetricks installée sur votre système.

***

### 3 - Changez les droits sur les périphériques HID :

*Une montre Suunto branchée sur un système Linux apparait dans `/dev/hidrawX` (X étant le numéro du périphérique HID correspondant à votre montre).*

*Par défaut, seul l'utilisateur **root** possède les droits de lecture/écriture sur le périphérique.*

Pour **créer automatiquement un règle** qui affectera les bons droits sur votre montre Suunto, nous utiliserons le script proposé par [openambit](https://github.com/openambitproject/openambit) (merci aux auteurs).

*J'en fait une copie ici au cas où...*


***

### 4 - Prepare Wine :

***

### 5 - Install SuuntoLink  :

***

### 6 (Optional) - Create a launcher :

***

![Watch OK](ok.png "It seems so work !")

***

#### Known bugs :
