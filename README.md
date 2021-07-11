# ajv-currency-code

Adds a `currency_code` format to [Ajv](https://ajv.js.org).

## Install

```bash
npm i --save @socketkit/ajv-currency-code
```

## Setup

```javascript
import Ajv from 'ajv'
import currenyCode from '@socketkit/ajv-currency-code'
const ajv = new Ajv()
currencyCode(ajv)
```

## Usage

When defining your JSON schema, use the `format` keyword with ther value set to `currency_code`. For example

```json
{
  "type": "object",
  "properties": {
    "currency": {
      "type": "string",
      "format": "currency_code"
    }
  }
}
```
