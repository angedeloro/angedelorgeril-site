# ange de lorgeril — site : ce qu'il reste à compléter

Le site est un site statique (aucun outil à installer). Il contient :

- `index.html` : la page unique
- `mentions-legales.html` : la page des mentions légales
- `style.css` : toute la mise en forme (couleurs, polices, tailles)
- `assets/` : les favicons

## 1. À compléter avant de publier

| Quoi | Où | Comment |
|---|---|---|
| **Ton email** | `index.html` (4 endroits) et `mentions-legales.html` (2 endroits) | Chercher `contact@angedelorgeril.fr` et le remplacer partout par ton adresse |
| **Ton Instagram** | `index.html` (2 boutons « Instagram ») | Remplacer `https://www.instagram.com/` par le lien de ton nouveau compte, par exemple `https://www.instagram.com/ton-compte` |
| **SIRET** | `mentions-legales.html` | Remplacer le texte surligné « À COMPLÉTER » |
| **Adresse professionnelle** | `mentions-legales.html` | Idem |
| **TVA** | `mentions-legales.html` | Si tu es en franchise de TVA, garde la mention proposée ; sinon adapte-la |
| **Adresse de l'hébergeur** | `mentions-legales.html` | À reprendre depuis les pages légales de vercel.com |

Astuce : dans un éditeur de texte, la fonction « Rechercher et remplacer dans tous les fichiers » fait le travail en une fois.

Le texte des mentions légales est un modèle de départ, pas un avis juridique : fais-le relire avant publication.

## 2. À ajuster la semaine prochaine

Tu vas travailler ton offre et ton positionnement. Voici où intervenir :

- **Tarifs ou formules** : à ajouter dans une nouvelle section de `index.html`, entre « Méthode » et « À propos ».
- **FAQ** : les réponses sur le budget et les résultats sont volontairement prudentes (aucun chiffre promis). Adapte-les à ton offre.
- **Études de cas** : remplace le bloc en pointillés de la section « Réalisations » quand tu auras tes premiers résultats.
- **Texte « À propos »** : rédigé de façon neutre, à personnaliser (école, parcours, projets de design marquants).

## 3. Police : hébergement local (recommandé)

Le site charge la police Space Grotesk depuis Google Fonts. Cela fonctionne, mais envoie l'adresse IP des visiteurs à Google. Pour l'éviter :

1. Télécharger les fichiers de la police (Space Grotesk, graisses 300, 400, 500 et 700) et les placer dans un dossier `assets/fonts/`.
2. Remplacer les lignes `<link ... fonts.googleapis.com ...>` de `index.html` et `mentions-legales.html` par des règles `@font-face` dans `style.css`.
3. Supprimer le dernier paragraphe de la section « Données personnelles » dans `mentions-legales.html`.

Si tu m'envoies les fichiers de la police, je fais ces trois étapes pour toi.

## 4. Mise en ligne (GitHub + Vercel)

1. Sur GitHub, crée un dépôt (par exemple `site-ange-de-lorgeril`), en public ou privé.
2. Dépose **tout le contenu du dossier** (pas le dossier lui-même) à la racine du dépôt : `index.html`, `mentions-legales.html`, `style.css`, `assets/`.
3. Sur Vercel, clique sur « Add New… » puis « Project », importe ton dépôt et clique sur « Deploy ». Aucun réglage n'est nécessaire.
4. Plus tard, ajoute ton nom de domaine dans les réglages du projet Vercel.

Chaque modification enregistrée sur GitHub met le site à jour automatiquement.

## 6. Interrupteur clair / sombre

Le site contient un bouton (lune / soleil) dans l'en-tête. Au premier passage, il suit le réglage du téléphone ou de l'ordinateur du visiteur ; ensuite, le choix est mémorisé dans son navigateur. Rien d'autre à faire.
