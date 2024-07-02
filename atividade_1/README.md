## Atividade Prática: Implementação de um Servlet de Calculadora

- Criar um Novo Servlet:
  -  Crie um servlet chamado CalculatorServlet que manipule requisições GET.
  - O servlet deve realizar a operação matemática com base nos parâmetros recebidos na requisição.

- Implementar a Lógica do Servlet:
  - No método doGet, leia os parâmetros num1, num2, e operacao da requisição e responda com o resultado da operação.
  - operacao pode ser um valor entre: soma, subtracao, multiplicacao, divisao ○ Realize validação dos parâmetros (num1 e num2 devem ser valores numéricos).
  - Dica: utilize o método request.getParameter() para pegar um parâmetro da requisição.

- Testar o Servlet:
  - Use o Postman ou um navegador para enviar requisições GET ao servlet.
  - Verifique se as respostas são geradas corretamente.
