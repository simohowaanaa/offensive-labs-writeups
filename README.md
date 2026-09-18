# Offensive Labs Write-ups

Portfolio de write-ups issus de laboratoires de cybersécurité **autorisés**. Ce dépôt documente une démarche méthodique : reconnaissance, analyse, exploitation contrôlée, élévation de privilèges et recommandations de remédiation.

> **Usage éthique et légal** — Le contenu de ce dépôt est exclusivement destiné à l'apprentissage, aux CTF et aux environnements pour lesquels une autorisation explicite existe. Ne reproduisez jamais ces techniques sur un système, un réseau ou une application sans autorisation écrite préalable. Les secrets, identifiants et informations sensibles sont exclus des publications.

## Objectif

Construire un portfolio junior orienté offensive security, démontrant la capacité à :

- cartographier une surface d'attaque et prioriser les pistes ;
- exploiter des failles dans un cadre contrôlé ;
- effectuer une post-exploitation raisonnée (Linux, Windows et Active Directory) ;
- expliquer l'impact, les preuves et les mesures correctives de façon claire ;
- produire une documentation reproductible et responsable.

## Structure

```text
.
├── writeups/
│   ├── tryhackme/          # Rooms TryHackMe
│   ├── hack-the-box/       # Machines et challenges Hack The Box
│   ├── other-platforms/    # PortSwigger, VulnHub, CTF, etc.
│   ├── web/                # Classement transversal : applications web
│   ├── linux/              # Classement transversal : systèmes Linux
│   └── active-directory/   # Classement transversal : Windows / AD
├── templates/
│   └── writeup-template.md
├── docs/
│   └── responsible-disclosure.md
└── README.md
```

Un write-up est rangé en priorité dans le dossier de sa plateforme. Les dossiers par thème servent aux laboratoires indépendants d'une plateforme ou aux futures synthèses thématiques.

## Index des write-ups

| # | Plateforme | Lab | Catégorie | Difficulté | Write-up |
| --- | --- | --- | --- | --- | --- |
| 001 | PortSwigger Web Security Academy | SQL injection in WHERE clause allowing retrieval of hidden data | SQL injection | Apprentice | [Lire le write-up](writeups/other-platforms/portswigger/sql-injection-where-clause-hidden-data/) |

Cet index est mis à jour à chaque nouvelle publication.

## Format des write-ups

Chaque lab suit le [template réutilisable](templates/writeup-template.md) et contient :

1. Contexte, périmètre et objectifs du lab ;
2. Résumé exécutif et niveau de difficulté ;
3. Méthodologie : reconnaissance, énumération et validation des hypothèses ;
4. Chaîne d'exploitation avec commandes et preuves soigneusement expurgées ;
5. Élévation de privilèges et post-exploitation, si applicable ;
6. Impact, remédiations et apprentissages.

## Compétences travaillées

| Domaine | Exemples |
| --- | --- |
| Reconnaissance | Nmap, OSINT de lab, énumération de services |
| Web | Authentification, injection, upload, contrôle d'accès |
| Systèmes | Énumération Linux/Windows, permissions, services |
| Active Directory | Cartographie, ACL, Kerberos et mouvements latéraux en lab |
| Reporting | Reproductibilité, analyse d'impact, recommandations |

## Convention de nommage

Créez un dossier par cible : `writeups/<plateforme>/<nom-du-lab>/README.md`.

Exemple : `writeups/tryhackme/blue/README.md`.

Utilisez des noms en minuscules, avec des tirets, et ne publiez jamais de flag, token, mot de passe réel ni contenu qui contourne les règles d'une plateforme.

## Statut

Le dépôt est en cours de construction. Chaque write-up indique clairement son périmètre et les prérequis nécessaires à sa reproduction dans un environnement autorisé.

## Contact

Portfolio maintenu par **[Votre nom]**. Ajoutez ici vos liens professionnels (LinkedIn, GitHub, site personnel) lorsque le dépôt sera publié.
