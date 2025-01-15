São os meta dados que podemos definir na aplicação.
Existe um objeto Metadata:

```
export const metadata: Metadata = {
 title: {
	absolute: '',
	default: '',
	template: ''
 }
 description: 'Generated by create next app'

}
```

Podemos definir os metadados padrões em _/app/page.tsx_, mas também podemos definir metadados específicos para cada página, por exemplo:

	/app/products/[id]/page.tsx
```

export const metadata Metadata = {
	title: "Nome do produto"
}

export default function Products(){
	return (
	<div>
	<p> Teste </p>
	</div>
	)
}

```