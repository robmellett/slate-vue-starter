## This is a vue starter template for slate, it is based on Shopify's starter template


Thanks to [@dan-gamble](https://github.com/dan-gamble) for helping with the slate configurations

Thanks to [@liron-navon](https://github.com/liron-navon) for the initial Vue.js Config

This project is based off [shopify/skeleton-theme](https://github.com/shopify/skeleton-theme), checkout Slate for more information.

get started
```
$ yarn create slate-theme my-new-theme robmellett/slate-vue-starter
```


### How to work with slate for Shopify:

- rename .env-sample to .env and setup your development store config.

- run: npm start 
- slate will open your localhost, just ignore that, and go to your development store. 
- In the development store you should have your theme loaded
- Changes will hot reload in the dev store.

### Using vue in shopify

- Do notice that this is not meant to be an SPA, for that you can use storefront, vue here is purely to replace JQuery for logic operations and animations. 

You can mount components in vue/app.js 

```js
Vue.component('example-component', require('./components/ExampleComponent.vue').default);
```

You can render the vue template in the following manner
```html
<example-component
    shopName="{{ shop.name }}"></example-component>
```
