#TP1

# Attaques passives : sniffing passif

## Deffinition

Les sniffers (appelé aussi « analyseurs de protocoles » ou « analyseurs de réseau ») sont des outils logiciels qui peuvent capturer les trames circulant sur un réseau local et afficher leurs contenus (entêtes des protocoles, identités des utilisateurs, mot de passe non cryptés, etc).

## Objectif

- Implémenter un sniffer passif simple
- Manipuler des logiciels de sniffing

## Outils logiciels

Linux, wireshark, compilateur cc ou gcc

## Partie 1 : Implémentation d’un sniffer passif

1. Compilation du code source 

a. (cc -c sniffer_eth_ip_tcp_data.c)
    
![IMAGE](codesource.jpeg)

b. puis on génére l'exécutable(cc sniffer_eth_ip_tcp_data.c – o sniffer)

![IMAGE](exec.jpeg)

2. execution du sniffer en mode root (exemple 10 packet)

![IMAGE](testsnif.jpeg)

3. Dans la manipulation précédente, les trames sont affichées sous format hexadécimal. Pour
afficher le contenu de l’entête ETHERNET, il faut enlever le commentaire de la fonction
ParseEthernetHeader ,recompiler puis régénérer l’exécutable et refaire l’étape 2.

les trames s'affiche comment suivant:

![IMAGE](testsnif.jpeg)

