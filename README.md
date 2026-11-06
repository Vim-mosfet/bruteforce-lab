# ⚡ BruteForce Lab - Simulateur de Terminal Hydra

Application web interactive conçue pour démontrer visuellement la vitesse d'une attaque brute-force et l'efficacité des mots de passe complexes lors d'ateliers cybersécurité (collège / lycée).

## 🌐 Accès direct à l'outil en ligne

Le site est hébergé sur GitHub Pages et accessible directement ici :  
👉 **[https://Vim-mosfet.github.io/bruteforce-lab/](https://Vim-mosfet.github.io/bruteforce-lab/)**

---

## 🎯 Principe de la démonstration

1. **Interface scindée 50/50** : D'un côté le réseau social ("Faux-book"), de l'autre le terminal Linux.
2. **Saisie au clavier** : L'intervenant tape la commande dans le terminal devant les élèves.
3. **Impact visuel** : Défilement ultra-rapide des mots de passe et ouverture automatique du compte piraté (ou message d'échec sur les mots de passe forts).

---

## ⌨️ Commandes & Scénarios

1. **Mot de passe simple (`123456`)** :
   `hydra -l lucas -P dictionnaire_simple.txt`  
   *→ Piraté en 0.8s*

2. **Attaque OSINT (`Lucas2010`)** :
   `cupp -i lucas 2010 && hydra -P dictionnaire_lucas.txt`  
   *→ Piraté en 2s grâce aux infos publiques (réseaux sociaux)*

3. **Méthode de la phrase (`U5v!Qcdlh3?`)** :
   `hydra -l lucas -P dictionnaire_complexe.txt`  
   *→ ÉCHEC (Temps estimé : +400 ans)*
   
