# Installation écran 3.5 pouces pour Raspberry Pi 2 ET 3 B/B+/A+/A/B

### sources = https://github.com/goodtft/LCD-show

![alt text](https://images-na.ssl-images-amazon.com/images/I/7115DVSOKfL._SL1500_.jpg)

Alimentation par broches GPIO

Configurer l’écran 3.5 inch TFT LCD Touch Screen avec le Raspberry Pi

Caractéristiques de l’écran

    Ecran TFT LCD
    Interface SPI
    3.5 pouces
    320 * 480 pixels
    65536 couleurs



## Installation des drivers et résolution du problème d’écran blanc Raspberry Pi

Au commencement, l'écran se fiche sur les broches gpio du Raspberry Pi. 

L’écran affiche un écran blanc.

Puis entrer dans le terminal et d’y inscrire ces quelques lignes pour installer les drivers de l’ecran lcd 3.5 sur votre Raspberry pi.

    sudo rm -rf LCD-show
    git clone https://github.com/goodtft/LCD-show.git
    chmod -R 755 LCD-show
    cd LCD-show/
    sudo ./LCD35-show

Après redémarrage du Raspberry Pi vous devriez voir apparaitre le desktop de Raspbian sur votre petit écran 🙂

#Désactiver l’écran LCD 3.5 du raspberry pi et retourner vers un écran HDMI

Lorsque votre écran est “activé” sur le Raspberry pi, vous ne pouvez plus utiliser d’écran standard sur la sortie HDMI. Si vous avez le besoin de faire marche arrière et de retourner a un écran classique vous devrez tapez les ligne suivante:

    chmod -R 755 LCD-show
    cd LCD-show/
    sudo ./LCD-hdmi


#Pour ceux qui voudraient sauter cette étape, sachez qu’il existe des Raspbian Custom intégrant directement les drivers pour l’écran. Vous pouvez les trouver à cet adresse en bas de page: http://www.lcdwiki.com/3.5inch_RPi_Display .
