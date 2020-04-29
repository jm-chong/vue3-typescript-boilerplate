# Vue3 + Typescript + ESLint + Prettier Boilerplate

Setup Vue3 without `cli`.

## Vue3 / Typescript / Webpack

First Install `Vue3`

```
yarn add vue@3
```

Then Install `vue-loader`, `webpack`, `typescript`

```
yarn add -D vue-loader@16 @vue/compiler-sfc@3
yarn add -D webpack-cli webpack webpack-dev-server
yarn add -D typescript ts-loader
```

Then setup `webpack.config.js`, `tsconfig.json`

## ESLint : Vue, Typescript, Prettier

This shows how to handle 3 different syntax with ESLint.

```
yarn add -D eslint eslint-plugin-vue@next
yarn add -D eslint @typescript-eslint/parser @typescript-eslint/eslint-plugin
```

in `.eslintrc.js`, setup 'ParserOptions.parser' with '@typescript-eslint/parser'
see detail [eslint-plugin-vue How to use Custom parser](https://vuejs.github.io/eslint-plugin-vue/user-guide/#how-to-use-custom-parser)

### With Prettier

```
yarn add -D prettier eslint-config-prettier eslint-plugin-prettier
```

Final eslint rules order to be

```
extends: [
    'plugin:vue/vue3-recommended',
    'plugin:@typescript-eslint/recommended',
    'prettier/@typescript-eslint',
    'plugin:prettier/recommended'
  ]
```

And now you are ready to enjoy Vue3 + TS!

Reference

- [Building a Vue 3 component with Typescript](https://dev.to/lmillucci/building-a-vue-3-component-with-typescript-4pge)
- [Using ESLint and Prettier in a TypeScript Project](https://dev.to/robertcoopercode/using-eslint-and-prettier-in-a-typescript-project-53jb)
