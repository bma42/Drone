# Générateur d'étude de faisabilité drone — déploiement GitHub Pages

Ce dossier contient le générateur prêt à être hébergé sur **GitHub Pages** (gratuit, dispo sur tout appareil avec une simple URL).

## Contenu

- `index.html` — l'application complète (= `Drone.html` renommé pour que GitHub Pages le serve par défaut)
- `.nojekyll` — fichier vide qui désactive Jekyll (évite tout traitement parasite des assets)
- `README.md` — ce document

## Mise en ligne en 5 minutes

### 1. Créer un dépôt sur GitHub

1. Va sur https://github.com et connecte-toi (ou crée un compte gratuit).
2. En haut à droite, clique sur **+** → **New repository**.
3. Nom : `drone-mission` (ou ce que tu veux). **Privé** ou **Public**, peu importe — Pages fonctionne dans les deux cas.
4. Coche **Add a README file**.
5. Clique **Create repository**.

### 2. Téléverser les fichiers

1. Sur la page du nouveau dépôt, clique **Add file** → **Upload files**.
2. Glisse-dépose **les 3 fichiers de ce dossier** (`index.html`, `.nojekyll`, `README.md`).
   - ⚠ Sous macOS, `.nojekyll` est masqué : pour le rendre visible avant le drag, presse **⌘ + Maj + .** dans le Finder.
3. En bas, clique **Commit changes**.

### 3. Activer GitHub Pages

1. Onglet **Settings** du dépôt (en haut à droite).
2. Menu de gauche : **Pages**.
3. Sous **Source**, sélectionne **Deploy from a branch**.
4. Sous **Branch**, choisis `main` + `/ (root)`, puis **Save**.
5. Attends 1 à 2 minutes — GitHub publie l'URL.

### 4. Ouvrir l'application

L'URL prend la forme :

```
https://<ton-pseudo>.github.io/drone-mission/
```

(elle s'affiche dans la même page **Settings → Pages** une fois le déploiement terminé)

Ajoute-la aux **favoris** sur ton téléphone (Safari → bouton partager → Ajouter à l'écran d'accueil) et tu auras une icône qui ouvre l'app comme une appli native, avec **toutes les fonctions** (carte, autocomplétion, météo, etc.).

## Mises à jour ultérieures

Pour publier une nouvelle version :

1. Sur GitHub, ouvre `index.html`.
2. Clique sur l'icône crayon (en haut à droite).
3. Colle le contenu mis à jour de `Drone.html`.
4. **Commit changes**.

GitHub Pages republiera automatiquement en 30 s. L'URL ne change jamais.

## Confidentialité

- En **dépôt privé**, GitHub Pages reste **public** (l'URL est devinable). Pour vraiment restreindre, il faut un compte GitHub Pro + désactiver Pages public, ou utiliser un autre hébergement (Cloudflare Pages avec accès restreint, Netlify avec protection par mot de passe).
- L'app ne fait aucun envoi serveur : tout reste dans le navigateur. Les données saisies ne sortent pas du téléphone.

## Alternative : Cloudflare Pages

Si tu préfères une URL plus discrète + protection par mot de passe gratuite :

1. https://pages.cloudflare.com → **Connect Git** → ton repo
2. Build command : (vide)
3. Build output directory : `/`
4. Deploy

Bonus : Cloudflare permet de protéger l'accès par **Cloudflare Access** (gratuit jusqu'à 50 utilisateurs).
