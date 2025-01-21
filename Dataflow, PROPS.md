Em react, os dados seguem em uma única direção, do componente pai para o componente filho, seguindo o padrão de fluxo de dados unidirecional. Isso ajuda as aplicações a serem mais fáceis de debugar.

Componentes pai podem passar dados para componentes filhos usando ***PROPS***.

```

function MyComponent() {
  return (
    <div>
      <Title title='My Component' />
    </div>
  );
}

function Title({ title }) {
  return <h1>{title}</h1>;
}
```


OS ***PROPS*** são usados