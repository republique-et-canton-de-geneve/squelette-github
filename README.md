Ce projet est un squelette de projet Git.
Il contient une série de fichiers techniques (de licence, de bonne conduite, etc.) et de documentation.
Une fois ces fichiers intégrés à un projet Git, le projet respecte les recommandations de GitHub et les
exigences de l'État de Genève en vue d'une publication en open source sur GitHub.

# Usage

Le plus simple est de copier les fichiers de ce projet dans votre projet Git.
Si votre projet Git n'existe pas encore, vous pouvez le créer à partir de ce squelette :
```
git clone https://github.com/republique-et-canton-de-geneve/squelette-github
git remote --v
git remote set-url origin <URL GitLab DGSIN>
git remote --v
```

Dans tous les cas, apportez ensuite les modifications décrites ci-dessous.

# Modifications à apporter aux fichiers

## Fichier README.md

Ce document fournit la description fonctionnelle et technique de votre projet. Il est obligatoire.
Veuillez remplacer le contenu de ce fichier `README.md` par un contenu plus adéquat.

## Fichier LICENSE.txt

Ce document définit la licence sous laquelle votre projet est posé sur GitHub. Le choix de l'État s'est porté
sur la licence AGPL 3.0.

Aucune modification n'est nécessaire : copiez le fichier `LICENSE.txt` tel quel, à la racine de votre projet.

## Fichier LICENSE-sources.txt

- Ouvrez le fichier `LICENSE-sources.txt` et modifiez les champs à changer : 
  - `Nom du logiciel`
  - `Date`. Remplacer par exemple par `2015 - 2018`.

- Dans chaque fichier source du projet, introduisez en en-tête le contenu du fichier `LICENCE-source.txt` 
ainsi modifié.

- Détruisez le fichier `LICENSE-sources.txt`.

## Fichier CONTRIBUTING.md

Ce document founit aux développeurs de la communauté des instructions sur la manière de collaborer à votre projet.
Il est facultatif, mais recommandé.

Selon que votre projet est en français ou en anglais, renommez le fichier `CONTRIBUTING-fr.md` ou le fichier
`CONTRIBUTING-en.md` en `CONTRIBUTING.md`, puis détruisez l'autre fichier. Le fichier `CONTRIBUTING.md` est à
laisser à la racine de votre projet.

Ces fichiers ne sont que des exemples : vous êtes libre de choisir un autre contenu.
Vous pouvez en particulier consulter les références proposées par GitHub au bas de sa page d'
[instructions](https://help.github.com/articles/setting-guidelines-for-repository-contributors).
Si le format `.md` (markdown) vous rebute, vous être libre de créer un fichier `CONTRIBUTING.txt` en format texte.

## Fichier CODE_OF_CONDUCT.md

Ce document précise aux développeurs de la communauté les attentes de l'État sur l'attitude des participants
au projet. Il vise à établir une atmosphère positive et respecteuse.
Il est facultatif.

Pour l'instant, seule une version en anglais est proposée.

Ce fichier `CODE_OF_CONDUCT.md` est à laisser, tel quel ou modifié, à la racine de votre projet.

Pour en savoir davantage sur le sujet, voir par exemple [ici](https://opensource.guide/code-of-conduct).

## Fichiers ISSUE_TEMPLATE

Ces fichiers guident les développeurs de la communauté lorsqu'ils créent sur GitHub un rapport
d'anomalie ou une proposition d'évolution. Ils sont à trouver dans le répertoire `.github/ISSUE_TEMPLATE`.
Ces fichiers sont facultatifs.

Selon que votre projet est en français ou en anglais,
- détruisez le fichier `bug_report-en.md` ou le fichier `bug_report-fr.md`
- détruisez le fichier `feature-request-en.md` ou le fichier `feature-request-fr.md`.

Vous pouvez modifier le contenu des fichiers restants.
Ils doivent être placés dans le répertoire `.github/ISSUE_TEMPLATE`.

## Pages github.io

Les fichiers présents dans le répertoire `docs` servent à enrichir la
[page GitHub](https://republique-et-canton-de-geneve.github.io) de l'État.

Si votre projet est en français, ces fichiers sont inutiles ; vous pouvez les détruire.

Si votre projet est en anglais et qu'il soit attendu de vous que le projet soit mentionné dans la page
GitHub de l'État, vous pouvez procéder comme suit :
- placez tout le répertoire `docs` dans votre projet
- modifiez le contenu du fichier `index-en.html` en fonction de votre projet. N'oubliez pas d'adapter
les liens hypertexte (chercher "myProject").
Comme source d'inspiration, vous pouvez cliquer sur les projets au bas la 
[page GitHub](https://republique-et-canton-de-geneve.github.io) de l'État.
Recommandation : ne changez que le texte, éventuellement l'agencement, mais pas les images ni le
thème graphique ; cela assurera l'homogénéité de la page GitHub de projet à projet.

Ce répertoire `docs` ne sera vraiment exploité que lorsque la DGSIN l'aura référencé depuis les
sources de la page GitHub.

## Fichier .gitignore

Si votre projet est un projet Java, le fichier `gitignore_java` peut vous intéresser. Renommez-le simplement
en `.gitignore` (sans oublier le `.` en préfixe) et laissez-le à la racine du projet.

Si votre projet n'est pas un projet Java, vous pouvez détruire le fichier `gitignore_java`. 


## GitHub

Dans GitHub, n'oubliez pas d'ajouter une description en une ligne de votre projet (bouton `Edit` sur la page
du projet).

Une fois que tous les fichiers ci-dessus ont été intégrés à votre projet sur GitHub, pour vérifier qu'ils sont
adéquats, allez sur l'onglet `Insights`, puis sur l'option `Community`, et vérifiez que les indicateurs sont
au vert.
L'indicateur "Pull request template" n'est pas au vert, mais le fonctionnement de base de GitHub pour la création
d'une pull request est suffisant.
Notez que vous devez être connecté à GitHub pour voir l'option `Community`.

Vérifiez que vous êtes bien observateur de votre propre projet (bouton `Watch`).
Sans cela, si un développeur de la communauté soumet une pull request ou une "issue" (fiche
d'anomalie ou demande d'évolution), vous ne serez pas averti par courriel.
