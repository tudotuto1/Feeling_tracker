# aujourd’hui 🌅🌱

Un compagnon de journée pour enfant (et parents) : journal d’humeurs, liste de
tâches planifiable jusqu’à un mois à l’avance, et bilan hebdo/mensuel à partager.

**100 % gratuit · aucune installation · aucune clé · aucun serveur.**
Tout fonctionne dans le navigateur, et les données sont enregistrées localement
sur l’appareil de chaque personne.

-----

## ▶️ Tester tout de suite (sans rien installer)

Double-clique sur `index.html` : il s’ouvre dans ton navigateur. C’est tout.
(Une connexion internet est nécessaire la 1re fois pour charger les librairies.)

-----

## 🚀 Le mettre en ligne sur GitHub (pour que tes amis / parents testent)

1. Crée un compte sur **github.com** (gratuit), puis clique sur **New repository**.
1. Donne-lui un nom (ex. `aujourdhui`), laisse-le **Public**, et clique **Create repository**.
1. Sur la page du dépôt, clique **Add file → Upload files**, puis dépose le fichier
   **`index.html`** (à la racine, pas dans un dossier). Clique **Commit changes**.
1. Va dans **Settings** (onglet en haut) → **Pages** (menu de gauche).
1. Sous *Build and deployment*, choisis **Source : Deploy from a branch**,
   puis **Branch : `main`** et **`/ (root)`**, et clique **Save**.
1. Attends 1 à 2 minutes, rafraîchis la page : un lien apparaît, du type
   **`https://ton-pseudo.github.io/aujourdhui/`**.
1. Partage ce lien 🎉 — il s’ouvre sur ordinateur comme sur téléphone.

> 💡 Pour mettre à jour l’appli plus tard : ré-upload `index.html` (Add file →
> Upload files), commit, et le site se met à jour tout seul en ~1 min.

-----

## 📒 Bon à savoir

- **Les données sont locales.** Les humeurs et les tâches sont enregistrées dans
  le navigateur **de chaque personne**. Elles ne sont pas partagées entre
  appareils, et un autre utilisateur ne voit pas les tiennes.
- **Le bilan est calculé dans l’appli** (verdict, statistiques et conseils),
  sans intelligence artificielle en ligne → **aucun token, aucun coût.**
- **« Envoyer aux parents »** ouvre l’application e-mail avec le bilan déjà
  rédigé. **« Copier le bilan »** met le texte dans le presse-papiers.

-----

## 🛠️ En cas de page noire

L’appli charge 3 librairies depuis un CDN. Si jamais elles ne se chargent pas,
ouvre `index.html` dans un éditeur de texte et remplace les 3 lignes
`<script src="https://cdnjs...">` du `<head>` par celles-ci :

```html
<script src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
<script src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
<script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
```

Puis ré-enregistre et ré-upload le fichier.

-----

## ➡️ Et après ?

Cette version est volontairement gratuite et hors-ligne. Si un jour tu veux les
**conseils rédigés par une IA** (plus personnalisés, basés sur les commentaires),
ou l’**envoi automatique du bilan chaque semaine**, il faudra ajouter un petit
serveur (fonction serverless) qui garde une clé API secrète. C’est faisable —
mais ce n’est plus gratuit ni sans configuration.