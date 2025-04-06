# Board de Gerenciamento de Tarefas 📝

Este sistema permite criar e gerenciar boards para acompanhar o progresso de suas tarefas de maneira eficiente. Os boards são compostos por várias **colunas**, e cada coluna contém **cards** representando suas tarefas. O objetivo deste projeto é organizar suas atividades de maneira visual e funcional, com a possibilidade de movimentar, bloquear e excluir cards.

## Funcionalidades Principais 🚀

### 1. **Menu Inicial**
Ao iniciar o sistema, você verá um menu com as seguintes opções:

- **Criar novo board** ➕: Crie um novo board para começar a organizar suas tarefas.
- **Selecionar board** 📂: Selecione um board previamente criado para visualizar e gerenciar.
- **Excluir boards** ❌: Exclua boards que não precisa mais.
- **Sair** 🚪: Encerre o sistema.

### 2. **Estrutura de um Board**
Cada board é composto por várias colunas, e você pode personalizar o nome delas. Um board deve ter pelo menos 3 colunas:

1. **Coluna Inicial**: Onde as tarefas começam.
2. **Coluna Final**: Onde as tarefas são finalizadas e concluídas.
3. **Coluna de Cancelamento**: Onde as tarefas canceladas são movidas.

Além dessas, você pode criar **colunas adicionais de status pendente** 🕑, caso precise de etapas intermediárias.

### 3. **Regras para Movimentação dos Cards** 🔄
Dentro do board, as tarefas são representadas por **cards**. Cada card pode ser movido entre as colunas, mas com algumas regras:

- **Ordem das colunas** 🔢: As colunas têm uma ordem definida:
  - A coluna **Inicial** ➕ deve ser sempre a primeira.
  - A coluna **Final** ✅ deve ser sempre a penúltima.
  - A coluna **Cancelamento** ❌ deve ser sempre a última.
  - Você pode adicionar colunas de **status pendente** 🕑 entre a Inicial e a Final, quantas forem necessárias.

- **Movimento de cards** 📤: As tarefas (cards) devem seguir a ordem entre as colunas sem pular nenhuma etapa, exceto se forem movidas para a coluna de **Cancelamento** ❌, que pode receber cards de qualquer coluna (exceto a coluna Final ✅).

### 4. **Bloqueio e Desbloqueio de Cards**
Às vezes, você pode precisar **bloquear** um card para evitar que ele seja movido. Para bloquear um card, basta informar o **motivo do bloqueio**. Somente após o **desbloqueio** do card é que ele poderá ser movido entre as colunas.

- **Bloqueio** 🔒: Impede que o card seja movido até que seja desbloqueado.
- **Desbloqueio** 🔓: Após ser desbloqueado, o card pode ser movido para a próxima coluna.

Para bloquear ou desbloquear um card, será necessário informar um **motivo**, o que ajuda a entender por que o card está temporariamente parado ou liberado.

### 5. **Manipulando o Board e os Cards**
Depois de selecionar um board, você pode realizar várias ações nos cards, acessando o menu de manipulação:

- **Mover card para a próxima coluna** ⏩: Move a tarefa para o próximo estágio no board.
- **Cancelar card** ❌: Move a tarefa para a coluna de **Cancelamento**.
- **Criar um card** ➕: Adiciona uma nova tarefa ao board.
- **Bloquear card** 🔒: Impede a movimentação do card até que seja desbloqueado.
- **Desbloquear card** 🔓: Permite que o card seja movido novamente.
- **Fechar o board** 🚪: Encerra a sessão do board selecionado.

### 6. **Armazenamento de Informações**
Todas as informações sobre os boards, colunas e cards são armazenadas em um **banco de dados MySQL**, garantindo que as alterações feitas no board sejam salvas e preservadas entre as sessões.

### 7. **Relatórios Opcionais**
Para otimizar o gerenciamento das tarefas, o sistema pode gerar dois relatórios importantes:

- **Relatório de Tempo de Conclusão** ⏱️: Um relatório detalhado com o tempo que cada tarefa levou para ser concluída, incluindo o tempo gasto em cada coluna.
- **Relatório de Bloqueios** 🚫: Um relatório que mostra os cards que foram bloqueados, o tempo que ficaram bloqueados, e os motivos de bloqueio e desbloqueio.

### 8. **Conclusão 🎯**
Esse sistema foi projetado para ajudar você a organizar suas tarefas de maneira clara e eficiente. Você pode personalizar os boards conforme necessário, movendo suas tarefas entre as colunas e gerenciando-as com facilidade. Se alguma tarefa precisar ser bloqueada ou cancelada, o sistema fornece as ferramentas necessárias para gerenciar essas situações de forma simples e transparente.
