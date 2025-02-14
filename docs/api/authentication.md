# API Authentication

## Overview

Grocery Gooose uses OAuth 2.0 for API authentication. This guide explains how to authenticate your requests to our API.

## Getting Started

### 1. Register Your Application
Visit the [Developer Portal](https://developer.grocerygooose.com) to:
- Create a developer account
- Register your application
- Get your API credentials

### 2. Authentication Methods

We support multiple authentication methods:

#### OAuth 2.0
```bash
POST /oauth/token
Content-Type: application/x-www-form-urlencoded

grant_type=client_credentials
&client_id=YOUR_CLIENT_ID
&client_secret=YOUR_CLIENT_SECRET
```

#### API Keys
```bash
GET /api/v1/products
Authorization: Bearer YOUR_API_KEY
```

## Security Best Practices

- Never share your API keys
- Rotate keys regularly
- Use environment variables
- Implement rate limiting
- Monitor API usage

## Error Handling

| Error Code | Description |
|------------|-------------|
| 401 | Invalid credentials |
| 403 | Insufficient permissions |
| 429 | Rate limit exceeded 