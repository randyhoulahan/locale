---
sidebarDepth: 2
---
# Locale Service

## Description

 Resolves the Locale from as a lowercase 2 letter code:


1. HTML 5 Locale 
```html 
<html lang="en"> 
```
2. Legacy HTML meta tag 
```html 
<meta http-equiv="content-language" content="en">
```
3. Legacy Browsers
```js
navigator.languages[0] || navigator.userLanguage || navigator.language || navigator.browserLanguage 
```
4. Browser
```js
(new Intl.NumberFormat()).resolvedOptions().locale
```

## Install

```bash
yarn add @houlagins/locale

#OR 

npm install @houlagins/locale
```

## API

### getLocale
```js
import { getLocale } from '@houlagins/locale'

const locale = getLocale()

console.log(locale)
```

### getUnLocale
Returns one of the 6 UN languages or default en.

```js
//[ 'ar', 'en', 'es', 'fr', 'ru', 'zh' ]
import { getUnLocale } from '@houlagins/locale'

const locale = getUnLocale()

console.log(locale)
```
