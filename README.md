# gatsby-plugin-first-touch-attribution

Stores the original referrer in a cookie.

## Install

`npm install --save https://github.com/pieh/gatsby-plugin-first-touch-attribution/releases/download/1.0.0/gatsby-plugin-first-touch-attribution-v1.0.0.tgz`

## How to use

```javascript
// In your gatsby-config.js
module.exports = {
  plugins: [`gatsby-plugin-first-touch-attribution `]
};
```

## How to read the referrer

In one of your React components, you can do something like this:

```javascript
import { getOriginalReferrer } from "gatsby-plugin-first-touch-attribution ";

class Test extends React.Component {
  componentDidMount() {
    console.log(getOriginalReferrer());
  }
}
```
