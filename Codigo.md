Num componente react, tudo começa por uma função:
```
export default function Page(){
	return (
	
	);
}
```

Nessa função, tudo que está antes do return é código JS, tudo que está depois, é html:

```
export default function Page(){

	const users = [
	{
		id: 1,
		nome: "Fulano",
		idade: 23
	},
	{
		id: 2,
		nome: "Ciclano",
		idade: 44
	}
	]

	return (
		<h1> Olá mundo! </h1>
	);
}
```

Porém, se dentro do return abrirmos chaves, podemos usar JS também:
```
export default function Page(){

	const users = [
	{
		id: 1,
		nome: "Fulano",
		idade: 23
	},
	{
		id: 2,
		nome: "Ciclano",
		idade: 44
	}
	]

	return (
		{users.map((user) => (
			<h1>Olá {user.name}</h1>
		))}
	);
}
```

Nesse caso, usamos um map para retornar um H1 contendo o nome de cada user do array declarado.

Porém nesse caso, quando usamos um map, o React pede que o desenvolver especifique uma chave única para diferenciar os itens da estrutura que estamos percorrendo. No caso de user, seria o 'id':

```
export default function Page(){

	const users = [
	{
		id: 1,
		nome: "Fulano",
		idade: 23
	},
	{
		id: 2,
		nome: "Ciclano",
		idade: 44
	}
	]

	return (
		{users.map((user) => (
			<div key={user.id}> 
			<h1>Olá {user.name}</h1>
			</div>
		))}
	);
}
```

