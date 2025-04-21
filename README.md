# Sistema de E-commerce de Produtos Naturais
Este é um sistema de loja eletronica (e-commerce) de produos naturais, onde um cliente pode manter um carrinho de compras
 com os produtos naturais, o cliente pode manter um carrinho de compras com os produtos que ele adicionar duratente a navegação.
Também, pode consultar produtos no site e rastrear pedidos já realizados anteriormente. O cliente também pode manter uma comprassendo realizada ou finalizá-la.
 Para efetuar essas ações, o cliente deve efetuar login.

# Diagrama de Caso de Uso - Sistema de E-commerce de Produtos Naturais
```mermaid
usecaseDiagram
  actor Cliente

  Cliente --> (Efetuar login)
  Cliente --> (Consultar produtos)
  Cliente --> (Rastrear pedido)
  Cliente --> (Manter carrinho de compra)
  Cliente --> (Finalizar compra)
  Cliente --> (Manter compra)

  (Manter carrinho de compra) --> (Consultar produtos) : <<include>>
  (Manter carrinho de compra) --> (Efetuar login) : <<include>>
  (Manter compra) --|> (Efetuar login) : <<extend>>
```
