# Mon Portfolio 2026

Portfolio personnel développé en HTML / CSS / JavaScript pur.

---

## Structure du projet

```
portfolio/
├── index.html       ← ton site complet (une seule page)
├── vercel.json      ← configuration Vercel
├── .gitignore       ← fichiers à ignorer par Git
├── CV-MonNom.pdf    ← ton CV (à ajouter toi-même)
└── ma-photo.jpg     ← ta photo (à ajouter toi-même)
```

---

## Déployer sur Vercel (étape par étape)

### ÉTAPE 1 — Installer Git
Va sur https://git-scm.com/downloads et installe Git.
Vérifie l'installation dans le terminal PyCharm :
```
git --version
```

### ÉTAPE 2 — Créer un compte GitHub
Va sur https://github.com → "Sign up" → crée ton compte gratuit.

### ÉTAPE 3 — Créer un dépôt GitHub
1. Connecte-toi sur GitHub
2. Clique sur le "+" en haut à droite → "New repository"
3. Nom : `mon-portfolio`
4. Laisse tout par défaut → clique "Create repository"
5. GitHub t'affiche des commandes → copie l'URL de ton repo
   (ex: https://github.com/tonnom/mon-portfolio.git)

### ÉTAPE 4 — Initialiser Git dans PyCharm
Dans le terminal PyCharm (View → Tool Windows → Terminal) :
```bash
cd chemin/vers/ton/dossier/portfolio
git init
git add .
git commit -m "Premier commit — portfolio 2026"
git branch -M main
git remote add origin https://github.com/tonnom/mon-portfolio.git
git push -u origin main
```
> Remplace l'URL par celle de ton vrai repo.

### ÉTAPE 5 — Déployer sur Vercel
1. Va sur https://vercel.com → "Sign Up" avec ton compte GitHub
2. Clique "Add New Project"
3. Clique "Import" à côté de `mon-portfolio`
4. Ne change rien → clique "Deploy"
5. En 30 secondes ton site est en ligne !
   URL exemple : https://mon-portfolio.vercel.app

### ÉTAPE 6 — Mettre à jour le site
À chaque modification dans PyCharm, dans le terminal :
```bash
git add .
git commit -m "Description de ma modif"
git push
```
Vercel redéploie automatiquement en 20 secondes.

---

## Personnaliser le portfolio

### Ajouter ta photo
1. Copie ta photo dans ce dossier (ex: `ma-photo.jpg`)
2. Dans index.html, remplace le bloc `<div class="profile-placeholder">` par :
```html
<img class="profile-card-img" src="ma-photo.jpg" alt="Ma photo">
```

### Activer le téléchargement du CV
1. Copie ton CV dans ce dossier (ex: `CV-MonNom.pdf`)
2. Dans index.html, cherche `href="#" download` et remplace par :
```html
href="CV-MonNom.pdf" download
```

### Changer ton nom
Dans index.html, cherche `Ton Prénom Nom` et remplace par ton vrai nom.

### Changer ton email
Dans index.html, cherche `ton.email@exemple.com` et remplace (2 endroits).