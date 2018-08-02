# gatsby-plugin-first-touch-attribution

Stores the original referrer in a cookie.

## Install

`npm install --save gatsby-plugin-first-touch-attribution`

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
