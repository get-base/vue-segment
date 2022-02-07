# vue-segment

> Vue.js plugin for Segment Analytics.js

[Segment Analytics.js Documentation](https://segment.com/docs/sources/website/analytics.js/)

## Setup

1. Add the `@get-base/vue-segment` dependency with `yarn` or `npm` to your project
2. Configure it:

```js
import Vue from 'vue'
import Segment from '@get-base/vue-segment'

Vue.use(Segment, {
  writeKey: 'YOUR_SEGMENT_WRITE_KEY',
  disabled: true,
  router,
  pageCategory: 'shop',
  settings: {
    ...
  }
})
```

## Usage

See [Segment Vue Quickstart Guide](https://github.com/segmentio/analytics-vue#how-to-get-started).

## Options

### writeKey

- Type: `String`
  - Default: `''`

### disabled

Disable automatic script loading, if you need compliance with GDPR.

- Type: `Boolean`
  - Default: `false`

### router

Call `analytics.page` method on `afterEach` router method if provided.

- Type: `Object`

### pageCategory

In case you provided router, you can specify the category page of the `page` event. See segment [page](https://segment.com/docs/sources/website/analytics.js/#page) method reference.

- Type: `String`,
  - Default: `''`

### settings

See [Load options](https://segment.com/docs/sources/website/analytics.js/#load-options) reference.

- Type: `Object`

## Development

1. Clone this repository
2. Install dependencies using `yarn install` or `npm install`
3. Start development server using `npm run dev`

## License

[MIT License](./LICENSE.md)

