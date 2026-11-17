# Matriz de Rastreabilidade do SentinelTrade

| Requisito | Caso de uso associado | Diagrama futuro | Controle técnico |
|---|---|---|---|
| RF05 - Comprar ativos | Enviar ordem de compra | Atividade, sequência e estados | Verificar saldo, limite e evitar ordens duplicadas. |
| RF06 - Vender ativos | Enviar ordem de venda | Atividade, sequência e estados | Verificar se o investidor possui os ativos disponíveis. |
| RF08 - Validar ordens | Validar ordem | Atividade e sequência | Verificar os dados da ordem e os limites de risco. |
| RF10 - Registrar auditoria | Registrar auditoria | Classes, componentes e implantação | Guardar os registros das operações e mudanças de status. |
| RNF01 - Segurança | Autenticar-se com MFA | Casos de uso, componentes e implantação | Proteger senhas, confirmar o segundo código e controlar o acesso. |
| RNF06 - Confiabilidade | Transmitir ordem à corretora | Sequência, estados e implantação | Evitar o processamento duplicado e tratar falhas de comunicação. |
