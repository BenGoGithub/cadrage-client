<!-- template-version: v1.1 -->
# CLAUDE.md — Outil de cadrage client interactif

Fichier de référence lu à chaque session.

---

## Règles absolues — Sécurité

- Ne jamais commiter `.env`, `.env.*`, `*.local`.
- Ne jamais inclure de secrets, clés API ou tokens dans le code ou les commits.
- Validation explicite requise avant toute action destructive (suppression, force-push, etc.).
- Proposer avant d'agir — ne jamais modifier sans que Ben ait dit « go ».

---

## Préférences générales

- **Langue** : répondre en français. Commits, commentaires et docstrings en anglais.
- **Commits** : conventionnels (`feat:`, `fix:`, `docs:`, `chore:`), pas de `Co-Authored-By`.
- **Ne jamais produire de code sans demande explicite.**
- **DRY / KISS / Clean Code** — pas d'abstraction prématurée.

---

## Contexte projet

- **Nom** : Outil de cadrage client interactif
- **Type** : artefact web autonome — livrable client + support soutenance CDA
- **Objectif** : cadrer un projet web client avant développement, réutilisable sur tous les futurs clients
- **Stack** : HTML / CSS / JS vanilla, fichier unique, zéro dépendance, zéro backend
- **Structure** :
  - `cadrage-client.html` — artefact complet (HTML + CSS + JS inline)
  - `cadrage-projet-client.md` — canevas source / spec des 8 sections
  - `README.md` — description, usage, déploiement

---

## Workflow Git

- Branches : `actualisation` (staging) → `main` (prod / publication)
- Flux montant : `feat/*` | `fix/*` | `docs/*` | `chore/*` → `actualisation` → `main`
- Ben seul mergeur vers `main`
- Pas de PR automatique — merge direct sur `actualisation`, PR pour `main`
- Pas de `--no-verify`, pas de force-push sans validation explicite

---

## Workflow Tâches

- **Pas de liste Nextcloud dédiée** (garde-fou 5 listes + critère de durabilité < 3 mois).
- Les tâches de dev sont rattachées à la liste **`Soutenance`** dans Nextcloud.
- Suivre `docs/TASK_ROUTING.md` du repo Productivity pour tout arbitrage de routing.
