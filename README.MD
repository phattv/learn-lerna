### how to run

`yarn install`

`lerna bootstrap`

`node packages/usage/index.js`

expected result: `xxx alpha beta`

### how lerna works
`packages/usage/index.js`
```
"dependencies": {
    "alpha": "1.0.0",
    "beta": "1.0.0"
  }
```
`lerna init` will symlink `alpha` (from packages/alpha) & `beta` (from pacakges/beta) in it's **node_modules**