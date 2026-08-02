# Auditoria de correções — JirauLog 2.0

## Problemas corrigidos
1. Modelo antigo limitava cada material a um único serviço.
2. Painel matricial havia sido substituído por uma lista genérica.
3. Remessa automática priorizava linhas de material, não saldos por serviço.
4. Controle visual dava prioridade ao kg em vez das unidades.
5. Busca da tela de materiais era apenas decorativa.
6. Importador não reconhecia planilhas com colunas separadas por serviço.

## Compatibilidade
Registros antigos são migrados para a coluna do serviço legado. Remessas antigas recebem o serviço que existia no material na versão anterior.

## Ponto que ainda exige teste real
Compilação Flutter, abertura do banco migrado em Android e teste com a PLANILHA MESTRE real.
