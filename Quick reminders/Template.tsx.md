É um arquivo similar ao layout, que encapsula uma página. A diferença é que ele não é persistente entre a navegação de rotas, e sempre que isso acontece, seu estado é resetado e ele é renderizado novamente.

É útil em casos como:
- Funcionalidades que dependem do _useEffect (logging page views)_ 
-  Funcionalidades que dependem do _useState_.

Templates aceitam children pops.

	Quando um usuário navega entre rotas que compartilham o mesmo template, uma nova instância do componente é montada, elementos DOM são recriados, o estado não é preservado em ClientComponents e os efeitos são re-sincronizados.
	