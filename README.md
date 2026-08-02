# JirauLog 2.0 — Correção funcional

Esta versão restaura a regra original do projeto: ser mais prática que uma planilha.

## Restaurado/corrigido
- Painel matricial por material e por serviço.
- Um material pode participar simultaneamente de Escoramento de Viga, Escoramento de Laje, Travamento de Viga, Travamento de Pilar e Reescoramento.
- Controle principal em unidades; peso calculado automaticamente para cargas.
- Busca por código/descrição e filtro por serviço.
- Importação de planilhas no formato matricial ou no formato serviço + quantidade.
- Cadastro manual com cinco campos de distribuição por serviço.
- Remessa automática por prioridade e limite de peso usando o saldo de cada serviço.
- Remessa manual separada por material e serviço.
- Migração automática da base antiga para o novo modelo sem apagar dados.
- Dashboard por serviço atualizado para usar a matriz real.

## Preservado
Obras, remessas, separação/conferência, devoluções, aditivos, relatórios, backup e identidade visual Jirau.

## Regra de dados
- Quantidades e movimentações: unidades do material.
- Planejamento do caminhão: kg calculados por quantidade × peso unitário.

## Compilação
```bash
flutter create .
flutter pub get
flutter build apk --release
```

O ambiente onde esta correção foi produzida não possui Flutter/Dart; portanto, a análise estática final e a compilação do APK devem ser feitas em um ambiente Flutter.

## Versão 3.1 Web/PWA

A base Operator agora inclui estrutura web responsiva, manifesto instalável e persistência SQLite no IndexedDB. Consulte `WEB_PWA.md` para os comandos de execução e publicação.

## Versão 3.2 — Fase 1

A fundação do aplicativo foi consolidada. O banco está na versão 8, com migrações centralizadas, índices, integridade, metadados e histórico técnico. Consulte `FASE_1_FUNDACAO.md`.


## Versão 3.4 — Importação operacional da obra

- Upload do contrato diretamente na Tela Única da Obra.
- Pré-visualização antes de gravar dados.
- Associação automática com o Cadastro Mestre.
- Padronização de código, descrição, unidade e peso.
- Identificação de materiais novos e divergentes.
- Modos **Atualizar e acrescentar** ou **Substituir lista**.
- Substituição bloqueada quando já existem movimentações.
- Atualização preserva remessas, devoluções, aditivos e histórico.


## Versão 3.6 — Fluxo completo

A Tela Única agora inclui devolução rápida, aditivo rápido, histórico unificado e acesso direto aos relatórios da obra.
