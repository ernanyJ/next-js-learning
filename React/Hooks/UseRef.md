Uma forma de acessar partes específicas do HTML no nosso JS:

```
export default function Page(){

	const emailRef = useRef();
	const passRef = useRef();

	<form>
	<input name="email" type="email" ref={emailRef}/>
	<input name="password" type="password" ref={passRef}/>
	</form>
	
}

```

Nesse exemplo, email e pass ref são controllers que armazenam o estado, incluindo o valor que está dentro do componente input do html.