# Regras de Negócio do SentinelTrade

- RN01 - Compra: o investidor só pode comprar ativos se tiver saldo suficiente para a ordem.
- RN02 - Venda: o investidor só pode vender a quantidade de ativos que possui disponível na carteira.
- RN03 - Ordem duplicada: a mesma ordem não pode ser processada ou executada duas vezes.
- RN04 - Status da ordem: uma ordem executada, rejeitada ou cancelada não pode voltar para o estado inicial.
- RN05 - Auditoria: toda mudança de status de uma ordem deve ser registrada.
- RN06 - Acesso administrativo: apenas usuários autorizados podem acessar as funções de administrador.
- RN07 - Falha na corretora simulada: se a corretora simulada falhar, a ordem não pode ser apagada e a carteira não pode ser alterada de forma incorreta.
- RN08 - Dados do investidor: cada investidor só pode consultar suas próprias informações.
