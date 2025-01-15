O arquivo layout.tsx é o primeiro a ser chamado ao iniciar a aplicação.
Ele acomoda todos os nossos componentes e páginas dentro do seu corpo.

Por isso é interessante para que componentes que serão padrões em todo o projeto, sejam declarados aqui, como headers, asides e rodapés.

## Layouts aninhados

Dentro das nossas rotas, por exemplo _app/products/[productid]_
Podemos colocar um arquivo _layout.tsx_ (Tem que ter exatamente esse nome.)
Dessa forma, ele também irá abrigar e se tornar padrão para todos os filhos subsequentes e podemos ter layouts específicos para cada rota.


