# Evaluation Stratégie Debuggage Product Feedback

Sujet d'évaluation contrôle continu sur la stratégie de débuggage avec les APIs et le DOM en Javascript de niveau 4.

![illustration](./docs/sujet2-figma.png)

## Résumé

**Durée: 1h**

**Matériels et outils autorisés**:

- Ordinateur
- Internet

**Interdiction**:

- IA génératives type ChatGPT, Google Gemini, GitHub Copilot, etc... ne sont pas autorisées.

---

## Consignes

**<ins>Avant de commencer</ins>**:

1. **Créer un répository publique** sur votre github nommé `exam-api-product-feedbacks`

2. **Télécharger et décompresser** le fichier [debug-startupfile.zip](https://drive.google.com/file/d/1ioP2zgynaMwT-R1JKqE3Xduh3-OK1Y_J/view?usp=drive_link)

3. **Publier** l'ensemble de votre code dans votre repository github.

### Sujet - Debuggage Javascript DOM et API

**Description**

A partir du fichier `index.html` présent dans le fichier [debug-startupfile.zip](https://drive.google.com/file/d/1ioP2zgynaMwT-R1JKqE3Xduh3-OK1Y_J/view?usp=drive_link), vous devez trouver et régler 15 bugs cachés dans le script `js/app.js` afin d'afficher dynamiquement la liste de commentaires appartenent à au feedback dont l'id est `2`.

Vous devez <ins>uniquement</ins> modifier le code Javascript `js/app.js` pour réparer les 15 bugs cachés dans l'application.

**Maquette Figma**: [Lien vers la maquette Figma](https://www.figma.com/design/4o3XpxzWhK3JSGqztwxBei/subject-api-product-feedback?node-id=1027-2&p=f&t=5OGkujep40Q4RjBE-0)

**URL de l'API**: `http://51.38.232.174:3002`

**Documentation de l'API**: `http://51.38.232.174:3002/v1/swagger.json`

**Objectifs**:

- Au chargement de la page, l'application doit afficher l'ensemble des champs (`votes`, `title`, `description`, `category`) du feedback possèdant l'id: `2` ainsi que le nombre de commentaires associés au feedback.


- Au chargement de la page, l'application doit afficher la liste des commentaires associés au feedback.


- Au chargement de la page, l'application doit afficher le nombre total de commentaire à droite du titre `Comments` au dessus de la liste des commentaires.


- Lorsque l'utilisateur clique sur le bouton `Post Comment`, l'application doit émettre une requête à l'API pour créer un nouveau commentaire en utilisant le texte présent dans la balise `<textarea></textarea>` et l'afficher dans la liste de commenaire. _(Si la réponse retourné par l'API est réussie alors il faudra afficher le nouveau commentaire dans la liste des commentaires déjà existante)_.


- Lorsque l'utilisateur ajoute un caractère dans le champs de text dans la balise `<textarea>` du formulaire, l'application doit afficher le nombre de caractère restant à gauche du bouton `Post Comments`.

**Tips**:

- Prenez le temps d'analyser la structure du fichier `index.html` afin de comprendre l'organisation global de la page ainsi que des balises qui la compose.

- Liser le code `Javascript` dans le fichier `js/app.js` pour retracer le parcours du programme et comprendre l'ordre dans lequel les instructions sont réalisées.
