# Enviar ordem de compra

## Nome
Enviar ordem de compra.

## Ator principal
Investidor.

## Objetivo
Permitir que o investidor envie uma ordem de compra de um ativo na bolsa simulada.

## Pré-condições
- O investidor deve estar logado com MFA.
- O ativo deve estar disponível no sistema.

## Fluxo principal
1. O investidor escolhe o ativo e informa a quantidade e o preço.
2. O sistema verifica os dados, o saldo, os limites e se a ordem já foi enviada.
3. Se estiver tudo certo, o sistema registra a ordem e envia para a corretora simulada.
4. A corretora simulada informa o resultado da ordem.
5. O sistema atualiza o status, registra o evento na auditoria e mostra o resultado ao investidor.

## Fluxos alternativos
- Se o saldo for insuficiente ou o limite for excedido, a ordem não é enviada.
- Se os dados forem inválidos ou o ativo estiver indisponível, o sistema informa o problema.
- Se a corretora simulada falhar, a ordem fica registrada, sem alterar a carteira incorretamente, e o investidor é avisado.

## Pós-condições
- Se o envio funcionar, a ordem fica registrada com seu status.
- Se a ordem for recusada, o motivo fica informado e o evento é registrado.

## Regras de negócio
RN01, RN03, RN04, RN05 e RN07.

## Requisitos relacionados
RF05, RF08, RF09, RF10 e RF11; RNF01, RNF02, RNF03, RNF04 e RNF06.
