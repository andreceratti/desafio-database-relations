<p align="center">
  <img src="https://i.imgur.com/Wh3jjrl.png" alt="André Ceratti da Rocha" />
</p>

# Desafio 09: Relacionamentos com banco de dados no Node.js

## Sobre
Desafio 09 do bootcamp GoStack da Rocketseat, neste desafio foi criado um backend de uma loja, onde é possivel cadastrar novos clientes, novos produtos e serem feitas compras dos produtos.

## Como utilizar

Para usar este app devem estar instalados Node.js maquina, junto com banco de dados Postgres com banco ```gostack_desafio09``` criado e ```gostack_desafio09_teste``` caso queira rodar os testes.

Cheque o arquivo ```ormconfig.json``` e veja se as configurações batem com da sua máquina.

Se tudo estiver correto é só dar o comando:
```yarn dev:server```

## Rotas
Todas as rotas estão usando http://localhost:3333

### Create Customer [POST]
- localhost:3333/customers
JSON
```js
{
	"name": "André Ceratti da Rocha",
	"email": "andre-rocha@gmail.com"
}
```
Exemplo de envio:
JSON
```js
{
	"name": "HD 2tb Seageat",
	"price": 500.00,
	"quantity": 50
}
```
### Create Product [POST]
- localhost:3333/products
Exemplo de envio:
JSON
```js
{
	"customer_id": "6ae3e7ff-7d46-46b9-b5ca-1766b87aee2a",
	"products": [
		{
			"id": "e78cd7e7-ef67-41e2-a573-55362e98f346",
			"quantity": 5
		}
	]
}
```
### Create Order [POST]
- localhost:3333/orders
Exemplo de envio:
```
```
### Find Order [POST]
-

Sem corpo de envio
Exemplo:
```
localhost:3333/orders/640b272f-1e07-40ec-8460-ec6373d71b0b
```
