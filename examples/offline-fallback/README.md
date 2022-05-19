# next-pwa - offline fallback example

[TOC]

> **Checkout this simple and easy way to implement offline fallbacks without inject manifest: **
>
> **[offline-fallback-v2](https://github.com/shadowwalker/next-pwa/tree/master/examples/offline-fallback-v2)**

This example demonstrates how to use `next-pwa` to implement fallback route, image or font when fetch error. Fetch error usually happens when **offline**. (Note fetch is successful even when server returns error codes `404, 400, 500, ...`)

This example uses **Inject Manifest** module from `workbox`. The advantage of using this module is you get more control over your service worker. The disadvantage is that it's more complicated and needs to write more code.

The idea of implementing comprehensive fallbacks can be found [here](https://developers.google.com/web/tools/workbox/guides/advanced-recipes#comprehensive_fallbacks).

> In the future, using inject manifest may not be needed. When [this proposal](https://github.com/GoogleChrome/workbox/issues/2569) is completed in workbox v6.

## Usage

[![Open in Gitpod](https://img.shields.io/badge/Open%20In-Gitpod.io-%231966D2?style=for-the-badge&logo=gitpod)](https://gitpod.io/#https://github.com/shadowwalker/next-pwa/)

``` bash
cd examples/offline-fallback
yarn install
yarn build
yarn start
```

## Recommend `.gitignore`

```
**/public/workbox-*.js
**/public/sw.js
```



