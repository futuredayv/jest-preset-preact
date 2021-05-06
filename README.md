# jest-preset-preact

## Customized for Vite
Supports esmodules for **Vite**. [See this issue](https://github.com/babel/babel/issues/9849#issuecomment-592668815)

Jest preset containing all required configuration for writing tests for [preact](https://github.com/preactjs/preact).

Features:

- Transpiles JSX to `h()`
- Aaliases for `"react"` imports to point to `preact/compat`
- Automatically serialize Preact `VNodes` in snapshots
- Stub style imports (`.css`, `.less`, `.sass/scss`, etc)
- Add typeahead preview for filtering in jest's watch mode

## Usage

Install it via npm or yarn:

```bash
npm install --save-dev jest-preset-preact
# or via yarn
yarn add -D jest-preset-preact
```

...and add the preset to your `jest.config.js` file.

```js
// jest.config.js
module.exports = {
	preset: 'jest-preset-preact',
};
```

## License

MIT, see [the LICENSE file](./LICENSE).
