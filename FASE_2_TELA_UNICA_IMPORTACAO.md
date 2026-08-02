# Fase 2 — Tela Única da Obra e importação assistida

Esta etapa conecta o Cadastro Mestre ao fluxo operacional da obra.

## Fluxo

1. Abrir a obra.
2. Clicar em **Importar planilha**.
3. Selecionar `.xlsx`, `.xls` ou `.ods`.
4. Revisar a prévia com materiais vinculados, padronizados e novos.
5. Escolher atualizar/acrescentar ou substituir.
6. Confirmar e continuar na mesma tela.

## Segurança

- Obras com movimentações não podem substituir toda a lista.
- Atualização procura primeiro o vínculo mestre, depois código e descrição/unidade.
- Materiais existentes mantêm seus IDs, preservando os relacionamentos.
- Materiais desconhecidos são criados provisoriamente no Cadastro Mestre.
