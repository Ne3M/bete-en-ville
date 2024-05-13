# Les petites betes en ville

Salut !  
Voici quelques instruction pour ajouter des pages et prévisualiser le site.

## Comment créer de nouvelles pages

1. Premierement, pour créer une page, tu va dupliquer le fichier `/src/pages/la-coccinelle.astro` et le renommer avec le nom que tu veux. Le nom de ce fichier définira l'URL de la page, donc veille a y mettre des tirets, et à garder l'ensemble cohérent.

2. Ensuite, tu pourras créer un nouveau dossier dans `/src/images/` et garder la même structure que dans le dossier coccinelle.

3. Enfin dans le dossier `/public/` tu vas pouvoir ajouter le fichier `.glb` pour la 3D

4. Dans le fichier `/src/components/layout/Header.astro` tu pourras éditer le liens vers ta nouvelle page


Normalement, tout est prêt pour commencer l'édition. Ca va se passer dans ton fichier `.astro` que tu as créé à l'étape 1.
Tu vas surement commencer par modifier les URl des images dont tu as besoin, il faudra y mettre le chemin des images que tu as ajouté dans `/src/images/`
Ensuite, tu pourras descendre dans le fichier et en modifier le contenu.

___

## Comment visualiser les modifications en direct

Pour voir tes modifications en direct, tu va devoir utiliser le terminal. Pour l'ouvrir, ça se passe dans la barre de menu en haut `Terminal > New terminal`

Ensuite pour lancer le mode developpement, tu vas lancer la commande suivante `npm run dev`. Le terminal te fournira l'adresse locale ou tu peux voir le site, l'url ressemble à quelques chose comme ça `http://localhost:xxxx/`. Il te suffira de faire un `ctrl + click` dessus pour l'ouvrir dans Chrome.

Le rafraichissement est automatique, il te suffit de sauvegarder un fichier pour que les modification soient prise en compte.

Pour arreter la tache dans le terminal (quand tu as terminé), il te suffit de faire un `ctrl + c` dans le terminal pour terminer la tache.

___

## Comment vérifier que l'ensemble fonctionnera en ligne

Pour vérifier que le site est fonctionnel une fois compilé, nous allons d'abord le faire une fois en local.

Pour cela, il faut lancer la commande `npm run build`  
Une fois que la compilation est finie, tu peux voir le site compilé avec la commande `npm run preview`

Le script te fournira une URL comme pour le mode de developpement.

___

## Comment envoyer les modifications sur github et déclencher une mise à jour du site web

Une fois que tu es satisfaite de ta page, il est temps d'envoyer ton code vers github. Il sera sauvegardé, et récupérable sur d'autres PC.

Pour cela nous allons aussi utiliser le terminal, avec `git` cette fois-ci.

Tout d'abord, tu vas vérifier les fichier que tu as modifié en utilisant la commande suivante :
```git
git status
```
Elle va te lister l'ensemble des fichiers modifié. En cas de soucis appelle moi, mais en théorie, tu ne devrais pas avoir de surprise.

Une fois validé les fichiers à envoyer, tu vas tous les ajouter à ton futur commit via la commande :
```git
git add .
```

Enfin, tu va créer un commit et lui associer un message. Ca se fait via la commande :
```git
git commit -m "Page <nom_de_la_page>"
```

Et enfin, tu va pouvoir envoyer tes données au serveur avec la commande suivante :
```git
git push
```


Tout le reste est automatique, et tu devrais voir la mise à jour apparaitre en ligne après quelques minutes.


Bon courage !