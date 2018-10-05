# Developpez.com theme for jsonresume [![npm version](https://badge.fury.io/js/jsonresume-theme-developpez.svg)](http://badge.fury.io/js/jsonresume-theme-developpez)

Based on [Stack Overflow theme for jsonresume](https://github.com/francescoes/jsonresume-theme-stackoverflow) by Francesco Esposito.

**Printable version with custom CSS**

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

Pour construire votre propre CV, créez un fichier `resume.json` à la racine du projet et suivez la structure du [schéma json](https://jsonresume.org/schema/).

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
  "city": "Zürich",
  "countryCode": "CH",
  "region": "Switzerland"
} 
```

Exemple avec l'objet `birth` :

```
"birth": {
  "place": "New York",
  "state": "USA",
  "date": "1988"
}
```

### i18n

Le thème d'origine a été modifié pour supporter le français (et uniquement le français, le thème d'origin ne supportant qu'une seule langue).

## License

[MIT license](http://opensource.org/licenses/mit-license.php).
