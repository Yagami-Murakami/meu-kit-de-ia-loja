# Registro da execução e dos testes

**Data:** 17/11/2026  
**Resultado da IA:** checklist operacional e mensagem modelo  
**Escopo dos testes:** exemplos fictícios, sem equipamento ou cliente real

## Resultado produzido

O arquivo [`checklist-triagem-notebooks.md`](checklist-triagem-notebooks.md) contém:

- Etapa de recebimento com registro do relato, condição externa, acessórios e consentimento.
- Tabela de triagem com estados para dados verificados e não verificados.
- Separação explícita entre fatos, hipóteses e pendências.
- Mensagem de andamento para o cliente, sempre sujeita a revisão.
- Aprovação humana antes de intervenções, compartilhamentos ou compromissos.

## Teste 1 — lentidão e aquecimento relatados

**Entrada simulada:** “O notebook está lento e esquenta muito”. Nenhuma medição ou diagnóstico disponível.

**Preenchimento correto:** colocar ambos em `relato do cliente`; deixar medição térmica, armazenamento e ventilação como `não testado` ou `pendente`. Não afirmar que há necessidade de limpeza, troca de pasta térmica ou formatação.

**Mensagem de teste:** “Olá! Recebemos o notebook para avaliar a lentidão e o aquecimento relatados. A avaliação ainda está pendente, por isso não temos um diagnóstico confirmado. Vamos informar os próximos passos antes de realizar qualquer serviço.”

**Conferência do texto:** não contém causa técnica, preço, prazo nem intervenção sem autorização.

## Teste 2 — equipamento não inicia

**Entrada simulada:** “O notebook não liga”. Não há confirmação de teste com fonte, bateria ou botão de energia.

**Preenchimento correto:** `não liga` permanece como relato; itens de alimentação e inicialização ficam `não testado` ou `pendente`. Não afirmar defeito na placa-mãe.

**Mensagem de teste:** “Olá! Registramos o problema informado na inicialização do notebook. Ainda precisamos realizar as verificações autorizadas para identificar a causa. Avisaremos quando houver resultado e antes de qualquer intervenção.”

**Conferência do texto:** não transforma uma suspeita em diagnóstico nem promete um resultado específico.

## Revisão com o princípio “Pare, Confira, Use”

| Verificação | Resultado |
|---|---|
| Risco de prejuízo por afirmação técnica incorreta | Mitigado por campos de teste pendente e autorização |
| Preços, datas, nomes, diagnósticos ou fontes inventados | Não identificados nos materiais |
| Diferença entre o que foi relatado e confirmado | Preservada nos dois testes simulados |
| Exposição de dados de clientes | Não há dados de clientes nos exemplos |
| Teste físico em equipamento real | **Não realizado** |
| Avaliação do responsável e uso operacional | **Pendente** |

O trabalho de elaboração foi executado e conferido **quanto à consistência textual e às regras de segurança**. Isso não significa que o procedimento já foi aprovado pelo dono da loja ou testado em produção.

> Evidência textual transparente. Anexar print autêntico do resultado da conversa para complementar o portfólio exigido pela DIO.
