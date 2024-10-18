# Free E-commerce Products API

Welcome to the **Free E-commerce Products API**! This API provides a collection of sample e-commerce product data, categorized into different product groups. You can use this data for your projects, testing, or prototyping.

## Available Endpoint

### 1. All Products

- **URL**:  
  `https://github.dev/Kolzsticks/Free-Ecommerce-Products-Api/main/products.json`

- **Description**:  
  This endpoint provides a comprehensive list of all products. You can access a wide range of categories, and for **version 1.1.0**, we have **10 products per category**. You can filter the products based on category using JavaScript array methods.

- **Available Categories**:
  1. **Electronics & Gadgets**
  2. **Fashion & Apparel**
  3. **Beauty & Personal Care**
  4. **Home & Kitchen**
  5. **Health & Fitness**

### Example: Fetching All Products Using JavaScript

```javascript
fetch('https://github.dev/Kolzsticks/Free-Ecommerce-Products-Api/main/products.json')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error fetching products:', error));
```

### Example: Filtering by Category (Fashion & Apparel)

```javascript
fetch('https://github.dev/Kolzsticks/Free-Ecommerce-Products-Api/main/products.json')
  .then(response => response.json())
  .then(data => {
    const fashionProducts = data.filter(product => product.category === "Fashion & Apparel");
    console.log(fashionProducts);
  })
  .catch(error => console.error('Error fetching products:', error));
```

### Example Product Data

```json
{
  "id": "50",
  "image": "https://kolzsticks.github.io/Free-Ecommerce-Products-Api/main/images/product/knee-pads.jpg",
  "name": "Adjustable Knee Pads",
  "rating": {
    "stars": 4.3,
    "count": 70
  },
  "priceCents": 4000,
  "category": "Health & Fitness",
  "subCategory": "Sports Gear & Accessories",
  "keywords": [
    "knee pads",
    "sports",
    "gear",
    "fitness"
  ]
}
```

## How to Use

You can easily fetch data from the API using JavaScript’s `fetch()` method or any other HTTP client like Axios, Postman, or cURL. The endpoint provides **all products** in one file, and you can filter based on the categories listed above.

### Example: Fetching by Category

You can filter the results using JavaScript `filter()` as shown above, targeting the `"category"` field to retrieve products for specific categories such as **Electronics & Gadgets**, **Fashion & Apparel**, etc.

## Notes

- **Version 1.1.0**:  
  For this version, each category contains 10 products for now. More products and categories will be added in future updates.

- **Pricing**:  
  The pricing for products is provided in `priceCents` (USD cents).

- **Images**:  
  Product images are hosted within the API and can be directly used by referencing the URLs provided in the data.

## Enjoy!

Feel free to use this API for testing, prototyping, or personal projects. It will continue to be updated with more categories, products, and features over time. Enjoy and share your feedback!

