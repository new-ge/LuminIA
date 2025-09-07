# Padrão de Commits

Para a padronização dos commits, eles devem seguir o padrão "Conventional Commits".

## Formato do Commit:
```
<id tarefa> - <tipo>: <descrição>
```

## Tipos de Commit:

- test: indica qualquer tipo de criação ou alteração de códigos de teste. Exemplo: Criação de testes unitários.
- feat: indica o desenvolvimento de uma nova feature ao projeto. Exemplo: Acréscimo de um serviço, funcionalidade, endpoint, etc.
- refactor: usado quando houver uma refatoração de código que não tenha qualquer tipo de impacto na lógica/regras de negócio do sistema. Exemplo: Mudanças de código após um code review
- style: empregado quando há mudanças de formatação e estilo do código que não alteram o sistema de nenhuma forma.
- fix: utilizado quando há correção de erros que estão gerando bugs no sistema.
- chore: indica mudanças no projeto que não afetem o sistema ou arquivos de testes. São mudanças de desenvolvimento.
- docs: usado quando há mudanças na documentação do projeto.
- build: utilizada para indicar mudanças que afetam o processo de build do projeto ou dependências externas.
- perf: indica uma alteração que melhorou a performance do sistema.
- ci: utilizada para mudanças nos arquivos de configuração de CI.
- revert: indica a reverão de um commit anterior.

## Mais informações:
https://medium.com/linkapi-solutions/conventional-commits-pattern-3778d1a1e657