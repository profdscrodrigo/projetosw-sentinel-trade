# Requisitos do SentinelTrade

## Sobre o sistema

O SentinelTrade é um sistema que simula a negociação de ativos financeiros. O investidor pode acessar sua conta, consultar saldo, carteira e cotações, além de enviar e cancelar ordens de compra e venda.

O sistema precisa verificar saldo, quantidade de ativos e limites antes de aceitar uma ordem. As operações e as mudanças de status também devem ficar registradas.

## Atores

- Investidor: consulta os dados da conta e faz operações.
- Administrador: gerencia os ativos e as configurações do sistema.
- Analista de Risco: acompanha e ajusta os limites das operações.
- Corretora/Bolsa Simulada: recebe as ordens e informa o resultado.
- Provedor de Cotações: fornece os preços simulados dos ativos.
- Serviço de Notificação: envia avisos sobre as ordens.
- Serviço de Auditoria: registra as operações e mudanças realizadas.

## Requisitos funcionais (RF)

São as funções que o sistema precisa ter.

- RF01 - Login: permitir que o usuário entre na conta.
  - Critério de aceitação: usuário com dados corretos entra; dados incorretos não permitem o acesso.
- RF02 - MFA: pedir um segundo código para confirmar o login.
  - Critério de aceitação: o acesso só é liberado com o código correto.
- RF03 - Consultar carteira: mostrar saldo, ativos e quantidades do investidor.
  - Critério de aceitação: a carteira mostra quantidade, preço médio e valor estimado dos ativos.
- RF04 - Consultar cotações: mostrar os preços dos ativos disponíveis.
  - Critério de aceitação: são mostrados o preço, o horário e a variação simulada.
- RF05 - Comprar ativos: permitir o envio de uma ordem de compra.
  - Critério de aceitação: a ordem só é aceita se houver saldo e limite disponíveis.
- RF06 - Vender ativos: permitir o envio de uma ordem de venda.
  - Critério de aceitação: a ordem só é aceita se o investidor tiver a quantidade necessária.
RF07 - Cancelar ordens: permitir o cancelamento de ordens pendentes.
  - Critério de aceitação: apenas ordens pendentes podem ser canceladas.
- RF08 - Validar ordens: verificar os dados, o saldo, a posição e os limites antes de enviar a ordem.
  - Critério de aceitação: ordens inválidas ou acima dos limites não são enviadas.
- RF09 - Consultar status: mostrar o andamento e o histórico das ordens.
  - Critério de aceitação: o investidor consegue ver o status atualizado de cada ordem.
- RF10 - Registrar auditoria: guardar os principais eventos das ordens.
  - Critério de aceitação: criação, validação, rejeição, cancelamento e execução ficam registradas.
- RF11 - Enviar notificações: avisar o investidor sobre eventos das ordens.
  - Critério de aceitação: o sistema gera avisos quando uma ordem é executada, rejeitada, cancelada ou apresenta falha.
- RF12 - Gerenciar ativos: permitir que o administrador altere ativos e parâmetros do sistema.
  - Critério de aceitação: as alterações ficam registradas para consulta.

## Requisitos não funcionais (RNF)

São condições que o sistema deve respeitar.

- RNF01 - Segurança: proteger senhas com hash, usar MFA, controlar o acesso e verificar os dados recebidos.
- RNF02 - Integridade: uma ordem deve ter investidor, ativo, tipo, quantidade e preço válidos.
- RNF03 - Auditoria: os registros de eventos importantes devem ser guardados e protegidos contra alterações indevidas.
- RNF04 - Disponibilidade: uma falha em um serviço externo não pode alterar incorretamente as ordens ou a carteira.
- RNF05 - Desempenho: consultas de carteira e cotações devem responder em tempo adequado para uma simulação.
- RNF06 - Confiabilidade: a mesma ordem não pode ser processada duas vezes por causa de reenvio ou falha de comunicação.
- RNF07 - Manutenibilidade: o código, a documentação, o banco de dados e os diagramas devem estar organizados no repositório.
- RNF08 - Privacidade: somente usuários autorizados podem acessar os dados de cada investidor.
