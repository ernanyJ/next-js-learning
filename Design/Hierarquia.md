Nem todos os elementos são iguais

_Hierarquia visual_ se refere ao qual importante os elementos da sua interface parecem ser em relação aos outros. É a ferramenta mais importante que você tem para fazer algo parecer "designed".

Quando tudo numa interface está competindo por atenção, as coisas se tornam barulhentas e caóticas, como uma grande parede de conteúdo onde não está claro oque realmente importa:

![[Pasted image 20250121103058.png]]

Quando você deliberadamente enfatiza informações secundárias e terciárias e faz um esforço para destacar elementos que são mais importantes, o resultado é imediatamente mais satisfatório, mesmo que o layout, cores e fontes não tenham mudado

![[Pasted image 20250121103217.png]]


## Como aplicar hierarquia?

### 1. Tamanho não é tudo:

Depender muito no tamanho da fonte para definir sua hierarquia é um erro. Isso frequentemente faz com que o conteúdo primário seja muito largo, e o conteúdo secundário seja muito estreito

![[Pasted image 20250121103653.png]]

Use outros elementos para fazer o mesmo trabalho, como font-weight ou color.
Por exemplo, usar uma fonte bold para fazer um elemento primário se destacar permite que você use um tamanho de fonte mais razoável, e geralmente comunica melhor o destaque que você quer passar:

![[Pasted image 20250121103911.png]]

Da mesma forma, usar uma cor mais suave pra apoiar a hierarquia ao invés de apenas um tamanho menor faz as coisas parecerem mais clean sem sacrificar a legibilidade.

Tente se manter em três cores:

- *Uma cor escura* para conteúdo primário (como a headline de um artigo)
- *Uma cor acinzentada* para conteúdo secundário (como a data que um artigo foi publicado)
- *Uma cor acinzentada mais clara* para conteúdo terciário (talvez as diretrizes de copyright no footer do artigo.)

E geralmente, apenas dois pesos de fontes são suficientes para sua UI funcionar:

- Um font-weight normal (400 ou 500 dependendo da fonte) para a maioria dos textos
- Um font-weight mais pesado (600 ou 700) para o texto que você quer enfatizar

![[Pasted image 20250121110045.png]]

### Não use  textos acinzentados em fundos coloridos
Fazer um texto cinza claro é uma boa maneira de desenfatizá-lo em fundos brancos, mas não fica bom em fundos coloridos

![[Pasted image 20250121110255.png]]

Isso acontece porque o efeito que estamos aplicando com cinza no branco é o _reduced contrast_. Fazer um texto estar mais próximo da cor de fundo é oque realmente ajuda a criar hierarquia, não fazer ele cinza claro.

![[Pasted image 20250121110603.png]]

Para fazer dar certo, escolha uma cor a mão (e não apenas diminua a opacidade) baseada na cor de fundo. Escolha uma cor com o mesmo hue, ajuste a saturação e brilho até parecer bom.

![[Pasted image 20250121110725.png]]

### Desenfatizar para enfatizar

As vezes você vai se deparar com situações onde apenas enfatizar um elemento não o destaca o suficiente:
![[Pasted image 20250121110902.png]]

Ao invés de tentar enfatizá-lo mais, tente desenfatizar os elementos que estão competindo com ele:

![[Pasted image 20250121110944.png]]

Nesse exemplo, é possível fazer isso dando uma cor mais suave ao itens que não são o foco.


Isso é aplicável para pedaços maiores do layout também.

No exemplo abaixo, a sidebar parece estar competindo com a área do conteúdo principal. A solução foi tirar a cor de fundo e deixar o conteúdo diretamente no background:

![[Pasted image 20250121111114.png]]

### Labels são o último recurso

Quando apresentando dados para um usuário, é comum cair na armadilha de mostrar usando um formato label: valor

![[Pasted image 20250121111505.png]]

O problema dessa abordagem é que é difícil de apresentar qualquer tipo de hierarquia, pois todos os dados estão tendo a mesma ênfase.

Talvez você não precise de uma label. Em grande parte das situações, você pode dizer oque um dado é apenas olhando o formato.

xxxxx@xxxx.com -> email
(xx) xxxx-xxxx -> telefone
R$ 00,00 -> preço

Quando o formato não é suficiente, o contexto geralmente é.
Quando você vê a frase "Assistente de cliente" de baixo de um nome numa parte de "listar funcionários", você não precisa de uma label para fazer a conexão de que aquele é o departamento que aquela pessoa trabalha:

![[Pasted image 20250121111901.png]]


Até quando algum dado não é completamente entendível sem uma label, você pode geralmente evitar uma label adicionando um texto  esclarecendo.

Por exemplo, ao invés de mostrar "In stock: 12", use "'12 left in stock":
![[Pasted image 20250121114234.png]]

Algo como Quartos: 3 pode simplesmente virar 3 Quartos
![[Pasted image 20250121114425.png]]

### Labels são secundárias.

As vezes você realmente precisa de uma label, por exemplo quando você está exibindo múltiplos dados parecidos e eles precisam ser facilmente escaneáveis, como num dashboard.

Nesse caso, adicione a label, mas trate-a como um suporte do conteúdo. O dado em si é oque realmente importa. A label só está lá para fins de clareza.

![[Pasted image 20250121115610.png]]

Desenfatize a label fazendo ela parecer menor, reduzindo o contraste ou usando um peso menor na fonte. 

### Quando enfatizar uma label?

Se você está fazendo o design de uma interface que você sabe que o usuário vai estar _procurando_ por aquela label, faz sentido enfatizar a label ao invés do dado.

Isso é frequentemente o caso em páginas que são muito densas de informação, como as especificações técnicas de um produto.

Se o usuário está procurando pelas dimensões da página, ele provavelmente está escaneando a pagina procurando palavras como "profundidade", e não "7.6mm"

![[Pasted image 20250121115934.png]]

Não desenfatize muito o dado nesses cenários. Ainda é uma informação importante. Apenas use uma cor mais escura para a label e uma _um pouco_ mais clara para o valor.