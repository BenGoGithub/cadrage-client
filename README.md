# Outil de cadrage projet client

Formulaire web interactif pour cadrer un projet client avant développement.
Zéro dépendance — un seul fichier HTML à ouvrir ou héberger.

---

## Stack

HTML / CSS / JS vanilla · Fichier unique · Zéro backend · Zéro CDN

## Fonctionnalités

- **8 sections** : recueil du besoin (1–4) + cadrage du périmètre (5–8)
- **MoSCoW** : table de fonctionnalités avec priorités dynamiques (Must / Should / Could / Won't)
- **Jalons** : table préremplie avec les 5 étapes standard, éditables
- **Autosave** : sauvegarde silencieuse dans `localStorage` (debounce 300 ms)
- **Export client** : Markdown des sections 1–8
- **Export complet** : Markdown 1–8 + notes de décision internes
- **Impression / PDF** : `Ctrl+P` → rendu propre, boutons masqués

## Usage

### Par double-clic

Ouvrir `cadrage-client.html` directement dans le navigateur.
Les données sont persistées localement entre les sessions.

### GitHub Pages

Déposer `cadrage-client.html` à la racine du repo.
Activer Pages sur la branche `main` — l'outil est accessible via l'URL du site.

### VPS / hébergement statique

Copier `cadrage-client.html` dans le répertoire web servi.
Aucune configuration serveur requise.

## Fichiers

| Fichier | Rôle |
|---------|------|
| `cadrage-client.html` | Artefact complet (HTML + CSS + JS inline) |
| `cadrage-projet-client.md` | Canevas source — spec des 8 sections |

## Réinitialiser entre deux clients

Bouton **↺ Réinitialiser** dans l'en-tête → vide le `localStorage` et repart de zéro.
