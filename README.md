# 📚 Documentation Général
---
### 📑 Sommaire
- [🎯 Objectifs](#objectifs)
- [👥 Membres et rôles du groupe](#membres-et-rôles-du-groupe)
- [⚙️ Choix Techniques](#choix-techniques)
- [📜 Introduction](#introduction)
- [⚠️ Difficultés rencontrées](#difficultés-rencontrées)
- [💡 Solutions et alternatives trouvées](#solutions-et-alternatives-trouvées)
- [🚀 Améliorations possibles](#améliorations-possibles)
---
### **📝 Présentation du Projet**

**🎯 Objectifs**
<span id="objectifs"></span>  

**Principal:**
- 🌐 Scanner les ports d'un serveur (*à partir d'un client*)
- 🔒 Dans un environnement autorisé
- 🕵️‍♂️ Déduire des potentielles failles de sécurité

**Secondaire:**
- 🛠️ Créations de profils de scan personnalisés

### **👥 Membres et rôles du groupe**
<span id="membres-et-rôles-du-groupe"></span>  
| Prénom    | Rôles              | Tâches                      | 
| --------- | ------------------ | --------------------------- |
| Tom       | Product Owner      | Doc Admin, NMAP, VM, IP     |
| Balthazar | Membre             | NMAP                        |
| Thomas    | Membre             | VM (Serveur), IP            |
| Fabien    | Scrum Master       | Management                  |

### **⚙️ Choix Techniques**
<span id="choix-techniques"></span>
**📦 Logiciels**
- Nmap 👁️‍🗨️: Outil de scan de ports, disponible sous toutes les distributions.
- Wireshark 🦈 *(optionnel)* : Outil d'analyse réseau, utilisé pour surveiller le trafic en temps réel. 

**🖥️ Serveur : Debian 12**
- Nom : SRVLX01
- Compte : root
- Mot de passe : Azerty1*
- Adresse IP fixe : 172.16.10.10/24

**🐧  Client : Ubuntu 22.04**
- Nom : CLILIN01
- Compte utilisateur : wilder
- Mot de passe : Azerty1*
- Adresse IP fixe : 172.16.10.20/24

**💻 Client : Windows 10**
- Nom : CLIWIN02
- Compte utilisateur : wilder
- Mot de passe : Azerty1*
- Adresse IP fixe : 172.16.10.30/24
---
### **📜 Introduction**
<span id="introduction"></span> 
Dans un monde où tout est connecté et fonctionne grâce aux 0 et 1, nous faisons face à de nombreuses problématiques, notamment la sécurisation de réseau. Dans ce cadre, Nous allons scanner les ports d'un réseau afin d'identifier d'éventuelles failles de sécurité ou des ports ouverts qui ne devraient pas l'être. Dans ce cas, ces ports seront fermés pour limiter les risques et empêcher les cybercriminels d'exploiter ces vulnérabilités pour corrompre le réseau.

### **⚠️ Difficultés rencontrées**
<span id="difficultés-rencontrées"></span>
- Configuration de l'IP fixe
  - En essayant de la configurer, nous étions en mode "**NAT**", un autre problème était la configuration de l'IP fixe nous avons été confrontés à plusieurs soucis de configuration de celle-ci.
- a définir
- a définir 

### **💡 Solutions et alternatives trouvées**
<span id="solutions-et-alternatives-trouvées"></span>
- Configuration de l'IP fixe
  - Pour résoudre les problèmes que nous avions rencontrés, nous devions régler le mode réseau sur "**Bridge**" au lieu de "**NAT**" Ensuite pour le problème de configuration IP fixe, il fallait la configurer dans le fichier: `/etc/NetworkManager/` , sans oublier de définir le bon gateway sinon on ne peut ni envoyer ni recevoir de paquets.

### **🚀 Améliorations possibles**
<span id="améliorations-possibles"></span>
