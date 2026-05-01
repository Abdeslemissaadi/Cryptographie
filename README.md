# 🔐 Cryptographie Appliquée — Diffie-Hellman, RSA & ECDSA

> Implémentation from scratch des trois piliers de la cryptographie moderne, avec une approche orientée cybersécurité et IA.

---

##  Description

Ce projet implémente en Python les algorithmes fondamentaux qui sécurisent les communications numériques aujourd'hui — les mêmes protocoles utilisés dans TLS, les VPNs, les blockchains et les systèmes d'authentification modernes.
Dans un contexte où l'IA est de plus en plus utilisée pour détecter des anomalies cryptographiques, casser des implémentations vulnérables ou renforcer les protocoles de sécurité, comprendre ces fondations mathématiques est essentiel.


##  Algorithmes Implémentés

###  Partie I — Diffie-Hellman
- Échange de clés sur un canal non sécurisé
- Génération d'un nombre premier p et d'un générateur g
- Calcul des clés publiques/privées et de la clé secrète commune K
- Base du protocole DH+AES utilisé dans HTTPS

###  Partie II — RSA
- Génération complète des clés (p, q, n, φ(n), e, d)
- Chiffrement et déchiffrement via exponentiation modulaire rapide
- Implémentation de l'algorithme d'Euclide étendu pour calculer d
- Même mécanique que celle utilisée dans les certificats SSL/TLS

###  Partie III — ECDSA (Courbes Elliptiques)
- Construction d'une courbe elliptique y² = x³ + 1 sur Z/pZ
- Addition et multiplication scalaire de points (méthode binaire)
- Génération de clés publiques/privées sur la courbe
- Signature et vérification numérique d'un message
- Utilisé dans Bitcoin, Ethereum et les passeports biométriques


##  Lien avec la Cybersécurité & l'IA

Ces algorithmes sont au cœur des enjeux actuels en cybersécurité :
- Les modèles d'IA sont aujourd'hui utilisés pour **détecter des clés faibles** ou des paramètres mal générés
- Le **Logarithme Discret** (base de DH et ECDSA) est une cible active des recherches en **cryptanalyse assistée par IA**
- La montée des **ordinateurs quantiques** menace RSA et DH — comprendre ces bases est essentiel pour passer aux algorithmes post-quantiques (NIST 2024)
- Les mêmes courbes elliptiques sécurisent les **wallets crypto** et les **systèmes d'authentification zero-trust**

## 📋 Paramètres Personnalisables (info perso)

```python
NUMERO_ETUDIANT = 23010931   # Utilisé pour générer p
JOUR_MOIS       = 2710       # Clé secrète d'Alice / s (ECDSA)
ANNEE_NAISSANCE = 2001       # Clé secrète de Bob / message M
```
