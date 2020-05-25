# iHealthFood
É um projeto de plataforma de negócio digital multilateral, envolve B2C e B2B, aberto, para demonstrar como desenvolver uma solução de delivery exclusiva para pessoas que possuem intolerância a glúten e lactose, baseado em experiências e fatos reais. Neste projeto enfatizamos a **Jornada de Análise de Negócio** aplicada a **Gestão de Requisitos de Software** com objetivo de construir software de valor.

![](http://www.etecnologia.com.br/images/fars/banner-ihealthfood.png)

# Visão do iHealthFood
**Para pessoas que tem intolerância a glúten e/ou lactose o iHealthFood é um serviço de entrega exclusivo através de aplicativo móvel e web, intuitivo, seguro e fácil de usar que oferece a possibilidade de encontrar os melhores restaurantes que fornecem comidas e pratos deliciosos sem glúten e sem lactose.Diferente de outros, nosso serviço é dedicado para clientes que se necessitam comprar alimentos sem glúten e sem lactose.**

# Desafios de Análise de Requisitos de Software:
**Objetivo primário dos Desafios é especificar todos os requisitos de software que farão partes das próximas Sprints.** 

O trabalho do Analista de Requisitos começa no momento que os artefatos: Visão e Backlog do Serviço estão prontos, geralmente este trabalho acontece em um Workshop de Requisitos para descobrir os requisitos, entender as pessoas, entender o negócio e especificar os requisitos. 
O workshop deve ser colaborativo, ou seja, participam o Dono de Negócio, Desenvolvedores e Testadores de forma ativa.

Contudo, aqui você trabalhará sozinho, isso é comum em algumas empresas, existe a opção de chamar seus amigos para ajuda-lo, antes
de fazer os desafios leia e entenda a visão do serviço e o Backlog, eles estão na pasta de __Produto__:
- **Visão do Serviço**: A visão, escopo do serviço, mostra de forma clara para quem é destinado o serviço, quais são as caracteristicas-chave e diferenciais de mercado. 
- **Backlog do Serviço**: Lista com tudo que é necessário para desenvolvimento do serviço (iHealthFood). O Backlog é o principal artefato para especificar os requisitos.

Recomendamos a leitura dos arefatos de negócio devem ser lidos e compreendidos, eles estão na pasta __Negócio__ isso ajuda no entendimento dos requisitos, são eles:
- **Business Story**: Declaração do Problema 
- **Modelo de Negócio**: Mostra a lógica de negócio e como será gerado valor com iHealthFood
- **Business Value**: Demonstra qual é valor de negócio que o iHealthFood deverá gerar.
- **Mapa de Fluxo de Valor**: Mostra quais as atividades devem ser feitas para garantir a geração de valor
- **Regras de Negócio**: Apresenta todas as regras de negócio que devem ser aplicadas ao iHealthFood

Para que você exercite suas habilidades de Análise de Requisitos de Software propomos 5 desafios 
apresentados abaixo:

**Desafio-1 – Identificação dos itens do Backlog que devem ser especificados. Leve em consideração o nível de prioridade dos itens:**
- Definir quais itens do Backlog de Serviço devem ser especificados.  

**Desafio-2 – Histórias do Usuário:** 
- Escrever as histórias do usuário. 
<template>
Como [persona] posso [ação]
para fazer meu [valor].

Exemplo:
“Como cliente posso fazer _login_ com e-mail e senha para fazer meu pedido.”

**Desafio-3 - Especificação de Requisitos (baseada em US e BDD):**<BR>
- Fazer a especificação dos requisitos <BR>
<template> Estrutura de escrita dos cenários:<BR>

Funcionalidade: nome da funcionalidade ou item do Backlog<BR>
Persona: [nome do persona]<BR>
Cenário: [descrição do cenário]<BR>
Given (Dado): [Estado inicial ou ponto de partida]<BR>
When (Quando) [Ações que serão realizadas]<BR>
Then (Então) [Pós-condição, o que deve acontecer após a execução das ações]<BR>
<BR>
<exemplo><BR>
Funcionalidade: Fazer Login<BR>
Persona: Cliente<BR>
<BR>
Cenário: Fazer login com sucesso<BR>
Dado: Que entro na aplicação<BR>
Quando: Quando informo meu e-mail <BR>
E: minha senha de acesso<BR>
Então: Recebo a autorização de acesso a App<BR>
<BR>
E-mail |	Senha |	Resultado Esperado
-------|--------|-------
Jose.ferreira@email.com |****** | Autorizado (Login com sucesso)

Cenário: Fazer login com insucesso<BR>
Dado: Que entro na aplicação<BR>
Quando: Quando informo meu e-mail<BR>
E: minha senha de acesso<BR>
Então: Recebo a mensagem de erro "e-mail ou senha inválido"<BR>
<BR>
E-mail |	Senha |	Resultado Esperado
-------|--------|-------
Jose.ferreira@email.com |****** | Mensagem de erro
<BR>
<B>Importante:</B><BR>
Uma boa prática é sinalizar os itens do Backlog que estão prontos para serem desenvolvidos. Por isso, após a especificação dos requisitos, os itens do Backlog correspondentes devem estar com status de DoR (Definition of Ready ou Definição de Pronto).<BR>
<BR>

<B>Desafio-4 - Casos de Uso:</B><BR>

Casos de Uso é uma técnica utilizada pelo mercado (algumas vagas de emprego pedem esse conhecimento) para especificar o comportamento externo do software, ele mostra como ocorre a interação “ator” e software. Dica: "ator" e "persona" são sinônimos neste contexto.
Escrever os Casos de Uso.<BR>
Comece identificando o ator, em seguida faça o diagrama e para concluir descreva o caso de uso, veja o exemplo:<BR>
<BR>
  Diagrama de Caso de Uso<BR>
<BR>
<img src="http://www.etecnologia.com.br/images/fars/ucfazerlogin.png"><BR>
<HR>
Nome: UC#1 - Fazer Login<BR>
Ponto de ativação: Este caso de uso começa quando o cliente acessa a App e seleciona a opção fazer login.<BR>
Ator: Cliente<BR>
Objetivo: Autorizar o acesso do cliente<BR>
Pré-condição: Cliente cadastrado<BR>
Fluxo Normal:<BR>
1 - O cliente informa seu e-mail<BR>
2 - O cliente informa sua senha <BR>
3 - O cliente clica no botão enviar<BR>
4 - A App autêntica o cliente e a senha<BR>
5 - A App autoriza o acesso do cliente<BR>
<BR>
Fluxo Exceção:<BR>
1 - O cliente informa seu e-mail<BR>
2 - O cliente informa sua senha <BR>
3 - O cliente clica no botão enviar<BR>
4 - A App não autêntica o cliente e a senha<BR>
5 - A App a exibe a mensagem erro: Senha ou e-mail inválido<BR>
6 - A App não autoriza o acesso do cliente<BR>
<BR>
Pós-condição: Cliente autorizado<BR>

Cenário/Fluxo	| Pós-condição	| Autorização de acesso
-----|-----|----
Fluxo normal |	Verdadeira |	Sim
Fluxo de Exceção | Falsa	| Não 
<HR>
<BR>

**Desafio-5 - Requisitos Emergentes:**<BR> 
<BR>
Descobrir os Requisitos Não Funcionais emergentes (são aqueles requisitos que emergiram durante o fazimento da Especificação de Requisitos, eles também deve fazer parte da Especificação), importante ressaltar que na maioria das vezes eles não estão presentes no Backlog. Veja o exemplo:<BR>
<BR>
<exemplo><BR>
O item Fazer login quando implementado deverá ser feito em ambiente seguro e a senha deverá estar criptografada, para que isso aconteça teremos que especificar um requisito não funcional emergente. Neste caso, teremos um Requisito Não Funcional derivado de um Requisito Funcional. Podemos chamá-lo de Segurança de Acesso.<BR>

![](http://www.etecnologia.com.br/images/fars/rnrnfinclude.png)
