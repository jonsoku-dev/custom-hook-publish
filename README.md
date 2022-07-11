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
