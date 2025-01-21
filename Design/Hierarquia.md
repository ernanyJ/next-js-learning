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

### BALANÇO ENTRE WEIGHT E CONSTRASTE 

A razão pela qual textos bold chamam mais atenção que os normais é porque ele ocupa mais pixels na tela. Isso tem efeitos em outras coisas além de texto.

Ícones geralmente são bem "pesados" visualmente e cobrem bastante área da interface. Quando você coloca um ícone do lado de um texto, o ícone costuma ficar enfatizado 

![[Pasted image 20250121142629.png]]

Diferente do texto, não temos como diminuir o peso de um ícone. Uma forma simples de balancear a hierarquia desses elementos é brincando com as cores:

![[Pasted image 20250121142701.png]]


Isso funciona muito bem pra balancear elementos que tem diferentes pesos (weight). Reduzir o contraste funciona como um contrabalanço, fazendo elementos mais pesados parecerem mais leves mesmo que o weight não tenha sido alterado.

O contrário também funciona. Quando precisamos aumentar a enfatização de um elemento sutil, como aquelas pequenas bordas de 1px, caso aumentemos o contraste dessa borda, o efeito fica barulhento e sujo:

![[Pasted image 20250121143004.png]]



Nesses casos, uma boa solução seria aumentar o peso:

![[Pasted image 20250121143023.png]]

Deixamos a borda um pouco mais pesada sem perder o toque suave que ela deve ter.

## Semantics são secundárias

Quando há múltiplas ações que um usuário pode tomar, é comum cair na armadilha de desenhar aquelas ações baseadas puramente em semânticas:
![[Pasted image 20250121143202.png]]

Semânticas são uma parte importante do design de botoões, mas isso nã́o significa que você deve esquecer a hierarquia.

Todos os elementos numa UI estão numa pirâmide de importância. Na maioria dos casos, uma parte de uma UI tem apenas uma única ação principal, uma ou outra ação secundária menos importante, e uma ação terciária, quase esquecida e/ou não utilizada. 

Quando desenhamos essas ações, é importante comunicar seus lugares na hierarquia.

- Botões primários devem ser óbvios. Sólidos, background com cores com alto contraste.
- Botões secundários devem ser clean, mas não proeminentes. Outlined styles ou fundos com menos contraste são boas opções para estes.
- Botões terciários devem ser descobríveis, mas não intrusivos. Estilizar esses botões como links são geralmente a melhor abordagem.
- 
![[Pasted image 20250121143641.png]]

Quando tomamos uma abordagem priorizando a hierarquia pra desenhar as ações de uma parte da nossa UI, o resultado é uma interface muito mais clean, sem pesar a vista  e que tem uma comunicação mais clean

![[Pasted image 20250121143815.png]]


### DESTRUCTIVE ACTIONS

Uma ação destrutiva não significa que o botão deve ser grande, pesado e vermelho.

Se uma ação destrutiva não é a ação primária de uma tela, é melhor aplicar um estilo secundário ou terciário.

![[Pasted image 20250121143948.png]]

Combine isso com um dialog de confirmação onde a ação destrutiva realmente é a ação primária, e aplique o estilo grande, pesado e vermelho de fato.

![[Pasted image 20250121144048.png]]

