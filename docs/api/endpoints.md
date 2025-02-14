# API Endpoints

## Products

### List Products
```http
GET /api/v1/products
```

### Get Product
```http
GET /api/v1/products/{id}
```

### Search Products
```http
GET /api/v1/products/search?q={query}
```

## Shopping Lists

### List All Lists
```http
GET /api/v1/lists
```

### Create List
```http
POST /api/v1/lists
```

### Update List
```http
PUT /api/v1/lists/{id}
```

## Price Tracking

### Get Price History
```http
GET /api/v1/products/{id}/prices
```

### Set Price Alert
```http
POST /api/v1/price-alerts
```

## Response Format

All API responses follow this format:

```json
{
  "status": "success",
  "data": {
    // Response data here
  },
  "meta": {
    "page": 1,
    "per_page": 20,
    "total": 100
  }
}
``` 