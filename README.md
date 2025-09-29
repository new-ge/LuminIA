# API 6º Semestre BD

# PRO4TECH

<p align="center">
      <img src="docs/Logo LuminIA.jpeg" alt="logo_projeto" width="200">
      <h2 align="center"> LuminIA </h2>
</p>

<p align="center">
  | <a href ="#desafio"> Desafio</a>  |
  <a href ="#solucao"> Solução</a>  |   
  <a href ="#backlog"> Backlog do Produto</a>  |
  <a href ="#dor">DoR</a>  |
  <a href ="#dod">DoD</a>  |
  <a href ="#sprint"> Cronograma de Sprints</a>  |
  <a href ="#tecnologias">Tecnologias</a> | 
  <a href ="#Burndown">Burndown</a> | 
  <a href ="#equipe"> Equipe</a> |
</p>

> Status do Projeto: Em desenvolvimento... 🚧 
>
> Relatório de Testes: Em desenvolvimento... 🚧 📊
>
> Pasta de Documentação: Em desenvolvimento... 🚧 [Link]([docs/201302063.jpeg](https://github.com/new-ge/LuminIA/wiki)) 📄
> 
> Video do Projeto:  [Youtube](https://www.youtube.com/watch?v=0wkynwCSBhQ&list=PLHVGmwwpPVx5gGkzYJdrJ0NI2eazVkwds&pp=gAQB) 📽️

## 🏅 Desafio <a id="desafio"></a>

## Descrição do Desafio

A situação atual mostra que o banco de dados de suporte já não atende bem às necessidades da operação: ele não garante totalmente a conformidade com a lei, não oferece clareza suficiente para auditorias e nem facilita análises históricas ou preditivas. Isso significa que os relatórios acabam sendo engessados e repetitivos, sem dar uma visão completa para quem precisa tomar decisões. A proposta de modernização busca corrigir essas limitações, trazendo mais segurança no tratamento dos dados, transparência no acompanhamento das ações e dashboards que ajudem cada nível da equipe – desde os analistas até gestores e responsáveis estratégicos – a visualizar exatamente as informações de que precisam para trabalhar com mais eficiência.

---

## 🏅 Solução <a id="solucao"></a>

A LuminIA é um dashboard integrado com inteligência artificial, cuidadosamente desenvolvido para facilitar e otimizar a tomada de decisões da gestão, ao mesmo tempo em que oferece suporte contínuo aos analistas no atendimento de chamados. Com insights estratégicos e o reforço da inteligência artificial, a LuminIA transforma informações complexas em ações concretas, tornando todo o processo de suporte mais eficiente, ágil, inteligente e alinhado às necessidades do negócio. Tudo isso é oferecido por uma ferramenta moderna, intuitiva e de fácil utilização, projetada para que gestores e analistas consigam acessar rapidamente os dados.

---

## Requisitos Não Funcionais

| **ID** |  **Título** |
|--------|------------|
|RNF01|	Conformidade com LGPD (anonimização/pseudonimização de dados sensíveis)|
|RNF02|	Base preparada para análises históricas|
|RNF03|	Interface responsiva (web e mobile)|
|RNF04|	IA de analise de chamados|
|RNF05| Estrutura de nível de acesso|
|RNF06|	Manual do Usuário|
|RNF07|	Modelagem do Banco de Dados|

---

## Requisitos Funcionais

| **ID** | **Persona**   | **Título**                              | **Descrição**                                                                                                                                                                               |
| ------ | ------------- | --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| R1     | Analista      | Tempo médio de antecedência             | O sistema deverá exibir um card mostrando o **tempo médio de antecedência**, que servirá para o Analista (N1, N2 ou N3) analisar o desempenho da equipe que ele pertence, no caso o tempo ganho médio por chamado resolvido ou fechado. |
| R2     | Analista      | Volume de reincidência                  | O sistema deverá exibir um card com a quantidade de **chamados reincidentes**, que servirá para o Analista (N1, N2 ou N3) analisar o desempenho da equipe que ele pertence, no caso o número de casos dados como resolvido ou fechado que voltaram ao estado anterior dentro do fluxo de status.                                                       |
| R3     | Analista      | Volume de chamados negativos            | O sistema deverá exibir um gráfico com a quantidade de **chamados de avaliações ruins**, que servirá para o Analista (N1, N2 ou N3), ter ciência de sua demanda.                                                  |
| R4     | Analista      | Volume de chamados por período          | O sistema deverá exibir um gráfico mostrando **quantidade de chamados em períodos selecionáveis**, que servirá para o Analista (N1, N2 ou N3) analisar o desempenho da equipe que ele pertence de forma retroativa.                     |
| R5     | Analista      | Filtro SLA                     | O sistema deverá permitir que o analista aplique o **filtro de SLA** nos chamados no qual poderá ter um feedback nos cards e gráficos por tipo de cliente que estão lidando podendo ser: Padrão, VIP ou  Estendido.            |
| R6     | Analista      | Filtro status                     | O sistema deverá permitir que o analista aplique o **filtro status** no qual poderá ter um feedback nos cards e gráficos por tipo de status se encontram os chamados podendo ser: Aberto, Em Atendimento, Aguardando Cliente, Resolvido e Fechado.            |
| R7     | Analista      | Filtro prioridade                     | O sistema deverá permitir que o analista aplique o **filtro prioridade** no qual poderá ter um feedback nos cards e gráficos por tipo de prioridade que se encontram os chamados podendo ser: Baixa, Média, Alta e Crítica.            |
| R8     | Analista      | Filtro subcategoria                     | O sistema deverá permitir que o analista aplique o **filtro subcategoria** no qual poderá ter um feedback nos cards e gráficos por tipo de subcategoria que se encontram os chamados podendo ser: Erro de sistema, Lentidão, Funcionalidade indisponível, Problemas de login, Permissões, Cadastro de usuários, Relatórios, Exportação e Dados inconsistentes.           |
| R9     | Analista      | Filtro período                     | O sistema deverá permitir que o analista aplique o **filtro período** no qual poderá ter um feedback nos cards e gráficos por período, podendo filtrar entre duas datas.           |
| R10     | Product Owner | Volume aberto geral                     | O sistema deverá exibir um card mostrando o **total de chamados abertos** de todas as equipes que supervisiona, que servirá para analisar a situação de demanda de suas equipes.                                                                                      |
| R11     | Product Owner | Volume de chamados por período          | O sistema deverá exibir um gráfico com a **quantidade de chamados em períodos selecionáveis** de todas as equipes que supervisiona, que servirá para analisar a situação de suas equipes baseado em um período.                                                        |
| R12     | Product Owner | Tempo médio de resolução                | O sistema deverá exibir um gráfico ou card com o **tempo médio gasto para resolver chamados** de todas as equipes que supervisiona, que servirá para analisar a situação de suas equipes baseado em um tempo médio que a equipe leva para resolver um caso.                                                                                  |
| R13     | Product Owner | Chamados com SLA excedido               | O sistema deverá exibir um card identificando **chamados com o SLA excedido** de todas as equipes que supervisiona, que servirá para analisar a situação de suas equipes baseado em um número de chamado que passaram do limite de tempo para ser solucionado.                                                                                              |
| R14    | Product Owner | Volume de reincidência da equipe        | O sistema deverá exibir um gráfico ou card com a quantidade de **chamados reincidentes** de todas as equipes que supervisiona, que servirá para analisar a situação de suas equipes baseado no número de casos dados como resolvido ou fechado que voltaram ao estados anterior dentro do fluxo de status.                                                                     |
| R15    | Product Owner | Análise de sentimento                   | O sistema deverá exibir um gráfico com a quantidade de **chamados de avaliações ruins** de todas as equipes que supervisiona, que servirá para analisar a situação de suas equipes baseado no número de casos de reclamações de produtos da empresa.                                                                     |
| R16    | Product Owner | Filtro SLA                       | O sistema deverá permitir que o PO aplique **filtro de SLA** nos chamados no qual poderá ter um feedback nos cards e gráficos por tipo de cliente que as suas equipes estão lidando podendo ser: Padrão, VIP ou  Estendido.                                    |
| R17    | Product Owner | Filtro equipe                       | O sistema deverá permitir que o PO aplique **filtro de equipe** nos chamados no qual poderá ter um feedback nos cards e gráficos por qual equipe quer analisar.       |
| R18    | Product Owner | Filtro status                       | O sistema deverá permitir que o PO aplique **filtro de status** no qual poderá ter um feedback nos cards e gráficos por tipo de status se encontram os chamados que as suas equipes estão lidando podendo ser: Aberto, Em Atendimento, Aguardando Cliente, Resolvido e Fechado.                                     |
| R19    | Product Owner | Filtro período                       | O sistema deverá permitir que o PO aplique **filtro de período** no qual poderá ter um feedback nos cards e gráficos por período dos chamados que as suas equipes estão lidando podendo filtrar entre duas datas.                              |
| R20    | Product Owner | Filtro prioridade                       | O sistema deverá permitir que o PO aplique **filtro de prioridade** no qual poderá ter um feedback nos cards e gráficos por tipo de prioridade que se encontram os chamados que as suas equipes estão lidando podendo ser: Baixa, Média, Alta e Crítica.        |
| R21    | Product Owner | Filtro subcategoria                       | O sistema deverá permitir que o PO aplique **filtro de subcategoria** no qual poderá ter um feedback nos cards e gráficos por tipo de subcategoria que se encontram os chamados que as suas equipes estão lidando podendo ser: Erro de sistema, Lentidão, Funcionalidade indisponível, Problemas de login, Permissões, Cadastro de usuários, Relatórios, Exportação e Dados inconsistentes.        |
| R22   | Product Owner | Filtro tag                       | O sistema deverá permitir que o PO aplique **filtro de tag** no qual poderá ter um feedback nos cards e gráficos por tipo de tag que se encontram os chamados que as suas equipes estão lidando podendo ser: Urgente, Revisar, Bug, Solicitação, Melhoria, Financeiro, RH, TI, Duplicado, e Acompanhamento.        |
| R23    | Gestor        | Acesso global aos dados    | O sistema deverá exibir todos os gráficos, cards e filtros do nível de acesso do PO, porém no dashboard do gestor terá acesso a todas as equipes disponíveis.   |
| R24     | ADM         | Gestão de usuários e permissões       | Permitir ao administrador: <br>• Criar, editar e excluir usuários.<br>• Definir perfis e permissões por nível hierárquico.<br>• Garantir que usuários vejam apenas dados autorizados.<br>• Excluir dados de usuários quando solicitado (conformidade LGPD).<br>**Comportamento esperado:** logs de criação, edição e exclusão de usuários.            |
| R25     | ADM         | Logs detalhados                       | Armazenar **logs completos de todas as operações**, incluindo login/logout, alterações de dados, exclusões, acessos a relatórios e filtros aplicados.<br>**Objetivo:** garantir rastreabilidade e auditoria.                                               |
| R26     | Analista N1 | FAQ                                   | Disponibilizar **FAQ automatizado** para analistas de nível 1:            |


---
## 📋 Backlog do Produto <a id="backlog"></a>

|  **Rank** | **Épico** | **Prioridade** | **User Story** | **Sprint** | **Story Points** | **Status** | **Requisitos** |
| :--: | :--------: | :------: | :----------: | :----: | :------------------: | :----: | :----:|
| 1 | Dashboard de Indicadores de Suporte com IA | Alta | Como gestor ou analista de suporte, quero disponibilizar um FAQ com respostas às perguntas mais comuns dos clientes, para que eu possa reduzir o volume de chamados repetitivos e agilizar o atendimento. | 2 | 8 | Em andamento | R26, RNF04 |
| 2 | Dashboard de Indicadores de Suporte com IA | Alta | Como gestor de suporte, quero visualizar o volume de chamados em aberto, para que possa saber quantos chamados ainda estão precisando de uma resposta. | 1 | 4 | ✅Concluído | R23, RNF02 |
| 3 | Dashboard de Indicadores de Suporte com IA | Alta | Como gestor de suporte, quero visualizar o volume de chamados por período, com uma linha de tendência gerada por IA, para que possa identificar os picos de chamados e antecipar quais tipos de chamados têm maior probabilidade de ocorrer. | 1 | 11 | ✅Concluído | R23, RNF04 |
| 4 | Dashboard de Indicadores de Suporte com IA | Alta | Como gestor de suporte, quero visualizar o tempo médio de resolução dos chamados, para que possa identificar se o atendimento está dentro dos padrões esperados. | 1 | 4 | ✅Concluído | R23 |
| 5 | Dashboard de Indicadores de Suporte com IA | Alta | Como gestor de suporte, quero visualizar o volume de chamados que excederam o SLA, para que possa identificar atrasos, tomar ações corretivas e melhorar a eficiência da equipe de suporte. | 1 | 4 | ✅Concluído | R23 |
| 6 | Dashboard de Indicadores de Suporte com IA | Alta | Como gestor de suporte, quero visualizar o volume de chamados reincidentes, para que possa identificar problemas recorrentes, reduzir retrabalho da equipe e melhorar a satisfação do cliente. | 1 | 4 | ✅Concluído | R23, RNF02 |
| 7 | Dashboard de Indicadores de Suporte com IA | Alta | Como gestor de suporte, quero visualizar o volume de sentimento, usando uma IA para análise, para que possa identificar padrões recorrentes e a identificação rápida de chamados críticos. | 1 | 9 | ✅Concluído | R23, RNF04 |
| 8 | Dashboard de Indicadores de Suporte com IA | Alta | Como gestor de suporte, quero filtrar por planos de SLA, equipe, status, período, prioridade, subcategoria e tag, para que possa analisar os dados segmentados e tomar decisões mais precisas. | 1 | 28 | ✅Concluído | R23 |
| 9 | Dashboard de Indicadores de Suporte com IA | Alta | Como analista de suporte, quero visualizar o tempo médio de antecedência, para que eu possa entender se estou resolvendo os chamados com antecedência suficiente em relação ao prazo. | 2 | | Em andamento | R1 |
| 10 | Dashboard de Indicadores de Suporte com IA | Alta | Como analista de suporte, quero visualizar o volume de chamados reincidentes, para que eu possa identificar quantos problemas estão retornando e melhorar a qualidade do atendimento. | 2 | | Em andamento | R2 |
| 11 | Dashboard de Indicadores de Suporte com IA | Alta | Como analista de suporte, quero visualizar o volume de chamados com sentimento negativo, usando uma IA para análise, para que eu possa identificar padrões e atuar nos chamados mais críticos. | 2 | | Em andamento | R3, RNF04 |
| 12 | Dashboard de Indicadores de Suporte com IA | Alta | Como analista de suporte, quero visualizar o volume de chamados por período, para que possa analisar a demanda de atendimento e identificar picos de chamados. | 2 | | Em andamento | R4 |
| 13 | Dashboard de Indicadores de Suporte com IA | Alta | Como analista de suporte, quero filtrar por planos de SLA, status, prioridade, subcategoria e período, para que possa analisar os dados segmentados e melhorar o atendimento. | 2 | | Em andamento | R5, R6, R7, R8, R9 |
| 14 | Gestão de Acessos | Média | Como administrador, quero criar diferentes níveis de acesso, para que eu possa controlar quem pode ver tais dados. | 3 | | Em andamento | R23, RNF05 |
| 15 | Administração | Média | Como administrador, quero excluir usuários, para que possa revogar o acesso a aplicação. | 3 | | Em andamento | R24 RNF05 |
| 16 | Administração | Média | Como administrador, quero criar usuários, para que possa conceder o acesso a aplicação. | 3 | | Em andamento | R24, RNF05 | 
| 17 | Administração | Média | Como administrador, quero editar usuários, para que possa editar as informações dos usuários da aplicação. | 3 | | Em andamento | R24, RNF05 |
| 18 | Login | Baixa | Como usuário da aplicação, quero realizar login com credenciais seguras, para que eu possa acessar apenas as funcionalidades autorizadas ao meu perfil. | 3 | | Em andamento | RNF05 |
| 19 | Modernização dos dados | Alta | Como usuário da aplicação, quero que tenha uma modernização dos dados, para que possa acessar com mais facilidade os dados. | 1 | 3 | ✅Concluído | RNF07 |
| 20 | Modernização dos dados | Alta | Como usuário da aplicação, quero que meus dados pessoais sejam tratados em conformidade com a LGPD, ara que eu tenha segurança, transparência e facilidade ao acessar, corrigir ou excluir meus próprios dados. | 2 | 3 | Em andamento | RNF01 |
| 21 | Manual do Usuário | Alta | Como usuário da aplicação, quero que tenha um manual do usuário, para que possa ver as funcionalidades e saber como mexer na aplicação | 3 | | Em andamento | RNF06 |

---

## 🏃‍ DoR - Definition of Ready <a id="dor"></a>

- Tarefas divididas a partir das User Stories
- Design pronto no Figma
- User Stories com Critérios de Aceitação
  
## 🏆 DoD - Definition of Done <a id="dod"></a>

- Manual do usuário
- Código completo
---

## 📅 Cronograma de Sprints <a id="sprint"></a>

| Sprint          |    Período    |
| --------------- | :-----------: | 
| 🔖 **SPRINT 1** | 08/09 - 28/09 |
| 🔖 **SPRINT 2** | 06/10 - 26/10 | 
| 🔖 **SPRINT 3** | 03/11 - 23/11 |

## 🆕 Burndown <a id="Burndown"></a>
### Sprint-1
![Imagem do WhatsApp de 2025-09-28 à(s) 17 33 42_8897514d](https://github.com/user-attachments/assets/0db5215f-15f6-473b-a0b2-4543b32f4947)


## 💻 Tecnologias <a id="tecnologias"></a>

<h4 align="center">
 <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"></a>
 <a href="https://vuejs.org/"><img src="https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vue.js&logoColor=4FC08D"/></a>
 <a href="https://www.mongodb.com/"><img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white"></a>
 <a href="https://github.com/"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white"/></a>
 <a href="https://www.figma.com/"><img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white"/></a>
 <a href="https://pandas.pydata.org/"><img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"></a>
 <a href="https://fastapi.tiangolo.com/"><img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"></a>
 <a href="https://scikit-learn.org/"><img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"></a>
</h4>

## 🎓 Equipe <a id="equipe"></a>

<div align="center">
  <table>
    <tr>
      <th>Membro</th>
      <th>Função</th>
      <th>Github</th>
      <th>Linkedin</th>
    </tr>
    <tr>
      <td>Cauan Barbaglio</td>
      <td>Product Owner</td>
      <td><a href="https://github.com/Cauanvmb"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/cauan-barbaglio"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Vinícius Chaves</td>
      <td>Scrum Master</td>
      <td><a href="https://github.com/ChavesVini"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/vin%C3%ADcius-chaves-197353244"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Amanda Vannucci</td>
      <td>Desenvolvedor(a)</td>
      <td><a href="https://github.com/Amandavannuccic"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/amanda-vannucci"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Guilherme Wunderlich</td>
      <td>Desenvolvedor(a)</td>
      <td><a href="https://github.com/wunderlich-15"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/guilherme-wunderlich-aa56a2228"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Naiara Santos</td>
      <td>Desenvolvedor(a)</td>
      <td><a href="https://github.com/NaiaraSantos3"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/naiara-santos-73b83a186"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Raul Neto</td>
      <td>Desenvolvedor(a)</td>
      <td><a href="https://github.com/raulnt"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/raul-neto-b51b24157/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
  </table>
</div>
