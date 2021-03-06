<p align="center">
  <img alt="svgson" title="svgson" src="https://cdn.rawgit.com/elrumordelaluz/svgson/7883b450/logo.svg" width="450">
</p>

<h5 align="center">
  <code>cli</code>
</h5>

<p align="center">
  CLI version of <a href="https://github.com/elrumordelaluz/svgson">svgson</a>
</p>

## Install

```zsh
npm i -g svgson-cli
```

## Usage

```zsh
svgson icon.svg --output icon.json
```

## API

```zsh
 svgson input [options]
```

#### input

If specified `file` or `folder` with `.svg` files, otherwise `stdin`

#### options

##### output

Output filename

Type: `string`<br>
Default: `stdout`
Alias: `o`<br>

##### pretty

Prettyfied output

Type: `boolean`<br>
Default: `false`
Alias: `p`<br>

##### separated

Create separated output files<br>
Works only with folder input

Type: `boolean`<br>
Default: `false`
Alias: `s`<br>

##### camelcase

Camelcase attributes names

Type: `boolean`<br>
Default: `false`
Alias: `c`<br>

### Example using [svgo](https://github.com/svg/svgo)

```
svgo --input=svgs/icon-1.svg --output=- | svgson --pretty > icon-1.json
```

## Related

[svgson](https://github.com/elrumordelaluz/svgson) Transform SVG into `Object`

[element-to-path](https://github.com/elrumordelaluz/element-to-path) Convert SVG element into `path`

[path-that-svg](https://github.com/elrumordelaluz/path-that-svg) Convert entire SVG with `path`

[svg-path-tools](https://github.com/elrumordelaluz/svg-path-tools) Tools to manipulate SVG `path` (d)

## License

MIT © [Lionel T](https://lionel.tzatzk.in)
