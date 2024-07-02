## Atividade Prática: Gerenciamento de Tarefas com Manipulação de Dados em Memória

- Contexto
  - Você precisa refatorar a aplicação de gerenciamento de tarefas para utilizar IoC e Injeção de Dependências. A aplicação deve ser capaz de gerenciar tarefas (adicionar, listar, atualizar e remover) e utilizar serviços de notificação (por e-mail e SMS) para notificar o usuário sobre a adição de novas tarefas.


- Criar uma Interface de Serviço de Notificação:
  - Crie uma interface NotificacaoService com um método enviarNotificacao.


- Implementar Serviços de Notificação:
  - Crie duas classes que implementam a interface NotificacaoService: EmailNotificacaoService e SMSNotificacaoService.
  - Cada classe deve implementar o método enviarNotificacao para simular o envio de uma notificação.


- Refatorar o serviço de gerenciamento de Tarefas:
  - Crie uma classe TarefaService que use o serviço de notificação.
  - Use injeção de dependências (por construtor) para injetar a dependência do serviço de notificação no cliente de tarefas.
  - Adicione os métodos adicionar, atualizar, remover e listar que notifique o usuário no final da execução.
    - Utilize partes do código da classe TaskServlet original para construção de tais métodos.


- Atualizar o Servlet de Gerenciamento de Tarefas:
  - Atualize o servlet TaskServlet para utilizar a classe TarefaService ao invés de gerenciar diretamente as tarefas.
  - Use injeção de dependências para configurar o serviço de notificação utilizado pelo TarefaService.