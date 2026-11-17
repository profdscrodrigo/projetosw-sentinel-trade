# SentinelTrade

Disciplina: Projeto de Software  
Aluno: Lucas Jhun  
RA: 10395572

## Sobre o projeto

O SentinelTrade é um projeto de sistema para simular a compra e venda de ativos financeiros.

A ideia é que um investidor consiga acessar sua conta, consultar o saldo e a carteira, ver cotações, enviar ordens de compra ou venda e acompanhar o andamento dessas ordens. O sistema também deve verificar se o usuário tem saldo ou ativos suficientes antes de aceitar uma operação.

O projeto utiliza apenas dados e operações simuladas, sem dinheiro real.

## Tecnologias

- Linguagem escolhida para a implementação: Python 3.
- Banco de dados escolhido: SQLite.
- VS Code: para editar os arquivos.
- Draw.io (diagrams.net): para criar os diagramas UML.
- Git e GitHub: para organizar e entregar o projeto.
- Dependências: na N1 não é necessário instalar bibliotecas para executar o sistema. Para a implementação, a ideia é usar o módulo sqlite3 do Python.

## Execução

Na N1, o projeto contém apenas a documentação e os diagramas UML. A implementação será realizada nas próximas etapas.

## Organização dos arquivos

Estrutura prevista para o repositório:

```text
SentinelTrade/
├── README.md
├── .gitignore
├── .env.example
├── docs/
│   ├── requisitos/
│   │   ├── requisitos.md
│   │   ├── regras-de-negocio.md
│   │   └── matriz-rastreabilidade.md
│   ├── uml/
│   │   └── casos-de-uso/
│   │       ├── casos-de-uso.drawio
│   │       ├── enviar-ordem-compra.md
│   │       ├── enviar-ordem-venda.md
│   │       └── cancelar-ordem.md
│   └── evidencias/
├── src/
├── tests/
├── database/
│   ├── schema.sql
│   └── seed.sql
└── diagrams/
```

Os arquivos serão adicionados conforme o trabalho for sendo desenvolvido.
