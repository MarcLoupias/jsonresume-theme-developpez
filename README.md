# Thème [developpez.com](https://www.developpez.com/) pour les [JSON resume](https://github.com/jsonresume) [![npm version](https://badge.fury.io/js/jsonresume-theme-developpez.svg)](http://badge.fury.io/js/jsonresume-theme-developpez)

Basé sur le thème [Stack Overflow](https://github.com/francescoes/jsonresume-theme-stackoverflow) de Francesco Esposito.

**Ce thème n'est pas encore publié sur le registre npm**. La commande `npm install jsonresume-theme-developpez` n'aboutira donc à rien pour le moment.

## Démarrage rapide

### Installation

```
$ npm install
```

### Serveur de développement

```
npm start
```

Vous devriez voir ce message :

```
Preview: http://localhost:4000
Press ctrl-c to stop
```

Le site est généré dans le répertoire `public/`.

### Les données du CV

Pour construire votre propre CV, créez un fichier `resume.json` à la racine du projet et suivez la structure du [schéma json](https://jsonresume.org/schema/).

La commande `npm test` permet de valider le fichier `resume.json` avec le schéma json.

### Génération du livrable

```
npm build
```

Génère le livrable dans le répertoire `dist/`.

### Icônes des réseaux sociaux

**Profils supportés avec leurs couleurs :**

github, stack overflow, linkedin, dribbble, twitter, facebook, pinterest, instagram, soundcloud, wordpress, youtube, flickr, google plus, tumblr, foursquare.

La propriété `network` de la section `profiles` permet de définir le réseau social.

#### Support de propriétés supplémentaires

Les ajouts du [jsonresume-theme-stackoverflow](https://github.com/francescoes/jsonresume-theme-stackoverflow) ont été conservés :

- `keywords` pour chaque objet `work`, `publication` et `volunteer`
- `summary` pour chaque objet `interests`, `education`
- `location` pour chaque objet `work`, `education` et `volunteer`
- `birth` pour `basics`

Exemple avec l'objet `location` : 

```
"location": {
  "city": "Paris",
  "countryCode": "FR",
  "region": "France"
} 
```

Exemple avec l'objet `birth` :

```
"birth": {
  "place": "Paris",
  "state": "France",
  "date": "1988"
}
```

### i18n

Le thème d'origine a été modifié pour supporter le français (et uniquement le français, le thème d'origine ne supportant qu'une seule langue).

*French resume*

## License

[MIT license](http://opensource.org/licenses/mit-license.php).
