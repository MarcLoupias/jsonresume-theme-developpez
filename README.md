# Thème [developpez.com](https://www.developpez.com/) pour les [JSON resume](https://github.com/jsonresume) [![npm version](https://badge.fury.io/js/jsonresume-theme-developpez.svg)](http://badge.fury.io/js/jsonresume-theme-developpez)

Basé sur le thème [Stack Overflow](https://github.com/francescoes/jsonresume-theme-stackoverflow) de Francesco Esposito.

## Usage

Ce thème est à utiliser dans votre propre projet de création de CV en tant que dépendance de développement conjointement avec le [CLI de jsonresume](https://github.com/jsonresume/resume-cli).

```
$ npm i -D jsonresume-theme-developpez
```

### installation du CLI

**Important**

A l'octobre 2018, le CLI du projet [jsonresume](https://github.com/jsonresume) n'est plus maintenu très sérieusement, les dernières versions publiées sur le registre npm présentent des dysfonctionnements importants.

La branche `master` est en revanche fonctionnelle, la bonne méthode d'installation (en attendant un fix officiel) est donc :

```
$ npm i -D https://github.com/jsonresume/resume-cli/
```

Et non `$ npm i -D resume-cli`.

## Contribuer

### Installation

```
$ npm install
```

### Serveur de développement

Il s'agit ici de développer ce thème et non votre propre CV.

```
npm start
```

Vous devriez voir ce message :

```
Preview: http://localhost:4000
Press ctrl-c to stop
```

Le site est généré dans le répertoire `public/` lors du premier accès via votre navigateur.

### Les données du CV

Un fichier `resume.json` est situé à la racine du projet. Il respecte la structure du [schéma json](https://jsonresume.org/schema/).

La commande `npm test` permet de valider le fichier `resume.json` avec le schéma json.

Ce fichier est présent à des fins de tests et de développement, il n'est présent que dans le repository et pas dans le livrable du registre npm.

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
