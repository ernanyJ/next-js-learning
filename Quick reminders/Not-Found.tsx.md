Importando notFound do navigation do next, tem como controlar e enviar o usuário para a página padrão de rotas não definidas dentro do código, por exemplo ao entrar numa página e buscar um id que não existe no banco, retornar notFound

	import { notFound } from 'next/navigation'

		if(check){
			notFound();
		}

_Inclusive, essa função primeiro tenta buscar um notFound no diretório mais próximo de onde ela foi importada, para casos de páginas de notFound personalizadas:_

Por exemplo, na rota
/products/reviews/page.tsx

Caso redirecionarmos para um notFound, primeiro o  Next buscaria um arquivo not-found.tsx em _reviews_, depois em _products_, e caso não achasse algum arquivo personalizado (por exemplo, ao invés de só mostrar "essa página não existe", mostrar "Produto não cadastro", ou "Review não existe"), ele pegaria o not-found.tsx da pasta /app, que caso não exista, será usado o padrão do Next.