# Shop-Stripe
A Fullstack E-commerce website where users can view products, add products to their cart and checkout with stripe.

## Deployed Link
https://shop-stripe-mehdi.herokuapp.com/

## Screenshot Of Website
![ezgif com-gif-maker](https://user-images.githubusercontent.com/75599021/144123218-81201d81-671e-4232-8263-acc9e41775ad.gif)

## Built With
* [Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
* [Node.js](https://nodejs.org/en/docs/)
* [NPM-Library](https://docs.npmjs.com/)
* [Expres.js](https://expressjs.com/)
* [React.js](https://reactjs.org/)
* [Apollo](https://www.apollographql.com/)
* [Stripe](https://stripe.com/en-gb-us)

## Installation Steps For Local Running
1. Clone project.
2. Open terminal within the directory and run these commands in order
    - npm install
    - cd server
    - npm run seed
    - cd ..
    - npm run develop

## Code Snippet Of Order Model 
```javascript
const mongoose = require('mongoose');

const { Schema } = mongoose;

const orderSchema = new Schema({
  purchaseDate: {
    type: Date,
    default: Date.now
  },
  products: [
    {
      type: Schema.Types.ObjectId,
      ref: 'Product'
    }
  ]
});
```

## Author

* **Mehdi Safari**

- [Link to Portfolio Site](https://mehdisafari77.github.io/Basic-Bio/)
- [Link to Github](https://github.com/mehdisafari77)
- [Link to LinkedIn](https://www.linkedin.com/in/mehdi-safari-992799142/)
