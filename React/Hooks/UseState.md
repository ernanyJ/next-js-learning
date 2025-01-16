As únicas variáveis que alteram a tela ao ser alteradas são as variáveis de estado do React.

Para criar uma variável de estado gerenciado pelo React, usamos o useState:

```
const [users, setUsers] = useState([ ]);
```

users é a variável, setUsers é o nome da função que vai alterar essa variável. Atribuímos o useState ( ) e nos parâmetros passamos o estado inicial da variável, nesse caso é uma lista vazia, mas poderia ser um inteiro (0), ou uma String vazia (" ")...

