# Boas Práticas com Laravel

Siga também [PSR-2: Coding Style Guide](https://www.php-fig.org/psr/psr-2/)

| ?              | como              | exemplo                       | não faça                        |
| -------------- | ----------------- | ----------------------------- | ------------------------------- |
| Controller     | singular          | ProductController             | ~~ProductsController~~          |
| Model          | singular          | Product                       | ~~Products~~                    |
| Views          | snake_case        | product_attributes.blade.php  | ~~ProductAttributes.blade.php~~ |
| Views folder¹  | plural            | products                      | ~~product~~                     |
| Métodos        | camelCase         | getPrice                      | ~~get_price~~                   |
| Rotas          | plural            | produtos                      | ~~produto~~                     |
| Nomes de Rotas | snake_case com .  | users.products.index          | ~~user.product_index~~          |
| Tabelas        | snake_case plural | products, product_attributes  | ~~product~~                     |
| Variáveis      | camelCase         | $products, $productAttributes | ~~\$product_attributes~~        |
| Tabela pivot   | singular, plural  | product_attributes            | ~~product_attribute~~           |

1 - Pastas para _admin_ e _user_ ficam no singular.

## Comentários
- Insira o propósito do método
- Insira a rota do método
- Dê uma linha de espaço
- Coloce os parâmetros aceitos com o tipo de dado dele(ex. string, int, bool, char...) e o nome da variável
- Dê um espaço de linha
- Insira o retorno com o tipo do que é retornado

```php
/**
 * Here comes my method description
 * /this-is-my-route
 *
 * @param string $name
 * @param string $email
 * @param int $age
 *
 * @return boolean
 */
```
