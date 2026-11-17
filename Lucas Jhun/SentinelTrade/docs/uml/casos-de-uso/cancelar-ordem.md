# Cancelar ordem

## Nome
Cancelar ordem.

## Ator principal
Investidor.

## Objetivo
Permitir que o investidor cancele uma ordem que ainda está pendente.

## Pré-condições
- O investidor deve estar logado com MFA.
- A ordem deve pertencer ao investidor e estar pendente.

## Fluxo principal
1. O investidor acessa suas ordens e escolhe uma para cancelar.
2. O sistema verifica se a ordem pertence a ele e ainda está pendente.
3. O sistema solicita o cancelamento à corretora simulada, quando necessário.
4. Após a confirmação, o sistema muda o status para cancelada.
5. O sistema registra o cancelamento na auditoria e avisa o investidor.

## Fluxos alternativos
- Se a ordem já foi executada, rejeitada ou cancelada, o sistema não permite cancelar novamente.
- Se a ordem for de outro investidor, o acesso é negado.
- Se houver falha na corretora simulada, o sistema informa o problema e não marca a ordem como cancelada sem confirmação.

## Pós-condições
- Se o cancelamento for confirmado, a ordem fica com status de cancelada e o evento é registrado.
- Se o cancelamento não for possível, o status da ordem não é alterado incorretamente.

## Regras de negócio
RN04, RN05, RN07 e RN08.

## Requisitos relacionados
RF07, RF09, RF10 e RF11; RNF01, RNF03, RNF04 e RNF08.
