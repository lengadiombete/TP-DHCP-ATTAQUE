# TP Sécurité Réseau – Attaque DHCP Starvation

## Description
Ce travail pratique consiste à étudier le fonctionnement du protocole DHCP
et à démontrer une attaque de type **DHCP Starvation**.
Cette attaque permet d’épuiser le pool d’adresses IP d’un serveur DHCP,
empêchant ainsi les nouveaux clients d’obtenir une configuration réseau valide.

## Objectifs du TP
- Comprendre le fonctionnement du protocole DHCP
- Configurer un serveur DHCP sous Linux
- Vérifier l’attribution d’adresses IP aux clients
- Réaliser une attaque DHCP Starvation à l’aide de l’outil Yersinia
- Analyser l’impact de l’attaque sur le réseau

## Environnement de travail
- Oracle VirtualBox
- Serveur Linux (isc-dhcp-server)
- Client Linux
- Kali Linux (machine attaquante)

## Technologies utilisées
- Linux (Ubuntu / Kali Linux)
- isc-dhcp-server
- Yersinia
- Protocole DHCP
- Réseaux TCP/IP

## Instructions d’exécution
1. Démarrer les machines virtuelles (Serveur DHCP, Client, Kali Linux)
2. Vérifier que le serveur DHCP est actif
3. Vérifier que le client reçoit une adresse IP
4. 
5. Lancer l’attaque DHCP Starvation avec la commande :
   ```bash
   sudo yersinia dhcp -attack 1 -interface eth0
   
