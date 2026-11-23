# TP UI Component Libraries — projet de départ (Vite)

IMT Atlantique · 1re année alternance · cours « UI Component Libraries »

## Le TP

Reproduire le composant **FAQ accordion** de Frontend Mentor (maquettes dans `design/`), avec l'approche choisie par votre groupe.

Ce projet de départ sert aux approches **sans framework** :

| Approche | Techno |
|---|---|
| Classique | Bootstrap |
| Utilitaire | Tailwind CSS |
| Natif | HTML et CSS seuls (`<details>`) |

Les approches Angular Material et Angular Aria utilisent l'autre dépôt, `tp-ui-libs-angular`.

## Démarrer

Prérequis : Node.js 22 ou 24 (versions LTS), npm et git.

```bash
git clone <url-de-ce-depot>
cd tp-ui-libs-vite
npm install
npm run dev
```

Le site s'ouvre sur <http://localhost:5173>.

## Ce qui est fourni, et ce qui ne l'est pas

**Fourni** : un projet Vite vierge, le contenu texte de la FAQ dans `index.html`, les images et les polices dans `public/assets/`, les maquettes dans `design/` et les couleurs et polices dans `style-guide.md`.

**À faire vous-mêmes** : installer et configurer votre bibliothèque. Ça fait partie du TP : le coût d'installation d'une bibliothèque est une des choses que l'on compare à la fin. Partez de la documentation officielle :

- Bootstrap : <https://getbootstrap.com/docs/>
- Tailwind CSS : <https://tailwindcss.com/docs/installation>

**Règle des 15 minutes** : si l'installation ne fonctionne toujours pas au bout de 15 minutes, appelez l'enseignant.

## Ce qui est attendu

**Obligatoire**

- Fidèle à la maquette et responsive.
- Utilisable au clavier : Tab pour circuler, Entrée et Espace pour ouvrir et fermer.
- Le focus est visible sur chaque question.

**Bonus**

- Un seul panneau ouvert à la fois.

### Défis, si vous avez fini

À faire dans l'ordre : chaque défi s'appuie sur le précédent.

1. **Aux couleurs de l'IMT** : appliquez la charte IMT à votre accordéon (bleu IMT `#00B8DE`, bleu foncé `#14223C`, gris `#EDF3F4`, police Arial). Le résultat doit rester accessible.
2. **Une charte modifiable en direct** : ajoutez à la page un panneau pour changer la charte en direct (couleurs, police). Les choix sont conservés au rechargement de la page (`localStorage`).
3. **Exporter les tokens** : un bouton télécharge la charte en cours sous forme de fichier `tokens.css`, réutilisable dans le projet.

## La restitution

3 à 4 minutes par groupe :

1. Démo de votre accordéon.
2. Un test au clavier, en direct.
3. Votre choix : pourquoi cette techno, ou ce que vous auriez choisi.
4. Un avantage et une douleur de votre approche.

## Organisation des fichiers

```
├── index.html          ← le contenu de la FAQ, à structurer
├── src/
│   ├── main.js         ← point d'entrée JavaScript
│   └── style.css       ← vos styles
├── public/assets/      ← images et polices (servies sur /assets/...)
├── design/             ← maquettes mobile, desktop et états actifs
├── style-guide.md      ← couleurs, polices, tailles
└── CHALLENGE.md        ← l'énoncé original de Frontend Mentor (en anglais)
```

## Assistants IA

Les fichiers `AGENTS.md` et `CLAUDE.md` viennent de Frontend Mentor. La plupart des assistants IA les lisent automatiquement : ils vous guideront par questions et indices, sans écrire la solution à votre place.

## Crédits

Challenge par [Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-wyfFdeBwBz). Police Work Sans sous licence SIL Open Font License (`public/assets/fonts/OFL.txt`).
