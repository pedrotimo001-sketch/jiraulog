# JirauLog 3.2 — Fase 1: Fundação e Banco

Esta fase consolida a base técnica antes da próxima interface.

## Entregue

- Estrutura separada para schema, migrações, integridade e repositórios.
- Banco atualizado para a versão 8.
- Migração segura das versões anteriores.
- Tabelas de metadados e histórico técnico (`app_metadata` e `activity_log`).
- Índices adicionais para busca por obra, código, descrição, status e serviço.
- Validações de conferência de remessa no próprio banco.
- Bloqueio de exclusão de materiais que já possuem movimentações.
- Bloqueio de substituição integral da lista após criação de remessas.
- Normalização do total contratado pela soma das quantidades por serviço.
- Diagnóstico de integridade do banco por `AppDatabase.healthCheck()`.
- Repositórios iniciais para obras e materiais.

## Regra preservada

A quantidade contratada principal é a soma de Escoramento de Viga, Escoramento de Laje, Travamento de Viga, Travamento de Pilar e Reescoramento. O peso é derivado de quantidade × peso unitário.

## Próxima fase

Tela de Obras e Tela Única da Obra consumindo os repositórios, sem alterar as automações existentes.
