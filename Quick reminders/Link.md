
O componente link do 'next/link' nos permite navegar entre rotas

```
iport Link from 'next/link'

export default function Home(){
	return (
	<Link href={'/products'}>Ir para produtos</Link>
		)
}
```

Existe como checar a rota ativa no momento para alterar nossa tela usando a função _usePathname_:

```

const path = usePathname();

const isActive = path.startsWith('produto');
<p className = {`isActive ? text-red : text-blue`}> produtos </p>

```


Nesse caso, estamos usando a função para saber se estamos na rota produtos e alterar a cor do texto de um componente com base nessa informação.

Porém, usamos uma informação que só está disponível no navegador do cliente, que é a rota do navegador atual. Nesse caso, teremos que fazer um [Client Side Rendering Component](CSR%20-%20Client%20Side%20Rendering.md (Client Side Rendering)) 