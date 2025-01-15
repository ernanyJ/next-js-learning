**Navegação**
O next funciona através de Nested routes pelas pastas do projeto

Tem como criar rotas dinâmicas colocando o nome da pasta entre colchetes [ assim ]

Tem como passar parâmetros para as páginas:

	/app/info/page.tsx
```
export default function Page( {params} ){
	return <h1> Página {params.nome} </h1>
}
```
	
	
	/app/about/about.tsx
	
```
	import Page from @/info/page.tsx;

	export default function About(){
		return ( 
		<> 
			<Page nome="Sobre"/>
		</>
		);
	}
```


Desse jeito, page.tsx iria exibir uma headline h1 com o texto "Página sobre", 'sobre' foi passado como parâmetro a partir de about.

Do jeito atual, teríamos um aviso em tempo de compilação falando que params é do tipo _any_. Isso se deve ao Typescript estar nos avisando para tipar essa varíavel. Podemos fazer da seguinte maneira:

```
interface PageParams{
	params: {
		nome: string
	}
}

export default function Page( {params}: PageParams ){
	return <h1> Página {params.nome} </h1>
}
```

pronto. Agora 'params' é tipado e teremos checagem de tipos em tempo de compilação.