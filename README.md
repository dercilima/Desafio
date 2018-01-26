# Desafio - O frete é mais caro que o produto? ;(

Uma grande rede de fast foods com filiais em várias cidades do país está enfrentando um problema no seu setor de delivery. Isso tem causado um atraso muito grande para informar ao cliente, no momento de efetuar o pedido, qual o valor do frete para seu bairro. Pois, em alguns casos, o valor do frete inviabiliza a efetivação do pedido.

## Regra de Negócio

***O valor do frete das entregas são calculados com base no bairro do cliente.*** Ou seja, existe uma tabela impressa de bairros da cidade com seu respectivo valor de entrega. Para os bairros mais próximos da empresa o frete é grátis, já os demais tem valores que variam de R$ 5 até R$ 15 para os mais distantes.

## Solução

Para conseguir resolver esse problema, foi proposto pelo seu gerente de projetos, o desenvolvimento de uma ferramenta que será utilizada por todas as filiais da empresa. Essa ferramenta deverá ter apenas duas funcionalidades:
- 1 - Cadastrar o valor do frete para todos os bairros (por cidade).
- 2 - E a mais importante, uma tela para consultar o valor do frete com base no **CEP** ou o **Endereço** (obrigatório ter o bairro) informado.

## Descrição técnica

- **Funcionalidade 1: CRUD**
  > Para facilitar o cadastro, o sistema deverá ter uma relação prévia dos bairros da cidade, ou seja, será necessário que você faça uma comunicação com algum Web Service de base de dados de endereços (não esquecer de verificar se a fonte de dados está sendo atualizada) e retorne apenas os bairros da cidade informada. Por exemplo, a filial de Rio Verde vai fazer o cadastro de todos os valores de frete para os bairros da cidade, então ao acessar essa tela, o sistema vai solicitar para que o usuário informe a cidade da filial, e com isso, trazer uma lista de todos os bairros de Rio Verde.
  > Obs: As várias cidades do Brasil está em constante crescimento, então, mensalmente, pode ocorrer de novos bairros serem criados.

- **Funcionalidade 2:**
	> Essa é mais tranquila :D
	> Ter duas opções: Consultar valor do frete por: CEP e Bairro.
	> Fazer a busca na base de dados de frete já cadastrado na funcionalidade 1 e exibir a informação do valor do frete com base no CEP ou Bairro informado.

## Tecnologias obrigatórias

- Framework Angular 4
- Material Angular e/ou Teradata Covalent
- Firebase Firestore (AngularFire2 e/ou API do Firebase)

## Forma de entrega

Os códigos devem ser entregues via repositório público do GitHub.

## Prazo

A implementação deverá ser entregue até **Domingo dia 03/02**.
