# Comprendre la mécanique des skills

Un skill **pédagogique** pour Claude : il explique, en vulgarisation et avec des
schémas, comment fonctionnent les *skills* de Claude et sa *fenêtre de contexte*
— structure d'un skill, déclenchement, chaîne de tokens, architecture du
contexte, ordres de grandeur, débordement, et hygiène du contexte.

## Contenu du dépôt

- `SKILL.md` — le tuteur (rôle, méthode, message d'accueil, carte des modules).
- `references/` — le contenu pédagogique détaillé (modules 0 à 7 + encart),
  le catalogue d'illustrations, et l'annexe installation/partage.
- `assets/` — 10 illustrations SVG autonomes.

## Installation

### Dans l'app Claude (claude.ai)
1. **Customize → Compétences → « + »**.
2. Soit **« Ajouter depuis GitHub »** en pointant ce dépôt, soit télécharger ce
   dépôt en ZIP et le téléverser. (Le fichier `.skill` de la page *Releases*
   peut aussi être téléversé directement.)
3. Vérifier que le skill est **activé** (commutateur sur ON).

### Dans Claude Code
```bash
git clone https://github.com/lecinquiemejour-code/mecanique-des-skills.git ~/.claude/skills/mecanique-des-skills
```

## Affichage des illustrations

Les schémas sont des fichiers SVG autonomes dans `assets/`. Le tuteur les affiche
au moment opportun via un outil de rendu visuel ; le catalogue et les
déclencheurs sont décrits dans `references/illustrations.md`.

## Sécurité

Un skill peut, en principe, faire exécuter du code par Claude. **Relisez toujours
le contenu d'un skill avant de l'activer.** Celui-ci ne contient que du Markdown
et des SVG — aucun script, aucune dépendance.

## Auteur & licence

Créé par Jean Noël Lefebvre (L5J). Distribué sous licence **GNU GPL v3.0** (voir `LICENSE`).
