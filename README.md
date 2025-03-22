# Git & GitFlow Cheat Sheet

<div align="center">
  <img height="80" src="https://miro.medium.com/v2/resize:fit:640/format:webp/1*sOWIyC1rjrWSUdIS1KvyHw.gif" />
</div>
 

Ce document est un guide pratique pour comprendre et maîtriser Git et GitFlow. Que vous soyez un débutant découvrant les bases ou un utilisateur expérimenté cherchant à approfondir ses connaissances, cette cheat sheet aborde un large éventail de sujets essentiels.


## Table des matières

# 1. Git <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" height="39" alt="git logo"  />
  <img width="20" />
</div>

## [1.1 Introduction à Git](git-gitflow-documents/git.md)

## [1.2 Installation et configuration de Git](git-gitflow-documents/git.md)

## [1.3 Les bases de Git](git-gitflow-documents/git.md)

## [1.4 Git pour les projets collaboratif](git-gitflow-documents/git.md)



# 2. GitFlow <img src="https://res.cloudinary.com/practicaldev/image/fetch/s--b_QCE-F_--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_800/https://my-bucket-image2.s3.amazonaws.com/ImageGitHub/git-flow-logo.png" height="39" alt="git logo" />
  <img width="20" />
</div>

## [2.1 Guide Complet sur GitFlow](git-gitflow-documents/gitflow.md)
  
## [2.2 Installation de GitFlow](git-gitflow-documents/gitflow.md)
  
## [2.3 Initialisation de GitFlow dans un projet](git-gitflow-documents/gitflow.md) 
   
## [2.4 Utilisation des branches GitFlow](git-gitflow-documents/gitflow.md)
  
## [2.5 Commandes avancées et bonnes pratiques](git-gitflow-documents/gitflow.md)

## [2.6 Problèmes courants et solutions](git-gitflow-documents/gitflow.md)

## [2.7 Conclusion](git-gitflow-documents/gitflow.md)


# 3. Git & GitFlow Cheat Sheet : Commandes Principales 

Ce cheat sheet couvre les commandes essentielles pour **Git** et **GitFlow** afin de gérer efficacement les versions et le développement collaboratif.

<table>
    <thead>
        <tr>
            <th>Commande</th>
            <th>Fonction</th>
            <th>Exemple</th>
        </tr>   
    </thead>
    <tbody>
        <tr>
            <th colspan="3" align="left"> Mise en place & Initialisation</th>
        </tr>
        <tr>
            <td align="right"><code>git init</code></td>
            <td>Initialise un dépôt Git dans le dossier courant</td>
            <td></td>
        </tr>
         <tr>
            <td align="right"><code>git clone [url]</code></td>
            <td>Récupère l'entièreté d'un dépôt distant via URL</td>
            <td><code>git clone git@github.com:Simplon-hdf/cheats-sheets-git-flow.git</code></td>
        </tr>
        <tr>
            <th colspan="3" align="left">Index</th>
        </tr>
            <td align="right"><code>git status</code></td>
            <td>Affiche les fichiers modifiés dans le répertoire de travail</td>
            <td></td>
        </tr>
        <tr>
            <td align="right"><code>git ad﻿d [fichier]</code></td>
            <td>Déplace un fichier dans la zone de stage</td>
            <td><code>git add exemple.md</code></td>
        </tr>
        <tr>
            <td align="right"><code>git reset [fichier]</code></td>
            <td>Enlève un fichier de l'index tout en gardant les changements dans le répertoire de travail</td>
            <td><code>git reset exemple.md</code></td>
        </tr>
         <tr>
            <td align="right"><code>git diff</code></td>
            <td>Différence des changements en dehors de l'index</td>
            <td></td>
        </tr>
        <tr>
            <td align="right"><code>git diff --staged</code></td>
            <td>Différence entre l'index et le dernier commit</td>
            <td></td>
        </tr>
        <tr>
            <td align="right"><code>git diff [branche locale] [branche distante]</code></td>
            <td>Compare les différences entre une branche locale et distante</td>
            <td><code>git diff develop main</code></td>
        </tr>
        <tr>
            <td align="right"><code>git commit -m [message]</code></td>
            <td>Effectue le commit contenant les fichiers dans l'index</td>
            <td><code>git commit -m "Renamed exemple.md"</code></td>
        </tr>
        <tr>
            <th colspan="3" align="left">Branches</th>
        </tr>
        <tr>
            <td align="right"><code>git branch -av</code></td>
            <td>Liste les branches. Un * apparaîtra à côté de la branche actuelle</td>
            <td></td>
        </tr>
        <tr>
            <td align="right"><code>git branch [branche]</code></td>
            <td>Créer une nouvelle branche</td>
            <td><code>git branch main</code></td>
        </tr>
        <tr>
            <td align="right"><code>git switch [branche]</code></td>
            <td>Change la branche courante</td>
            <td><code>git switch develop</code></td>
        </tr>
        <tr>
            <td align="right"><code>git branch -d [branche]</code></td>
            <td>Supprime la branche locale</td>
            <td><code>git branch -d develop</code></td>
        </tr>
        <tr>
            <td align="right"><code>git checkout --track</code></td>
            <td>Créer une nouvelle branche locale à partir d'une branche distante, et la suivre</td>
            <td></td>
        <tr>
            <td align="right"><code>git tag [tag-name]</code></td>
            <td>Créer un tag sur le commit actuel</td>
            <td><code>git tag v1.0</code></td>
        </tr>
        </tr>
        <tr>
            <th colspan="3" align="left">Historique</th> 
        </tr>
        <tr>
            <td align="right"><code>git log</code></td>
            <td>Affiche l'historique des commits</td>
            <td></td>
        </tr>
        <tr>
            <td align="right"><code>git log -p [fichier]</code></td>
            <td>Affiche l'historique des commits sur un fichier spécifique</td>
            <td><code>git log -p exemple.md</code></td>
        </tr>
        <tr>
            <td align="right"><code>git blame [fichier]</code></td>
            <td>Affiche l'historique des modifications, y compris l'auteur sur un fichier spécifique</td>
            <td><code>git blame exemple.md</code></td>
        </tr>
        <tr>
            <th colspan="3" align="left">Mise à jour et publication</th>
        </tr>
        <tr>
            <td align="right"><code>git remote -v</code></td>
            <td>Liste les remote configurés</td>
            <td></td>
        </tr>
        <tr>
            <td align="right"><code>git remote show [remote]</code></td>
            <td>Affiche les informations de la remote</td>
            <td><code>git remote show origin</code></td>
        </tr>
        <tr>
            <td align="right"><code>git remote add [remote] [url]</code></td>
            <td>Permet de créer une connexion avec un dépôt distant sous un raccourci</td>
            <td><code>git remote add origin git@github.com:Simplon-hdf/cheats-sheets-git-flow.git</code></td>
        </tr>
        <tr>
            <td align="right"><code>git fetch [remote]</code></td>
            <td>Récupère toutes les modifications de la remote sans fusionner les changements</td>
            <td><code>git fetch origin</code></td>
        </tr>
        <tr>
            <td align="right"><code>git pull [remote] [branche]</code></td>
            <td>Récupère les modifications de la branche, et les fusionne</td>
            <td><code>git pull origin main</code></td>
        </tr>
        <tr>
            <td align="right"><code>git push [remote] [branche]</code></td>
            <td>Pousse les commits d'une branche locale vers un dépôt distant</td>
            <td><code>git push origin main</code></td>
        </tr>
        <tr>
            <th colspan="3" align="left">Fusionner & Rebaser</th>
        </tr>
        <tr>
            <td align="right"><code>git merge [branche]</code></td>
            <td>Fusionne la branche spécifiée avec la branche actuelle</td>
            <td><code>git merge main</code></td>
        </tr>
        <tr>
            <td align="right"><code>git rebase [branche]</code></td>
            <td>Réapplique l'historique des commits de la branche actuelle au dessus de la branche spécifiée</td>
            <td><code>git rebase main</code></td>
        </tr>
        <tr>
            <td align="right"><code>git rebase --abort</code></td>
            <td>Annule le processus de rebase en cours</td>
            <td></td>
        </tr>
        <tr>
            <td align="right"><code>git rebase --continue</code></td>
            <td>Poursuit le processus de rebase après la résolution des conflits</td>
            <td></td>
        </tr>
        <tr>
            <td align="right"><code>git mergetool</code></td>
            <td>Ouvre un outil de fusion pour résoudre les conflits</td>
            <td></td>
        </tr>
        <tr>
            <th colspan="3" align="left"    >Rétablir/Annuler</th>
        </tr>
        <tr>
            <td align="right"><code>git reset --hard HEAD</code></td>
            <td>Réinitialise l'index et le répertoire de travail au commit référencé par HEAD</td>
            <td><code>git reset --hard @~1</code></td>
        </tr>
        <tr>
            <td align="right"><code>git checkout HEAD [fichier]</code></td>
            <td>Restaure un fichier spécifique dans le répertoire de travail au dernier commit (HEAD)</td>
            <td><codue>git checkout HEAD exemple.md</code></td>
        </tr>
        <tr>
            <td align="right"><code>git revert [commit]</code></td>
            <td>Annule les modifications d'un commit spécifique</td>
            <td><code>git revert 8d6fe82</code></td>
        </tr>
        <tr>
            <td align="right"><code>git reset --hard [commit]</code></td>
            <td>Réinitialise l'index et le répertoire de travail au commit spécifié</td>
            <td><code>git reset --hard 8d6fe82</code></td>
        </tr>
        <tr>
            <td align="right"><code>git reset [commit]</code></td>
            <td>Déplace la branche actuelle vers le commit spécifié</td>
            <td><code>git reset 8d6fe82</code></td>
        </tr>
        <tr>
            <td align="right"><code>git reset --keep [commit]</code></td>
            <td>Déplace la branche tout en conservant les modifications en dehors de l'index </td>
            <td><code>git reset --keep 8d6fe82</code></td>
        </tr>
    </tbody>

</table>

### Outils Utilisés

- ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
- ![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white)
- ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)


# Auteurs

#### Abdellah
- **Role**: Tech lead
- **GitHub**: [Abdellah](https://github.com/abdellah59)

#### Aymeric
- **Role**: Developeur
- **GitHub**: [Aymeric](https://github.com/x2z591)

#### Milan
- **Role**: Developeur
- **GitHub**: [Milan](https://github.com/Milan59300)

#### Julien
- **Role**: Developeur
- **GitHub**: [Julien](https://github.com/SymBiios)