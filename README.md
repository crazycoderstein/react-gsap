# react-gsap

> React components for GSAP

[![NPM](https://img.shields.io/npm/v/react-gsap.svg)](https://www.npmjs.com/package/react-gsap) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save react-gsap
```

## Usage

```jsx
import React, { Component, Fragment } from 'react';

import { Tween, Timeline } from 'react-gsap';

class Example extends Component {
  render () {
    return (
      <div>
        <Tween from={{ x: '100px', rotation: -360 }}>
          <div>This element gets tweened</div>
          <div>This, too</div>
        </Tween>

        <Timeline
          target={
            <Fragment>
              <div>Target element which will be visible and gets tweened</div>
              <div>Another target element</div>
            </Fragment>
          }
        >
          <Tween from={{ opacity: 0 }} to={{ opacity: 1 }} />
          <Tween to={{ x: '50px' }} />
        </Timeline>
      </div>
    )
  }
}
```

## Examples

https://bitworking.github.io/react-gsap/

https://github.com/bitworking/react-gsap/tree/master/example/src/components

##### You can play with these examples at StackBlitz.io. Because learning by doing is the King:

[Tween](https://stackblitz.com/edit/react-gmmwqj)

[Timeline](https://stackblitz.com/edit/react-ambemn)

[Svg](https://stackblitz.com/edit/react-23bsde)

[Transition](https://stackblitz.com/edit/react-v61on3)


## License

MIT © [bitworking](https://github.com/bitworking)
