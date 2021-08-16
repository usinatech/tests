**

# Teste Prático - Laravel Básico
  
Esse teste prático visa avaliar os conhecimentos do programador com banco de dados MySQL, a linguagem PHP e o framework Laravel 8.

## Objetivos

-   Conhecer um pouco de suas habilidades em:
    - POO;
    - PHP;
    - Laravel;
    - MySQL;
    - Entendimento e análise dos requisitos;
    - Determinação na busca de soluções;
    - Responsabilidade na tomada de decisões.

## Fique tranquilo

-   Todo e qualquer código desenvolvido nesse teste não será utilizado em quaisquer outros softwares, nem comercializado.
-   O propósito deste teste é apenas avaliar o conhecimento em programaçao do candidato.

## Mãos ao código!

A aplicação a ser desenvolvida terá uma página inicial chamada HOME e uma área restrita denominada PAINEL acessível por login e senha.

A página HOME terá um título, subtítulo, texto em paragrafo e uma imagem da internet a livre escolha do desenvolvedor, um link para a página de login e um link para página de cadastro de novos usuários. 

A página PAINEL, acessível apenas com login e senha, dará acesso ao Dashboard contendo um menu lateral com links para Empresas, Categorias, Produtos, Permissões e Usuários. Antes de permitir acesso ao Dashboard, exiba as empresas do usuário para que ele possa escolher em qual empresa entrar.

Ao cadastrar uma Empresa, selecione os usuários que podem acessar a empresa.

Ao cadastrar uma Empresa, integre o package **CEP Webservice** da Usina Tech para preenchimento automático do endereço.  Use Ajax ou Axios para consumir o webservice.
https://github.com/usinatech/cepwebservice;

Ao cadastrar uma Categoria ou Produto, deve-se vincula-los apenas a uma Empresa.

Ao cadastrar um usuário, selecione quais empresas esse usuário terá acesso.

Os menus Empresas, Permissões e Usuários devem ser acessíveis apenas aos usuários com a permissão de Administrador.

Desenvolver MVC:
- Página Inicial (HOME)
- Página de Login do Painel
- Página de Recuperar Senha
- Página de Cadastro de Usuário
- Página do Dashboard com menu (PAINEL)
- CRUD Empresas
- CRUD Categorias
- CRUD Produtos
- CRUD Permissões
- CRUD Usuários

Desenvolver SEED:
- Empresas:
	- Loja José
	- Loja Maria
- Categorias:
	- Camisas
	- Calças
	- Bolsas
	- Óculos
- Produtos:
	- Camisa Xadrez
	- Camisa Polo
	- Calça Jeans
	- Calça de Sarja
	- Bolsa Rosa
	- Bolsa Verde
	- Óculos de Sol
	- Óculos de Esportes
- Permissões:
	-  Administrador
	- Geral
- Usuários:
	- Admin - admin@usina.tech / senha "admin"
	- Test - test@usina.tech / senha "test"
	- José - jose@usina.tech / senha "jose"
	- Maria - maria@usina.tech / senha "maria"

## Observações Importantes

Para acesso ao PAINEL, usar o middleware **Auth** nos grupos de rotas e resources para acesso a área autenticada.

Use **Validate** para validar os campos obrigatórios.

O usuário José de permissão Geral e os produtos Camisas e Calças devem estar atrelados nas categorias correspondentes na Loja José.

O usuário Maria de permissão Geral e os produtos Bolsas e Óculos devem estar atrelados nas categorias correspondentes na Loja Maria.

Os usuários admin e test devem estar atrelados nas permissões correspondentes e as Loja José e Loja Maria.