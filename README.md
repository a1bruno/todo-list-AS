# Projeto: Gerenciador de Tarefas v2.0

## 1. Visão Geral

Este é um projeto de um Gerenciador de Tarefas via terminal, desenvolvido em Python. A base do projeto oferece funcionalidades para adicionar, listar, concluir e remover tarefas. O objetivo deste trabalho é estender a funcionalidade do sistema e demonstrar um fluxo de trabalho de desenvolvimento profissional utilizando Git e GitHub.

## 2. Configuração Inicial

1.  **Fork:** Realize um fork deste repositório para a sua conta pessoal no GitHub.
2.  **Clone:** Clone o repositório que você criou (o seu fork) para o seu ambiente de desenvolvimento local.
    ```bash
    git clone [https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git](https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git)
    ```

## 3. Especificações da Tarefa

Você deve implementar as **duas** novas funcionalidades descritas abaixo.

### Funcionalidade 1: Prioridade de Tarefas

* **Estrutura de Dados:** A estrutura de dados de cada tarefa deve ser alterada para incluir um campo `prioridade`.
* **Adicionar Tarefa:** A função de adição deve ser modificada para solicitar ao usuário um nível de prioridade (`Alta`, `Média`, `Baixa`). Uma entrada inválida deve resultar na prioridade padrão `Baixa`.
* **Listar Tarefas:** A função de listagem deve ser atualizada para exibir a prioridade de cada tarefa.

### Funcionalidade 2: Edição de Descrição da Tarefa

* **Menu:** Uma nova opção para "Editar Tarefa" deve ser adicionada ao menu principal.
* **Implementação:** Deve ser criada uma função que permita ao usuário:
    1.  Selecionar uma tarefa existente pelo seu índice.
    2.  Visualizar a descrição atual.
    3.  Inserir uma nova descrição para substituí-la.
* **Feedback:** O sistema deve informar ao usuário se a operação foi bem-sucedida.

## 4. Requisitos de Entrega e Fluxo de Trabalho

A avaliação levará em conta a organização do seu repositório e o uso correto das ferramentas.

* **README.md:** Este arquivo deve ser atualizado com a seção "Minhas Contribuições" devidamente preenchida.
* **`.gitignore`:** O repositório precisa conter um arquivo `.gitignore` configurado adequadamente para projetos Python, ignorando arquivos e pastas como `__pycache__` e `venv/`.
* **Fluxo com Branches:** Cada uma das duas funcionalidades deve ser desenvolvida em uma *feature branch* separada (ex: `feature/task-priority` e `feature/edit-task-description`). Após a finalização, cada branch deve ser mesclada (`merge`) de volta à branch `main`.
* **Histórico de Commits:** É exigido um histórico com um mínimo de **8 a 10 commits atômicos**. As mensagens de commit devem ser claras e refletir o trabalho realizado em cada etapa.

## 5. Critérios de Avaliação

* **README:** Clareza e detalhamento da seção "Minhas Contribuições".
* **Git:** Qualidade das mensagens de commit e demonstração do fluxo de trabalho com branches e merges.
* **Funcionalidade:** Implementação correta e funcional das modificações solicitadas.
* **Código:** Legibilidade, organização e qualidade geral do código implementado.

---

## (Template para o Aluno)

## Minhas Contribuições

* **Nome:** `[Bruno Barcelos Alves]`
* **GitHub:** `[https://github.com/a1bruno]`

### Modificação 1: Prioridade de Tarefas

**Lógica Implementada:**
* [1. Adicionei um novo argumento chamado 'prioridade 'para a função que registrava novas tarefas;]
* [2. Na definição da estrutura onde é definido chave:valor, defini uma chave 'prioridade' com o valor passado como argumento;]
* [3. Adicionei, na opção 1 do menu, uma nova variável que capta um input do usuário que será o argumento propriedade da função;]
* [4. Implementei algumas validações com if no corpo da função para verificar se a entrada corresponde com a solicitação;]

**Como Testar:**
* [Forneça um passo a passo claro para que o avaliador possa testar a sua implementação.]
* [1. Para testar é necessário somente acessar a opção 1 do menu e registrar uma nova tarefa. Será solicitada a entrada da prioridade.]

### Modificação 2: Editar Descrição da Tarefa

**Lógica Implementada:**
* [1. Adicionei uma nova opção ao menu principal 'Editar descrição de uma tarefa';]
* [2. Adicionei a nova opção nas validações de opções 'elif escolha == "4"';]
* [3. Implementei a função que edita a descrição de uma tarefa existente com base na lista de tarefas e com o indice fornecido pelo usuário;]
* [4. Na área de validação das opções, o elif, eu chamei a função criada 'editar_descricao()' passando como argumentos: a lista de tarefas, o indice do item que o usuário escolheu;]
* [5. Eu fiz uma refatoração de um 'print' onde a falta de um espaço estava me incomodando, provavelmente essa alteração não deveria ter sido feita nessa branch, mas só pensei nisso depois de fazer.]

**Como Testar:**
* [Forneça um passo a passo claro para que o avaliador possa testar a sua implementação.]
* [1. Registre uma nova tarefa;]
* [2. Escolha a opção '4' para editar a descrição de uma tarefa existente;]
* [3. Forneça o indice da tarefa que deseja alterar a descrição.]