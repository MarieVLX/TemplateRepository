### Git Cheat Sheet

```bash
🚀 Installation & config
git --version
git config --global user.name "Ton Nom"
git config --global user.email "ton.email@example.com"
git config --global init.defaultBranch main

📂 Démarrage
git init
git clone <URL>

🔄 Cycle de vie
git status
git add <fichier>         # stage
git commit -m "msg"
git log --oneline --graph

🌿 Branches
git branch                # lister
git switch -c feature     # créer + switch
git switch main           # changer
git merge feature         # fusionner
git branch -d feature     # supprimer

☁️ Distant
git remote add origin <URL>
git push -u origin main   # premier push
git push                  # suivants
git pull                  # fetch + merge
git fetch                 # sans merge

⚔️ Conflits
Git marque <<<<<<< ======= >>>>>> dans les fichiers
git add <fichier>
git commit

🧹 Stash
git stash push -m "wip"
git stash list
git stash pop

🏷️ Tags
git tag v1.0.0
git tag -a v1.0.0 -m "Release 1.0.0"
git push origin v1.0.0

🛠️ Divers
git diff
git restore <fichier>
git reset --soft HEAD~1   # annuler dernier commit
git revert <hash>         # commit inverse
git reflog                # historique de HEAD
