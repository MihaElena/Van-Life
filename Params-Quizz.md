
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
   the route parameter in the <p>

import { useParams } from "react-router-dom"
function ProductDetail() {
    const params = useParams()
    return <p>Product ID: {params.productId}</p>
}
