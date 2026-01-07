---
title: MARTA.js
status: complete
partner: MARTA
tech:
  - JavaScript
  - TypeScript
  - npm
github: https://github.com/CivicTechAtlanta/marta-js
featured: false
---

JavaScript library wrapper for MARTA's Realtime APIs, making it easy for developers to build transit applications. Provides simple methods to fetch bus and rail arrival times from Atlanta's public transit system.

## Features

- Real-time bus arrival information
- Real-time rail arrival information
- Available as npm package
- TypeScript support

## Usage

```javascript
const marta = require('marta-js');
marta.rail.getArrivals().then(arrivals => {
  console.log(arrivals);
});
```
