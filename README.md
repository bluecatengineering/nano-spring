# @bluecateng/nano-spring [![GitHub license](https://img.shields.io/badge/license-ISC-blue.svg)](https://github.com/bluecatengineering/nano-spring/blob/master/LICENSE.md) [![npm version](https://img.shields.io/npm/v/@bluecateng/nano-spring.svg?style=flat)](https://www.npmjs.com/package/@bluecateng/nano-spring) [![CircleCI](https://circleci.com/gh/bluecatengineering/nano-spring.svg?style=shield)](https://circleci.com/gh/bluecatengineering/nano-spring)

Tiny implementation of spring animation with mass set to 1.

Size: 290 bytes before compression.

# Installation

npm i -S @bluecateng/nano-spring

# Example

```js
import spring from '@bluecateng/nano-spring';

const element = document.querySelector('#test');
element.style.opacity = .5;
spring(250, 30,
  (p) => element.style.transform = `translateX(${p * 300}px)`,
  () => element.style.opacity = '');
```

## Output
![Output](https://raw.githubusercontent.com/bluecatengineering/nano-spring/master/example.gif)
