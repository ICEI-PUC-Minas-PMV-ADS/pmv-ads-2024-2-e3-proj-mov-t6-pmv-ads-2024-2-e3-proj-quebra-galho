# Especificações do Projeto

<span style="color:red">Pré-requisitos: <a href="1-Documentação de Contexto.md"> Documentação de Contexto</a></span>

A definição do problema e os pontos mais relevantes a serem tratados neste projeto foram traçados com base nas experiências pessoais dos integrantes do grupo, relacionadas ao tema, e nos relatos de pessoas próximas. As informações descritas nessa seção estão organizados em personas e histórias de usuários.

## Personas

|FOTO |NOME| IDADE |OCUPAÇÃO|PROBLEMAS/FRUSTAÇÕES|
|-------|----|-------|--------|--------------------|
| <img src="img/Personas/MarianaSilva.jpg" alt="Mariana Silva" width="200"> | Mariana Silva | 21 Anos |Estudante de Engenharia de Computação | Frequentemente enfrenta a falta de carregadores e cabos USB, o que pode interromper seus estudos. |
| <img src="img/Personas/LucasPereira.jpg" alt="Lucas Pereira" width="200"> | Lucas Pereira | 24 Anos | Estudante de Administração de Empresas | Falta de canetas pode causar problemas durante provas. |
| <img src="img/Personas/AnaCosta.jpg" alt="Ana Costa" width="200"> | Ana Costa | 22 Anos |Estudante de Design Gráfico | Dificuldade em encontrar adaptadores quando necessário pode atrasar seus projetos de design. |
| <img src="img/Personas/PedroAlmeida.jpg" alt="Pedro Almeida" width="200"> | Pedro Almeida | 25 Anos | Estudante de Engenharia de Software | Faltar esses itens pode atrapalhar seus projetos. |
| <img src="img/Personas/JuliaOliveira.jpg" alt="Julia Oliveira" width="200"> | Julia Oliveira | 23 Anos |Estudante de Arquitetura | A falta de papel e grampeador pode dificultar a organização e apresentação de projetos. |

## Histórias de Usuários

Com base na análise das personas foram identificadas as seguintes histórias de usuários:

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Mariana Silva  | Ter acesso a carregadores e cabos USB | Garantir que esses itens estejam disponíveis durante os estudos e trabalhos acadêmicos.|
|Lucas Pereira  | Ter acesso a caneta e corretivo. | Poder utilizar esses itens durante provas para garantir um bom desempenho. |
|Ana Costa  | Ter acesso a adaptadores de tomada. | Facilitar o uso de equipamentos eletrônicos em seus projetos de design sem interrupções. |
|Pedro Almeida  |  Ter acesso a lapiz e borracha. | Garantir que esses itens estejam disponíveis para anotações e ajustes em projetos de programação. |
|Julia Oliveira  | Ter acesso a papel e grampeadore. | Manter a organização e a apresentação dos documentos acadêmicos e projetos. |

## Modelagem do Processo de Negócio 

### Análise da Situação Atual

Apresente aqui os problemas existentes que viabilizam sua proposta. Apresente o modelo do sistema como ele funciona hoje. Caso sua proposta seja inovadora e não existam processos claramente definidos, apresente como as tarefas que o seu sistema pretende implementar são executadas atualmente, mesmo que não se utilize tecnologia computacional. 

### Descrição Geral da Proposta

Apresente aqui uma descrição da sua proposta abordando seus limites e suas ligações com as estratégias e objetivos do negócio. Apresente aqui as oportunidades de melhorias.

### Processo 1 – NOME DO PROCESSO

Apresente aqui o nome e as oportunidades de melhorias para o processo 1. Em seguida, apresente o modelo do processo 1, descrito no padrão BPMN. 

![Processo 1](img/02-bpmn-proc1.png)

### Processo 2 – NOME DO PROCESSO

Apresente aqui o nome e as oportunidades de melhorias para o processo 2. Em seguida, apresente o modelo do processo 2, descrito no padrão BPMN.

![Processo 2](img/02-bpmn-proc2.png)

## Indicadores de Desempenho

Apresente aqui os principais indicadores de desempenho e algumas metas para o processo. Atenção: as informações necessárias para gerar os indicadores devem estar contempladas no diagrama de classe. Colocar no mínimo 5 indicadores. 

Usar o seguinte modelo: 

![Indicadores de Desempenho](img/02-indic-desemp.png)
Obs.: todas as informações para gerar os indicadores devem estar no diagrama de classe a ser apresentado a posteriori. 

## Requisitos

As tabelas que se seguem apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto. Para determinar a prioridade de requisitos, aplicar uma técnica de priorização de requisitos e detalhar como a técnica foi aplicada.

### Requisitos Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-001| O sistema deve permitir que o usuário efetue o login ou cadastre-se. | ALTA | 
|RF-002| Tela carregada após o login, ela deve conter uma listagem de itens dando preferência aos pedidos de amigos.   | BAIXA |
|RF-003| O sistema deve permitir que o usuário faça um pedido por empréstimo, especificando uma localização específica (uma seleção de prédios), a categoria do item,  qual o item de fato e um preço   | ALTA |
|RF-004| O sistema deve permitir que o usuário atenda um pedido.   | ALTA |
|RF-005| O sistema deve redirecionar o usuário para um serviço de chat externo.   | ALTA |
|RF-006| O sistema deve permitir que o usuário adicione outros usuários como amigos.   | MÉDIA |
|RF-007| O sistema deve permitir que o usuário edite seu próprio perfil.   | ALTA |
|RF-008| Ao finalizar um empréstimo, o sistema deve permitir que os usuários avaliem uns aos outros com uma avaliação positiva ou negativa. Caso seja uma negativa, o usuário deve informar um motivo.   | ALTA |
|RF-009| O sistema deve mostrar uma notificação quando existir um ou mais pedidos ativos e/ou solicitações de amizade.    | BAIXA |


### Requisitos não Funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-001| O carregamento da tela não deve demorar mais que 1,5 segundos. | ALTA | 
|RNF-002| Os servidores devem estar operantes durante 24h por dia |  BAIXA | 
|RNF-003| O sistema deve armazenar os dados de cadastro e login do usuário, além das relações de amizade entre os usuários. |  ALTA | 
|RNF-004| O sistema deverá ter uma funcionalidade que possibilitará o usuário que fez o pedido e o usuário que atenderá o pedido se comunicarem, através de um chat externo, sendo esse o WhatsApp. |  ALTA | 

Com base nas Histórias de Usuário, enumere os requisitos da sua solução. Classifique esses requisitos em dois grupos:

- [Requisitos Funcionais
 (RF)](https://pt.wikipedia.org/wiki/Requisito_funcional):
 correspondem a uma funcionalidade que deve estar presente na
  plataforma (ex: cadastro de usuário).
- [Requisitos Não Funcionais
  (RNF)](https://pt.wikipedia.org/wiki/Requisito_n%C3%A3o_funcional):
  correspondem a uma característica técnica, seja de usabilidade,
  desempenho, confiabilidade, segurança ou outro (ex: suporte a
  dispositivos iOS e Android).
Lembre-se que cada requisito deve corresponder à uma e somente uma
característica alvo da sua solução. Além disso, certifique-se de que
todos os aspectos capturados nas Histórias de Usuário foram cobertos.

## Restrições

O projeto está restrito pelos itens apresentados na tabela a seguir.

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|01| O projeto deverá ser entregue até o final do semestre |
|02| Não pode ser desenvolvido um módulo de backend        |

Enumere as restrições à sua solução. Lembre-se de que as restrições geralmente limitam a solução candidata.

> **Links Úteis**:
> - [O que são Requisitos Funcionais e Requisitos Não Funcionais?](https://codificar.com.br/requisitos-funcionais-nao-funcionais/)
> - [O que são requisitos funcionais e requisitos não funcionais?](https://analisederequisitos.com.br/requisitos-funcionais-e-requisitos-nao-funcionais-o-que-sao/)

## Diagrama de Casos de Uso

O diagrama de casos de uso é o próximo passo após a elicitação de requisitos, que utiliza um modelo gráfico e uma tabela com as descrições sucintas dos casos de uso e dos atores. Ele contempla a fronteira do sistema e o detalhamento dos requisitos funcionais com a indicação dos atores, casos de uso e seus relacionamentos. 

As referências abaixo irão auxiliá-lo na geração do artefato “Diagrama de Casos de Uso”.

> **Links Úteis**:
> - [Criando Casos de Uso](https://www.ibm.com/docs/pt-br/elm/6.0?topic=requirements-creating-use-cases)
> - [Como Criar Diagrama de Caso de Uso: Tutorial Passo a Passo](https://gitmind.com/pt/fazer-diagrama-de-caso-uso.html/)
> - [Lucidchart](https://www.lucidchart.com/)
> - [Astah](https://astah.net/)
> - [Diagrams](https://app.diagrams.net/)

# Matriz de Rastreabilidade

A matriz de rastreabilidade é uma ferramenta usada para facilitar a visualização dos relacionamento entre requisitos e outros artefatos ou objetos, permitindo a rastreabilidade entre os requisitos e os objetivos de negócio. 

A matriz deve contemplar todos os elementos relevantes que fazem parte do sistema, conforme a figura meramente ilustrativa apresentada a seguir.

![Exemplo de matriz de rastreabilidade](img/02-matriz-rastreabilidade.png)

> **Links Úteis**:
> - [Artigo Engenharia de Software 13 - Rastreabilidade](https://www.devmedia.com.br/artigo-engenharia-de-software-13-rastreabilidade/12822/)
> - [Verificação da rastreabilidade de requisitos usando a integração do IBM Rational RequisitePro e do IBM ClearQuest Test Manager](https://developer.ibm.com/br/tutorials/requirementstraceabilityverificationusingrrpandcctm/)
> - [IBM Engineering Lifecycle Optimization – Publishing](https://www.ibm.com/br-pt/products/engineering-lifecycle-optimization/publishing/)


# Gerenciamento de Projeto

De acordo com o PMBoK v6 as dez áreas que constituem os pilares para gerenciar projetos, e que caracterizam a multidisciplinaridade envolvida, são: Integração, Escopo, Cronograma (Tempo), Custos, Qualidade, Recursos, Comunicações, Riscos, Aquisições, Partes Interessadas. Para desenvolver projetos um profissional deve se preocupar em gerenciar todas essas dez áreas. Elas se complementam e se relacionam, de tal forma que não se deve apenas examinar uma área de forma estanque. É preciso considerar, por exemplo, que as áreas de Escopo, Cronograma e Custos estão muito relacionadas. Assim, se eu amplio o escopo de um projeto eu posso afetar seu cronograma e seus custos.

## Gerenciamento de Tempo

Com diagramas bem organizados que permitem gerenciar o tempo nos projetos, o gerente de projetos agenda e coordena tarefas dentro de um projeto para estimar o tempo necessário de conclusão.

![Diagrama de rede simplificado notação francesa (método francês)](img/02-diagrama-rede-simplificado.png)

O gráfico de Gantt ou diagrama de Gantt também é uma ferramenta visual utilizada para controlar e gerenciar o cronograma de atividades de um projeto. Com ele, é possível listar tudo que precisa ser feito para colocar o projeto em prática, dividir em atividades e estimar o tempo necessário para executá-las.

![Gráfico de Gantt](img/02-grafico-gantt.png)

## Gerenciamento de Equipe

O gerenciamento adequado de tarefas contribuirá para que o projeto alcance altos níveis de produtividade. Por isso, é fundamental que ocorra a gestão de tarefas e de pessoas, de modo que os times envolvidos no projeto possam ser facilmente gerenciados. 

![Simple Project Timeline](img/02-project-timeline.png)

## Gestão de Orçamento

O processo de determinar o orçamento do projeto é uma tarefa que depende, além dos produtos (saídas) dos processos anteriores do gerenciamento de custos, também de produtos oferecidos por outros processos de gerenciamento, como o escopo e o tempo.

![Orçamento](img/02-orcamento.png)
