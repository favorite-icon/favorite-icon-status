⚠️ Favorite Icon Status
====================

[![NPM version](https://img.shields.io/npm/v/favorite-icon-status.svg?style=flat)](https://www.npmjs.com/package/favorite-icon-status)
[![NPM downloads](https://img.shields.io/npm/dm/favorite-icon-status.svg?style=flat)](https://www.npmjs.com/package/favorite-icon-status)

Small library for status manipulating with desktop favicon.

# Desktop browser support
- Chrome: ✅
- Edge: ✅
- Firefox: ✅
- Opera: ✅
- IE: ❌
- Safari: ❌ (Safari hides favicons)

# Installation
`npm install favorite-icon-status`

# [Demo](https://favorite-icon.github.io/examples/status.html)

# Using
```js
import { FaviconStatus } from 'favorite-icon-status';

const status = new FaviconStatus();
status.set('ok'); // 'ok', 'error' or 'warning'
```

## Advanced options
```js
import { FaviconStatus } from 'favorite-icon-status';

const status = new FaviconStatus({
    faviconSrc: '/icons/favicon.png'
});

status.set('ok'); // 'ok', 'error' or 'warning'
```

# API

## `.set(status: 'ok' | 'error' | 'warning')`
Set the favicon with status.

```js
import { FaviconStatus } from 'favorite-icon-status';

const status = new FaviconStatus();
status.set('ok'); // 'ok', 'error' or 'warning'

```

## `.reset()`
Reset the favicon.

```js
import { FaviconStatus } from 'favorite-icon-status';

const status = new FaviconStatus();

// ...

status.reset();
```

# [License](./LICENSE)
MIT License
