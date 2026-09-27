# Nstein — Guide de mise en ligne (version gratuite)

Ce dossier contient ton app Nstein, installable sur téléphone, 100% gratuite
(IA gratuite Google Gemini + hébergement gratuit Vercel).

## Étape 1 — Récupérer ta clé IA gratuite (2 min, aucune carte bancaire)

1. Va sur : https://aistudio.google.com/app/apikey
2. Connecte-toi avec un compte Google (le tien, ou créés-en un)
3. Clique sur "Create API key"
4. Copie la clé qui apparaît (garde-la dans un bloc-notes)

## Étape 2 — Créer ton compte d'hébergement gratuit

1. Va sur : https://vercel.com
2. Clique "Sign Up", connecte-toi avec Google ou email

## Étape 3 — Mettre le site en ligne

1. Va sur : https://vercel.com/new
2. Dépose ce dossier entier ("nstein-deploy") pour l'importer
3. Vercel crée le projet automatiquement (il détecte index.html et api/chat.js tout seul)
4. Une fois le projet créé, va dans : Project Settings → Environment Variables
5. Ajoute une variable :
   - Nom : GEMINI_API_KEY
   - Valeur : la clé copiée à l'étape 1
6. Redéploie (Vercel te le propose automatiquement, bouton "Redeploy")
7. Tu obtiens un lien du style : https://nstein-xxxx.vercel.app
   → C'est ton lien public, gratuit, sans compte Claude requis

## Étape 4 — Installer l'app sur ton téléphone

**Sur iPhone (Safari) :**
Ouvre ton lien Vercel → bouton Partager (le carré avec la flèche) → "Sur l'écran d'accueil"

**Sur Android (Chrome) :**
Ouvre ton lien Vercel → menu ⋮ en haut à droite → "Installer l'application" ou "Ajouter à l'écran d'accueil"

L'icône Nstein apparaît alors comme une vraie app, en plein écran, sans barre d'adresse.

## Ce qui est vraiment gratuit ici

- Vercel : gratuit
- Gemini : gratuit dans la limite d'un quota d'usage quotidien (largement suffisant
  pour toi et quelques testeurs ; si un jour beaucoup de monde l'utilise en même
  temps, Google peut ralentir ou bloquer temporairement — c'est la contrepartie du gratuit)
- L'app installée sur le téléphone : gratuite, aucun Apple/Google Store impliqué

## Important

- Ne mets jamais ta clé API directement dans le code (index.html ou api/chat.js) —
  elle doit rester uniquement dans les Environment Variables de Vercel.
- Si tu veux vendre l'accès à des clients au-delà du quota gratuit, il faudra
  repasser sur une clé payante (Gemini ou Anthropic) à ce moment-là.
