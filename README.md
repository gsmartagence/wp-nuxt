# wp-nuxt
[![npm (scoped with tag)](https://img.shields.io/npm/v/wp-nuxt/latest.svg?style=flat-square)](https://npmjs.com/package/wp-nuxt)
[![npm](https://img.shields.io/npm/dt/wp-nuxt.svg?style=flat-square)](https://npmjs.com/package/wp-nuxt)
[![CircleCI](https://img.shields.io/circleci/github/yashha/wp-nuxt.svg?style=flat-square)](https://circleci.com/gh/)
[![Codecov](https://img.shields.io/codecov/c/github/yashha/wp-nuxt.svg?style=flat-square)](https://codecov.io/gh/)
[![Dependencies](https://david-dm.org/yashha/wp-nuxt/status.svg?style=flat-square)](https://david-dm.org/)
[![js-standard-style](https://img.shields.io/badge/code_style-standard-brightgreen.svg?style=flat-square)](http://standardjs.com)

> 

[📖 **Release Notes**](./CHANGELOG.md)

## Features

The module features

## Setup
- Add `wp-nuxt` dependency using yarn or npm to your project
- Add `wp-nuxt` to `modules` section of `nuxt.config.js`

```js
{
  modules: [
    // Simple usage
    'wp-nuxt',

    // With options
    ['wp-nuxt', { /* module options */ }],
 ]
}
```

## Usage

You can use the API of [WP-API](https://github.com/WP-API/node-wpapi) using the injected 'app.$wp'. (s. example)

### Example
```js
  <script>
export default {
  async asyncData ({ app, store, params }) {
    return { articles: await app.$wp.posts().perPage(10) }
  }
}
</script>
```

## License

[MIT License](./LICENSE)

Copyright (c) yasark <yasarkkk@protonmail.com>
