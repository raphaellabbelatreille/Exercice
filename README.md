# Exercice d'accessibilité des contenus

## Équipe
- Prénom nom
- Prénom nom

## Objectifs
- Expérimenter le versionnage de fichiers avec GIT
- Acquérire des compétences en accessibilité des contenus

## Prérequis
- Avoir lu et pris connaissance des notes du cours 10
- Avoir un compte GitHub
- Avoir installé et configurer GIT sur votre ordinateur
- Avoir installé l'outil CCA (colour-contrast-analyzer)

## Instructions

### 0. 
- Initialiser un dépôt GIT dans le dossier du projet
- Créer un fichier `index.html` et un fichier `style.css`

### 1.	Donner une alternative textuelle aux images

#### 1.1 Baliser dans le fichier `index.html` les images du dossier `1-textes-alternatifs` 

Pour vous guider dans le choix des balises, des attributs et des valeurs d'attributs, utiliser l'arbre de décision et référez-vous aux notes de cours.

#### 1.2 Évaluer la pertinence des contenus textuels alternatifs

Pour chacune des pages ci-dessous, les textes alternatifs sont-ils adéquats ?Commenter votre observation. Pourrait-on faire mieux ? Donnez un exemple de ce que vous proposeriez.

- https://www.sail.ca/fr/chaussures/junior/multi-sport-et-plein-air 
 
 Même si les chausures ne peuvent pas être mieux décrit que cela, il n'y a rien d'autre avec un alt="". Il y a notament une icone qui sert à ce rendre au panier et une autre pour ce connecter. Dans les deux cas, il n'y a aucune description de donné.
 Pour commencer, je rajouterais un alt pour expliquer que cette icon est pour le panier. Sinon, 
[capture-écran](images/1-textes-alternatifs/1-2/screencapture-sail-ca-fr-chaussures-enfant-chaussures-de-sport-2023-02-24-13_38_04.png)

- https://amzn.to/2NnbKPN 

Étonament, les scores d'étoiles de tout les produits ne possèdent pas d'alt mais un petit score en chiffre est déjà placés. Les alts des vélos sont beaucoup plus précis que ceux du site Sail, mais cela s'arête là. La petite announce accroché à la bannière ne stipule que "Prime Video", ce qui n'est pas super clair.
[capture-écran](images/1-textes-alternatifs/1-2/screencapture-amazon-ca-fr-s-2023-02-24-13_45_42.png)

- https://www.lesoleil.com/  

Selon moi, les images ne rajoutent pas tant que cela à la compréhension de la nouvelle. Par contre, il me semble inutiles pour les alts des images de tous simplement répétés le titre de la nouvelle ou du boutons auxquelles ils sont raccrochés. 
Il pourrait tout simplement mettre les alt vident dans ce cas si à moins qu'ils contiennent une donnée plutôt important comme un tableau ou autre.
[capture-écran](images/1-textes-alternatifs/1-2/screencapture-lesoleil-2023-02-24-13_58_36.png)

- https://www.rad.ca/  

Je ne vois absolument aucun alt. La section qui en souffre le plus doit être la grande images dans l'entête. Comme le texte lisible est dans l'image, la désactivation des images la fait disparaitre entièrement. Il devient alors impossible de savoir c'est quoi.
Je ne ferais que séparé le texte de cette image de la même manière que les autres nouvelles et de rajouté un alt résumant chaque image qui ne sont pas raccroché à un titre.
[capture-écran](images/1-textes-alternatifs/1-2/screencapture-rad-ca-2023-02-24-14_05_14.png)

Astuce  
Parfois, l’affichage des alt ne donnent pas un résultat facile à lire… lorsque cela se produit, faites un clic droit de la souris et choisir inspecter pour positionner l’inspecteur de DOM sur le HTML de l’image.
Essayer d’identifier l’emplacement du alt et puis regarder s’il y a une description tout de suite après.

### 2.Vérifier les contrastes de couleurs

#### 2.1	Utiliser l’outil d’analyse de contraste des couleurs (CCA) pour identifier les problèmes de contrastes sur cette page : http://2016.webaquebec.org/

Pour chaque problème de contraste identifié,
documenter le problème par une capture-écran incluant dans son cadre, la zone fautive à gauche et à droite, les résultats détaillés de l’outil, tel que démontré dans l’exemple ci-dessous.

Sauvegarder les captures dans le dossier images. Compléter les liens ci-dessous:
- [Contraste insuffisant 1](images/2-contrastes-couleurs/Capture%20d%E2%80%99%C3%A9cran%201.png)
- [Contraste insuffisant 2](images/2-contrastes-couleurs/Capture%20d%E2%80%99%C3%A9cran%20(34).png)
- [Contraste insuffisant 3](images/2-contrastes-couleurs/Capture%20d%E2%80%99%C3%A9cran%20(35).png)

### 3. Structurer avec les h1-h6 une table des matières

#### 3.1 Vérifier la structure

D’après les captures-écrans que vous trouverez dans le dossier [images/3-table-des-matieres_h1-h6/3-1/](images/3-table-des-matieres_h1-h6/3-1) , est-ce que la table des matières du document est correcte?  

Sinon, expliquez le problème en vous basant sur les règles de base énoncées dans les notes de cours. 

La première capture présente des h1 et h2 mal mit. Par exemple, le seul H1 de celui si semble avoir 4 sous titres alors que seulement un semble lui appartenir. Il faudrait que chaque H qui semble être un titre soit au même niveau.
La deuxième capture d'écran respecte le modèle établit.
__Tutoriel sur les formulaires du w3c__  
[Article](images/3-table-des-matieres_h1-h6/3-1/tuto-form-w3c.pdf)  

[Table des matières (outline)](images/3-table-des-matieres_h1-h6/3-1/tuto-form-w3c-outline.png) 

Réponse : 

----
----
----

__L’affaire Savtchenko__ 
[Article](images/3-table-des-matieres_h1-h6/3-1/article-savtchenko.pdf)  
[Table des matières (outline)](images/3-table-des-matieres_h1-h6/3-1/article-savtchenko-outline.png) 
  
Réponse : 

----
----
----


#### 3.2 S'exercer à bien structurer

- Ouvrir la capture-écran [concevoir-un-design-sans-la-couleur](images/3-table-des-matieres_h1-h6/3-2/concevoir-un-design-sans-la-couleur.pdf) que vous trouverez dans le dossier `sources > h1h6-partie-2` dans le logiciel PhotoShop.  
- Ajouter un calque de blanc à 50% de transparence
- Dans un 3e calque, par-dessus, identifiez les titres et leurs niveaux (h1-h6) de manière voyante (couleur rouge et font-size suffisant)
- Sauvegarder au format .psd ou .png dans le même dossier.
- [Relier ce fichier-réponse ici]()

### 4. Baliser un tableau de données pour qu’il soit accessible

D’après la capture-écran et le texte fourni dans le dossier [4-tableau-de-donnees](images/4-tableau-de-donnees), balisez de manière accessible ce tableau de données.  
  
Votre tableau de données doit comporter un titre (caption) : 

> "Recommandations de consommation de poissons selon l’âge, le sexe et la condition physique".  


Les __entêtes de rangées et de colonnes__ doivent être balisées comme des `<th>` plutôt que des `<td>` et puisque le tableau est *complexe*, vous devez utiliser des attributs `id` dans les `<th>`. 

Chaque cellule `<td>` du tableau doit avoir un attribut headers avec comme valeur(s), le ou les identifiants de ses entêtes de colonnes et de rangées.

Styler le tableau conformément au fichier [consommation-poissons.pdf](images/4-tableau-de-donnees/consommation-poissons.pdf).

#### Ressources
•	balisage accessible d’un tableau (voir les notes du cours 10)
•	balisage html : https://www.w3schools.com/TAGs/tag_table.asp
•	balisage css de tableau: https://www.w3schools.com/css/css_table.asp





