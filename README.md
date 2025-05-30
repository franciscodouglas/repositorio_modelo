# repositorio_modelo 

## Boas Práticas
- O nome do repositório precisa ter o mesmo no do Projeto. Por exemplo: Projeto SIGA.
- Todo arquivo README precisa informar:
  - Visão Geral do Projeto
  - As Tecnologias utilizadas
  -  Como instalar ou utilizar esse projeto
  -  Quem contribuiu (A Equipe)
  -  Como pode contribuir? (Comunidade externa que visualiza esse Repositório PUBLICO)

  ## Organização de Pastas
  - Toda Linguagem de Programação ou Framework exige uma organização em pastas. Em comúm todoas elas tem essa estrutura:

    - /src -> A pasta indicada para colocar o código fonte do projto
    - /test -> A pasta é indicada para colocar os testes unitários
    - /public -> A pasta é indicada pra colocar o Front-End ou qualquer arquivo que precisa ficar à nível Público. A nível de API, teriamos os ENDPOINTs (Rotas de acesso)
    - /config -> (ou scripts) arquivos de configuração ou instalação do bibliotecas do projeto (isso também pode ficar na raiz do projeto - config é uma pasta opcional)
    - /docs -> A pasta é indicada para guardar imagens ou docs relacionados ao projeto. Por exemplo: Diagramas, Fluxogramas, Mapa Mentais, Canvas e etc.


  ## Utilizar boas práticas em Commits
  
  É necessário realizar os dois:

  - Commit Atômicos: Realizar commits pequenos-> a unidade de trabalho
  - Commit Semântico: É informar com sufixo e em poucas palavras o que foi realizado nessa unidade de trabalho


  ## Na raiz do Projeto

  - É necessário ter:
    - o gitignore: é utilizado para informar ao git quais extensões ou pastas que precisam ser  ignoradas
    - license: é informado qual é a licença do projeto (obrigatório quando o projeto é Público)
    - contribuiting: é informado quem são os autores e como contribuir
    - changelog: é utilizado para informar o Histórico de Versões do projeto


  ## Gerenciar Branchs
  - Um projeto pode ter algumas dessas branchs abaixo:
  - main (ou master): Versão estável do Projeto (ou aquilo que o público está utilizando no momento)
  - homolog (ou tests): 
    - Versão posterior a de desenvolvimento, ou seja, é a de testes. Normalmente ela antecipa a main
    - no final ela é mesclada a main

  - develop: 
    - Versão em desenvolvimento, normalmente é utilizado por Desenvolvedores do Projeto. 
    - Centralizadora das modificações realizadas pelo os devs 
    - no final ela é mesclada a homolog

- Branchs relacionadas ao card do kanban (branch-de-trabalho):
  - Por exemplo  [sufixo-atomic]/[nome-card]
  - cada card do Kanban vai ter uma branch
  - cada dev pega um ou N cards do Kanban 
  - cada branch é baseada da develop
  - no final ela é mesclada a develop

- Flow das branchs:
  - branch-de-trabalho -> develop -> homolog -> main 
 

