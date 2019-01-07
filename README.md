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
