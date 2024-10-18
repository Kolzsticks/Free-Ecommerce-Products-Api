# Free E-commerce Products API

Welcome to the **Free E-commerce Products API**! This API provides a collection of sample e-commerce product data, including a general product catalog and a specific set of clothing brands. You can use this data for your projects, testing, or prototyping.

## Available Endpoints

### 1. All Products

- **URL**:  
  `https://kolzsticks.github.io/Free-Ecommerce-Products-Api/main/products.json`

- **Description**:  
  This endpoint provides a list of 26 sample products from various categories, including clothing, accessories, and household items.

- **Example Product Data**:
  ```json
  [
    {
      "id": "e43638ce-6aa0-4b85-b27f-e1d07eb678c6",
      "image": "https://kolzsticks.github.io/Free-Ecommerce-Products-Api/main/images/product/athletic-cotton-socks-6-pairs.jpg",
      "name": "Black and Gray Athletic Cotton Socks - 6 Pairs",
      "rating": {
        "stars": 4.5,
        "count": 87
      },
      "priceCents": 1090,
      "keywords": [
        "socks",
        "sports",
        "apparel"
      ]
    }
  ]
  ```

### 2. Clothing Brands

- **URL**:  
  `https://kolzsticks.github.io/Free-Ecommerce-Products-Api/clothe_brands`

- **Description**:  
  This endpoint specifically provides data on clothing brands with around 8 items.

- **Example Product Data**:
  ```json
  [
    {
      "id": "e43638ce-6aa0-4b85-b27f-e1d07eb678c6",
      "image": "https://kolzsticks.github.io/Free-Ecommerce-Products-Api/clothe_brands/img/campaign-men.jpg",
      "name": "Men outfit",
      "rating": {
        "stars": 4.5,
        "count": 87
      },
      "priceCents": 1090,
      "keywords": [
        "socks",
        "sports",
        "apparel"
      ]
    }
  ]
  ```

## How to Use

You can easily fetch data from the API using JavaScript’s `fetch()` method or any other HTTP client like Axios, Postman, or cURL.

### Example: Fetching All Products Using JavaScript

```javascript
fetch('https://kolzsticks.github.io/Free-Ecommerce-Products-Api/main/products.json')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error fetching products:', error));
```

### Example: Fetching Clothing Brands Using JavaScript

```javascript
fetch('https://kolzsticks.github.io/Free-Ecommerce-Products-Api/clothe_brands/products.json')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error fetching clothing brands:', error));
```

## Notes

- **Data Limitations**:  
  Currently, the API is limited to 26 products for the main catalog and 8 items for the clothing brands. This may be updated in the future.

- **Pricing**:  
  The pricing for products is provided in `priceCents` (USD cents).

- **Images**:  
  Product images are hosted within the API and can be directly used by referencing the URLs provided in the data.

## Enjoy!

Feel free to use this API for testing, prototyping, or personal projects. I will continue updating it over time to add more items and features. Have fun!
