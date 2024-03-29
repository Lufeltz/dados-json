## Dados para teste json-server

```
git clone https://github.com/Lufeltz/dados-json.git
```

```
cd dados-json
```

```
npm install
```

### Exemplo de uso

```
json-server --watch dados.json
```

#### Resposta esperada

```
json-server --watch .\dados.json

--watch/-w can be omitted, JSON Server 1+ watches for file changes by default
JSON Server started on PORT :3000
Press CTRL-C to stop
Watching .\dados.json...

( ˶ˆ ᗜ ˆ˵ )

Index:
http://localhost:3000/

Static files:
Serving ./public directory if it exists

Endpoints:
http://localhost:3000/clientes
http://localhost:3000/funcionarios
http://localhost:3000/pedidos
http://localhost:3000/orcamentos
```

#### Se apareceu a resposta acima tudo certo pode ir testar, caso contrário use o comando a seguir e execute o json-server novamente:

```
npm install -g json-server
```

#### URL base para acesso no navegador: http://localhost:3000

### Endpoints

- /clientes
- /funcionarios
- /pedidos
- /orcamentos

#### Requisição

```
http://localhost:3000/clientes
```

#### Resposta

```
[
	{
		"id": "1",
		"cpf": "12345678900",
		"nome": "Carlos Ribeiro",
		"email": "carlos@gmail.com",
		"endereco": "Rua Das Flores, n 15",
		"telefone": "41 991235652",
		"funcionario": false
	},
	{
		"id": "2",
		"cpf": "94857683456",
		"nome": "Antonio Roberto",
		"email": "antonio@gmail.com",
		"endereco": "Alameda Dos Anjos, n 3000",
		"telefone": "31 925415263",
		"funcionario": false
	},
	{
		"id": "3",
		"cpf": "35241526451",
		"nome": "Rosa Nunes",
		"email": "rosa@gmail.com",
		"endereco": "Avenida Brasil, n 1560",
		"telefone": "22 991235652",
		"funcionario": false
	},
	{
		"id": "4",
		"cpf": "21425165238",
		"nome": "Renata Gonçalves",
		"email": "renata@gmail.com",
		"endereco": "Rua dos voluntários, n 324",
		"telefone": "11 912345162",
		"funcionario": false
	},
	{
		"id": "5",
		"cpf": "36956856265",
		"nome": "Rogerio Cardoso",
		"email": "rogerio@gmail.com",
		"endereco": "Alameda João Batista, n 624",
		"telefone": "54 936522352",
		"funcionario": false
	}
]
```

#### Requisição

```
http://localhost:3000/clientes/1
```

#### Resposta

```
{
	"id": "1",
	"cpf": "12345678900",
	"nome": "Carlos Ribeiro",
	"email": "carlos@gmail.com",
	"endereco": "Rua Das Flores, n 15",
	"telefone": "41 991235652",
	"funcionario": false
}
```
