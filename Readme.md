# byted-koa-favicon 

 Koa middleware for serving a favicon. Based on [koa-favicon]
 本来是想着给egg.js用的，奈何人家自带，所以这个并无卵用，
 只是修改了一下中间件初始化参数，

## Installation

```js
$ npm install byted-koa-favicon
```

## Example

```js
const Koa = require('koa');
const favicon = require('koa-favicon');
const app = new Koa();

app.use(favicon({path: __dirname + '/public/favicon.ico'}));
```

## API

### favicon(options)

Returns a middleware serving the favicon found on the given `options.path`.

#### options

- `maxAge` cache-control max-age directive in ms, defaulting to 1 day.

## License

  MIT
