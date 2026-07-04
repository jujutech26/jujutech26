# REST 

REST एउटा API architecture (architectural style) हो, जुन पहिलो पटक Roy Fielding ले आफ्नो Ph.D. thesis मा प्रस्ताव गरेका थिए।

REST अर्थात् REpresentational State Transfer भनेको HTTP Protocol माथि API डिजाइन गर्ने एउटा architectural style हो।

REST ले Client–Server Architecture अपनाउँछ। 

- Client → Request पठाउँछ।
- Server → Request Process गरेर Response पठाउँछ।

अब REST का केही मुख्य सिद्धान्तहरू:

## 1. Stateless

RESTful API stateless हुन्छ।

Stateless भनेको प्रत्येक request/response pair अघिल्लो request बाट पूर्ण रूपमा स्वतन्त्र हुन्छ।

सर्भरले अघिल्ला requests हरू सम्झँदैन।

## 2. Resources

REST मा resources (स्रोतहरू) को concept हुन्छ।

User, Order, Product, Shopping Cart आदि resources का उदाहरण हुन्।

यी resources लाई URLs ले represent गर्छन्।

उदाहरण:
- /users
- /products
- /orders/123

## 3. HTTP Methods

REST API मा client ले resources सँग HTTP methods प्रयोग गरेर interact गर्छ।

- GET → Read
- POST → Create
- PUT → Update
- DELETE → Delete

यी methods लाई CRUD (Create, Read, Update, Delete) operations सँग map गर्न सकिन्छ।

## 4. Representation

Server ले request process गरेपछि resource को representation response मा फर्काउँछ।

आजकल यो representation प्रायः JSON format मा हुन्छ।

## References:
- Django for APIs by William S. Vincent
- https://blog.algomaster.io/p/rest-vs-graphql
- https://www.geeksforgeeks.org/node-js/rest-api-introduction/