# Getting Started
Install the dependencies and run the project
```
npm install
npm start
```

Head over to https://vitejs.dev/ to learn more about configuring vite
## About Scrimba

At Scrimba our goal is to create the best possible coding school at the cost of a gym membership! 💜
If we succeed with this, it will give anyone who wants to become a software developer a realistic shot at succeeding, regardless of where they live and the size of their wallets 🎉
The Fullstack Developer Path aims to teach you everything you need to become a Junior Developer, or you could take a deep-dive with one of our advanced courses 🚀

- [Our courses](https://scrimba.com/courses)
- [The Frontend Career Path](https://scrimba.com/fullstack-path-c0fullstack)
- [Become a Scrimba Pro member](https://scrimba.com/pricing)

Happy Coding!

1. What is a route/url parameter?
A route parameter (or URL parameter) is a dynamic part of the URL that lets you capture values from the URL and use them in your component.

For example, in this URL:


/products/42
If your route is defined as:

<Route path="/products/:productId" element={<ProductDetail />} />
Then :productId is a route parameter, and in this case, its value would be "42".

You can access it using the useParams() hook from react-router-dom.

------------
2. Add a route parameter called `productId` to the Route path below:


<Route path="/products/:productId" element={<ProductDetail />} />


------------
3. Add whatever you need to add for the component below to display
   the route parameter in the <h1>

import { useParams } from "react-router-dom"
function ProductDetail() {
    const params = useParams()
    return <h1>Product ID: {params.productId}</h1>
}
