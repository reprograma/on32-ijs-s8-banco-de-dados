# Desafio da semana

## 👉 Objetivos de aprendizagem do desafio 🎯

- Compreender os conceitos de banco de dados relacionais e como integrá-los em uma aplicação.
- Implementar e configurar um banco de dados PostgreSQL.
- Utilizar um ORM (Object-Relational Mapping) para gerenciar interações com o banco de dados.
- Criar e gerenciar transações e relatórios financeiros.

## 👉 Implementação com Banco de Dados

Seu desafio é adicionar um banco de dados PostgreSQL à aplicação Reprograma Bank, implementar a gestão de transações e criar relatórios financeiros gerados pelo gerente, acessíveis a todos os clientes.

## 👉 Requisitos de negócio

- Adicionar banco de dados PostgreSQL e ORM.
- Implementar extrato de transações da conta.
- Adicionar Relatório de prestação de contas diário e semanal do banco.
  - O gerente gera o relatório.
  - Qualquer Cliente pode acessar qualquer relatório gerado de qualquer data.
  - O banco guarda os relatórios de todos os anos.

```md
+---------------------------------+
| Cliente |
+---------------------------------+
| - nomeCompleto: string |
| - id: string |
| - endereco: string |
| - telefone: string |
| - contas: ContaBancaria[] |
| - gerente: Gerente |
+---------------------------------+
| + constructor(...) |
| + abrirConta(conta: ContaBancaria): void |
| + fecharConta(conta: ContaBancaria): void |
| + mudarTipoConta(conta: ContaBancaria, novoTipo: string): void |
+---------------------------------+
|
|
+--------+---------+
| |
+----v----+ +------v-----------------------------------+
| Conta | | ContaCorrente |
+---------+ +------------------------------------------+
| # saldo | | # chequeEspecial: number |
+---------+ +------------------------------------------+
| depositar(valor: number): void |
| sacar(valor: number): void |
| verificarSaldo(): number |
| transferir(destino: ContaBancaria, valor: number): void |
| extrato(): Transacao[] |
+-----------------------------------------------------------+
^
|
+-------+-------------------------------------------------+
| |
| ContaPoupanca |
+------------------------------------------------------ --+
| # taxaJuros: number |
+---------------------------------------------------------+
| calcularTaxa(): number |
| transferir(destino: ContaBancaria, valor: number): void |
| extrato(): Transacao[] |
+---------------------------------------------------------+

+-----------------------+
| Gerente |
+-----------------------+
| - nomeCompleto: string|
| - id: string |
| - clientes: Cliente[] |
+-----------------------+
| + constructor(...) |
| + adicionarCliente(cliente: Cliente): void |
| + removerCliente(cliente: Cliente): void |
| + abrirConta(cliente: Cliente, tipoConta: string): void |
| + fecharConta(cliente: Cliente, conta: ContaBancaria): void |
| + mudarTipoConta(cliente: Cliente, conta: ContaBancaria, novoTipo: string): void |
| + gerarRelatorio(data: Date): Relatorio |
+-----------------------+

+-----------------------+
| Transacao |
+-----------------------+
| - id: string |
| - data: Date |
| - tipo: string |
| - valor: number |
| - conta: ContaBancaria|
+-----------------------+
| + constructor(...) |
+-----------------------+

+-----------------------+
| Relatorio |
+-----------------------+
| - id: string |
| - data: Date |
| - transacoes: Transacao[] |
+-----------------------+
| + constructor(...) |
| + gerarRelatorio(): void |
| + acessarRelatorio(data: Date): Relatorio |
+-----------------------+
```
