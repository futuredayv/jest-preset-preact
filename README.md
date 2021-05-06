# Customized for Vite
Supports esmodules for **Vite**. [See this issue](https://github.com/babel/babel/issues/9849#issuecomment-592668815)

Jest preset containing all required configuration for writing tests for [preact](https://github.com/preactjs/preact).

Features:

- Transpiles JSX to `h()`
- Aaliases for `"react"` imports to point to `preact/compat`
- Automatically serialize Preact `VNodes` in snapshots
- Stub style imports (`.css`, `.less`, `.sass/scss`, etc)
- Add typeahead preview for filtering in jest's watch mode

## Usage

### 1. Install it via npm or yarn:

```sh
yarn add -D "git+https://github.com/futuredayv/jest-preset-preact.git"

# or via npm

npm install -D "git+https://github.com/futuredayv/jest-preset-preact.git"
```

### 2. Add the preset to your jest config.


You can write your jest config into your `package.json`, also, you may prefer to keep it in it's own file. Either way Jest picks it.
```json
"jest": {
	"preset": "jest-preset-preact"
}
```

also, you may prefer to keep it in it's own file.
```js
// jest.config.js
module.exports = {
	preset: 'jest-preset-preact',
};
```

## License

MIT, see [the LICENSE file](./LICENSE).
