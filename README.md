<h1 align="center">hyper-adapter-memory</h1>
<p align="center">A Cache port adapter for local memory in the <a href="https://hyper.io/">hyper</a>  service framework</p>
</p>
<p align="center">
  <a href="https://nest.land/package/hyper-adapter-memory"><img src="https://nest.land/badge.svg" alt="Nest Badge" /></a>
  <a href="https://github.com/hyper63/hyper-adapter-memory/actions/workflows/test.yml"><img src="https://github.com/hyper63/hyper-adapter-memory/actions/workflows/test.yml/badge.svg" alt="Test" /></a>
  <a href="https://github.com/hyper63/hyper-adapter-memory/tags/"><img src="https://img.shields.io/github/tag/hyper63/hyper-adapter-memory" alt="Current Version" /></a>
</p>

---

## Table of Contents

- [Getting Started](#getting-started)
- [Installation](#installation)
- [Features](#features)
- [Methods](#methods)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

```js
import { default as memory } from "https://x.nest.land/hyper-adapter-memory@1.2.5/mod.js";

export default {
  app: opine,
  adapter: [
    {
      port: "cache",
      plugins: [memory()],
    },
  ],
};
```

## Installation

This is a Deno module available to import from
[nest.land](https://nest.land/package/hyper-adapter-memory)

deps.js

```js
export { default as memory } from "https://x.nest.land/hyper-adapter-memory@1.2.5/mod.js";
```

## Features

- Create a named store in `memory`
- Destroy a named store in `memory`
- Create a document in a store in `memory`
- Get a document from a store in `memory`
- Update a document in a store in `memory`
- Delete a document from a store in `memory`
- List documents in a sttore in `memory`

## Methods

This adapter fully implements the Search port and can be used as the
[hyper Cache service](https://docs.hyper.io/cache-api) adapter

See the full port [here](https://nest.land/package/hyper-port-cache)

## Contributing

Contributions are welcome! See the hyper
[contribution guide](https://docs.hyper.io/contributing-to-hyper)

## Testing

```
./scripts/test.sh
```

To lint, check formatting, and run unit tests

## License

Apache-2.0
