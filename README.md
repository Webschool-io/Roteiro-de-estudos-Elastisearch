# Roteiro de estudos Elastisearch

Vamos estudar sa porra forteee!

Inicialmente vamos definir qual modelo de dados utilizaremos para nossos testes.

## Modelo de dados

Vamos pegar como base um modelo de produto para ecommerce, bem básico:

```js
{
  name: String,
  sku: String,
  description: String,
  price: {
    value: Number,
    currency: String
  },
  characteristics: [
    {
      name: String, // width
      value: Number, // 200
      unit: String // g
    }
  ],
  tags: [
    String
  ],
  created_at: Date,
  updated_at: Date,
}
```

## Índices

Agora precisamos escolher quais desses dados serão índices no ElastiSearch.

- name
- description ?
- characteristics
- tags
