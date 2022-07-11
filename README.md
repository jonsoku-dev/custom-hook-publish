# @jonsoku2/use-star-wars-quote

> I don&#x27;t know this custom hook w

[![NPM](https://img.shields.io/npm/v/@jonsoku2/use-star-wars-quote.svg)](https://www.npmjs.com/package/@jonsoku2/use-star-wars-quote) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save @jonsoku2/use-star-wars-quote
```

## Usage

```tsx
import React from "react";
import { useStarWarsQuote } from "@jsjoeio/use-star-wars-quote";

const App = () => {
  const { quote, loading } = useStarWarsQuote();

  if (loading) return <p>Loading...</p>;

  if (quote) {
    return <div>{quote}</div>;
  }

  return null;
};
export default App;
```

## License

MIT © [jonsoku2](https://github.com/jonsoku2)

---

This hook is created using [create-react-hook](https://github.com/hermanya/create-react-hook).

## package.json

- name 과 author 는 npmjs 의 username으로 해야한다.
- repository는 git에 맞춰서

```json
{
  "name": "@jongseok.lee/use-star-wars-quote",
  "version": "1.0.0",
  "description": "I don&#x27;t know this custom hook w",
  "author": "jongseok.lee",
  "license": "MIT",
  "repository": "jonsoku2/@jonsoku2/use-star-wars-quote",
  "main": "dist/index.js",
  "module": "dist/index.es.js",
  "types": "dist/index.d.ts",
  "jsnext:main": "dist/index.es.js",
  "engines": {
    "node": ">=8",
    "npm": ">=5"
  },
  "scripts": {
    "test": "cross-env CI=1 react-scripts test --env=jsdom",
    "test:watch": "react-scripts test --env=jsdom",
    "build": "rollup -c && tsc -d --emitDeclarationOnly --noEmit false --declarationDir dist",
    "start": "rollup -c -w",
    "prepare": "yarn run build",
    "predeploy": "cd example && yarn install && yarn run build",
    "deploy": "gh-pages -d example/build",
    "postpublish": "git push --tags"
  },
  "dependencies": {},
  "peerDependencies": {
    "react": ">=18.2.0"
  },
  "devDependencies": {
    "@babel/core": "^7.18.6",
    "@babel/runtime": "^7.18.6",
    "@rollup/plugin-babel": "^5.3.1",
    "@rollup/plugin-commonjs": "^22.0.1",
    "@rollup/plugin-node-resolve": "^13.3.0",
    "@rollup/plugin-typescript": "^8.3.3",
    "@rollup/plugin-url": "^7.0.0",
    "@testing-library/react-hooks": "^8.0.1",
    "@types/jest": "^28.1.4",
    "@types/react": "^18.0.15",
    "cross-env": "^7.0.3",
    "gh-pages": "^4.0.0",
    "react": "^18.2.0",
    "react-scripts": "^5.0.1",
    "react-test-renderer": "^18.2.0",
    "rollup": "^2.76.0",
    "rollup-plugin-peer-deps-external": "^2.2.4",
    "tslib": "^2.4.0",
    "typescript": "^4.7.4"
  },
  "publishConfig": {
    "access": "public"
  }
}
```
