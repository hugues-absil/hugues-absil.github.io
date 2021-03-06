---
layout: cours
title: Mode d’emploi du site
permalink: /README/
---

Ce site comprend diverses sections :

- les pages générales (biographie…) ;
- les pages de cours ;
- les pages d’actualité ;
- les pages « galeries » (photos d’œuvre).

## Syntaxe des fichiers
Entre <code>---</code> en haut des fichiers, on place des informations générales
(titre, date…). Pour savoir lesquelles placer, on se réfère aux fichiers déjà existants du même type.

### Syntaxe de base
Les textes sont écrits en syntaxe *Markdown* :

- Italique `*italique*`
- Gras `**gras**`
- Lien vers url `[texte_du_lien](url)`

### Ajouter une image

#### L’image existe déjà sur le site web ou sur un autre site web
On utilise la syntaxe suivante (retirer les \ ) :

<code>{\% include image.html url=http://urldusite caption=légende \%}</code>

On met la bonne url ou on peut prendre l’image déjà existante d’un autre site tel Wikimédia.

#### L’image doit être mise sur le site avant d’être placée
Les images et documents sont classées dans le dossier <code>/files</code> :

- <code>files/cours</code> : comprend les fichiers utilisés dans les cours ;
- <code>files/expositions</code> : comprend des fichiers relatifs aux expositions de Hugues Absil ;
- <code>files/galeries</code> : comprend les fichiers des galeries (voir l’aide sur les galeries) ;
- <code>files/personnel</code> : comprend des fichiers personnels ;
- <code>files/site</code> : comprend des fichiers concernant le site (favicon…).

Puis on utilise la même syntaxe.
