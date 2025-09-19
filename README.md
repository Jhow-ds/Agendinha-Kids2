# 🎮 Bem-vindo ao Gestão Maker!

O **Gestão Maker** é uma ferramenta completa para gerenciamento de sala de aula com elementos de gamificação. Projetado para ser simples e eficaz, ele funciona em um único arquivo HTML e salva todos os dados diretamente no seu navegador, sem a necessidade de um servidor ou banco de dados.

Este guia irá ajudá-lo a entender e utilizar todas as funcionalidades da plataforma.

## ✨ Primeiros Passos

1.  **Abra o Arquivo**: Para começar, simplesmente abra o arquivo `index.html` em qualquer navegador de internet moderno (como Google Chrome, Firefox, etc.).
2.  **Armazenamento Local**: Todos os dados (alunos, itens da loja, missões, etc.) são salvos no `localStorage` do seu navegador. Isso significa que os dados ficam salvos **apenas no computador e no navegador que você está usando**. Se você acessar o arquivo em outro computador ou em outro navegador, os dados não estarão lá.
3.  **Backup é Essencial**: Por conta do armazenamento local, é **altamente recomendado** que você use a função **Exportar Dados** regularmente para criar um arquivo de backup.

## 🚀 Funcionalidades Principais

A navegação é feita pela barra lateral (que fica oculta em telas de celular e pode ser aberta pelo menu no canto superior esquerdo).

### 👥 Painel de Alunos

Esta é a tela principal, onde você gerencia seus alunos.

* **Adicionar Alunos**:
    * **Individualmente**: Clique em **Novo Aluno**.
    * **Em Massa**: Vá para a seção **Cadastro em Massa**, selecione a turma, e cole a lista de nomes (um por linha).
* **Filtrar e Pesquisar**: Use os campos no topo para filtrar alunos por **turma** ou **pesquisar por nome**. O filtro de turma permanece ativo mesmo que você mude de seção e volte.
* **Card do Aluno**: Cada aluno tem um card com informações essenciais:
    * **Nome**: Exibe o primeiro e o último nome para melhor visualização.
    * **Avatar**: Gerado aleatoriamente. Passe o mouse sobre o card para ver o botão de **regenerar avatar** (🔄).
    * **Status de Presença**: A bolinha no canto do avatar indica se o aluno está presente (✅) ou ausente (❌).
    * **Moedas, Saúde e Felicidade**: Atributos principais do aluno.
    * **Frequência**: Barra de progresso com a porcentagem de presença.
    * **Aniversário**: Um ícone de bolo (🎂) aparece no card durante o mês de aniversário do aluno.
* **Ações Rápidas**: Ao passar o mouse sobre um card, botões para **Editar** e **Deletar** o aluno aparecem.
* **Próximo Mês**: Este botão abre um modal para inserir um valor de "Despesas Mensais". Ao confirmar, o valor é **deduzido das moedas de todos os alunos presentes na turma selecionada no filtro**. Uma animação de transição de mês é exibida.

### 📋 Chamada

* **Realizar Chamada**: Selecione uma turma e clique em **Nova Chamada**. Todos os alunos começam marcados como presentes. Desmarque os ausentes e clique em **Salvar Chamada**.
* **Histórico**: Todas as chamadas salvas são exibidas no histórico, mostrando a porcentagem de presença.
* **Editar e Deletar**: Você pode **editar** uma chamada passada ou **deletá-la** permanentemente.

### 🏆 Missões

Crie desafios para seus alunos.
* **Nova Missão**: Clique em **Nova Missão** e preencha os detalhes:
    * **Título e Descrição**: O que é a missão.
    * **Recompensa**: Quantas moedas o aluno ganha.
    * **Categoria e Dificuldade**: Para organização.

### 🛒 Loja

Crie e venda itens para os alunos usarem suas moedas.

* **Pesquisar Itens**: Use a barra de pesquisa para encontrar um item rapidamente.
* **Criar um Item**: Clique em **Novo Item** e adicione:
    * **Nome, Descrição, Imagem (URL), Valor e Categoria**.
    * **Efeitos de Saúde e Felicidade**: Defina valores positivos ou negativos que o item aplicará ao aluno no momento da compra.
* **Vender um Item**: Clique no botão **"Comprar"** em um card, selecione o aluno, e o sistema verificará se ele tem moedas suficientes. A compra deduz as moedas e aplica os efeitos de saúde/felicidade automaticamente.
* **Visualizar Imagem**: Clique na imagem de um produto para vê-la em tamanho maior.
* **Histórico de Compras**: Acompanhe todas as transações e **estorne** uma compra se necessário (as moedas serão devolvidas ao aluno).
* **Importar/Exportar Loja**: Você pode exportar apenas a lista de produtos da loja e importá-la posteriormente.

### 🔧 Ferramentas

* **Sorteio de Alunos**: Uma ferramenta para selecionar alunos aleatoriamente, individualmente ou para formar equipes.
* **Aplicar/Retirar em Massa**:
    * Selecione uma turma.
    * Insira valores nos campos de Moedas, Saúde ou Felicidade.
    * Clique em **"Aplicar"** para somar os valores a todos os alunos presentes na turma.
    * Clique em **"Retirar"** para subtrair os valores.

### 📊 Relatórios

Uma visão geral do desempenho da turma, incluindo:
* Top 5 Alunos com mais moedas.
* Aniversariantes do mês.
* Frequência geral da turma.
* Alunos com maior e menor frequência.

---

## 💾 Gerenciamento de Dados (MUITO IMPORTANTE)

* **Backup (Exportar)**:
    * Na barra lateral, clique em **Exportar Dados**.
    * Um arquivo `.json` será baixado com **todos os dados** da sua plataforma (alunos, missões, loja, etc.).
    * **Faça isso regularmente para não perder seu trabalho!**
* **Restauração (Importar)**:
    * Clique em **Importar Dados** e selecione um arquivo de backup (`.json`).
    * **Atenção**: Isso irá **sobrescrever todos os dados atuais** com os dados do arquivo.

Com este guia, você está pronto para transformar sua sala de aula com o **Gestão Maker**!
