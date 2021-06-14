# gatsby-source-pokeapi

A gatsby source plugin to fetch Pokemon data through the famous https://pokeapi.co/ API.

## Installation
```
npm install gatsby-source-pokeapi
```

## How to use
In your `gatsby-config.js`
```js
module.exports = {
  plugins: [
    {
      resolve: `gatsby-source-pokeapi`,
      options: {
        nbOfPokemons: 251,
      },
    },
  ],
}
```

## How to query
```js
query {
  allPokemon {
    nodes {
      name
      stats {
        attack
        defense
        special_attack
        hp
        special_defense
        speed
      }
      types
    }
  }
}
```

## License 
This project is under the [MIT license](https://github.com/grdnmsz/gatsby-source-pokeapi/blob/main/LICENSE).
