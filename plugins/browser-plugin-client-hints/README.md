# Snowplow Client Hint Tracking

[![npm version][npm-image]][npm-url]
[![License][license-image]](LICENSE)

Browser Plugin to be used with `@snowplow/browser-tracker`.

Adds Client Hints to your Snowplow tracking. Captures Navigator Client Hint data.

## Maintainer quick start

Part of the Snowplow JavaScript Tracker monorepo.  
Build with [Node.js](https://nodejs.org/en/) (12 LTS or 14 LTS) and [Rush](https://rushjs.io/).

### Setup repository

```bash
npm install -g @microsoft/rush 
git clone https://github.com/snowplow/snowplow-javascript-tracker.git
rush update
```

## Package Installation

With npm:

```bash
npm install @snowplow/browser-plugin-client-hints
```

## Usage

Initialize your tracker with the BrowserFeaturesPlugin:

```js
import { newTracker } from '@snowplow/browser-tracker';
import { ClientHintsPlugin } from '@snowplow/browser-plugin-client-hints';

newTracker('sp1', '{{collector}}', { plugins: [ ClientHintsPlugin() ] }); // Also stores reference at module level
```

## Copyright and license

Licensed and distributed under the [BSD 3-Clause License](LICENSE) ([An OSI Approved License][osi]).

Copyright (c) 2021 Snowplow Analytics Ltd, 2010 Anthon Pang.

All rights reserved.

[npm-url]: https://www.npmjs.com/package/@snowplow/browser-plugin-client-hints
[npm-image]: https://img.shields.io/npm/v/@snowplow/browser-plugin-client-hints
[docs]: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/javascript-tracker/
[osi]: https://opensource.org/licenses/BSD-3-Clause
[license-image]: https://img.shields.io/npm/l/@snowplow/browser-plugin-client-hints
