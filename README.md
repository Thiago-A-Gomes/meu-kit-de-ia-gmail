# Meu Kit de IA

Desafio de Projeto da [DIO](https://dio.me): monte o seu kit de IA para o dia a dia e delegue uma tarefa real, com você no comando.

Este repositório adapta o kit do Expert Bruno Lima a uma tarefa recorrente: revisar mensagens antigas do Gmail com critérios explícitos, preservar mensagens importantes e documentar cada execução.

**Copie → adapte → teste → confira → melhore**

## O Que Tem no Kit

| Pasta | Para que serve |
|---|---|
| [01-prompts](01-prompts) | Pedidos prontos para adaptar |
| [02-templates](02-templates) | Estruturas para bom pedido, pesquisa e delegação |
| [03-checklists](03-checklists) | Revisão de respostas e tarefas delegadas |
| [04-skills](04-skills) | Orientações para criação de skills |
| [05-delegacao-e-automacao](05-delegacao-e-automacao) | Gatilhos, supervisão e checkpoints |

---

## Minha Entrega

### Minha Tarefa Real

Escolhi organizar periodicamente o Gmail para reduzir mensagens antigas que ocupam espaço e dificultam encontrar o que é importante. A rotina foi configurada para acontecer a cada três dias. A revisão considera somente mensagens anteriores aos dois meses que antecedem o mês atual; para esta execução, o limite foi 1º de setembro de 2026.

### Meus Atalhos

Adaptei o modelo de prompts e o template de delegação. Mantive como regras fixas a proteção de mensagens com estrela, os assuntos que devem ser preservados e a revisão da idade da mensagem. O período analisado e os números do relatório mudam em cada execução.

**Atalho 1 — classificar mensagens**

```text
Revise mensagens do Gmail recebidas antes do limite de data informado. Para cada mensagem, classifique como “Mover para a Lixeira”, “Manter” ou “Revisar”.

Regra absoluta: nunca mova para a Lixeira uma mensagem com estrela, mesmo que pareça promoção, spam ou reprovação.

Considere para a Lixeira somente promoções comerciais claras, mensagens promocionais da MANUAL, avisos antigos de driver AMD e reprovações explícitas de processos seletivos. Preserve mensagens sobre aluguel, pagamentos, bancos e segurança, compras, pedidos e entregas, cursos e certificados, e-mails importantes e mensagens ambíguas. Preserve também etapas positivas de seleção, convites para entrevista, segunda etapa e testes técnicos.

Use a data-limite informada e não mexa em mensagens mais recentes. Antes de mover qualquer mensagem, confira novamente a estrela, a data e a categoria. Mova apenas para a Lixeira do Gmail, que permite recuperação; nunca exclua permanentemente. Informe contagens por categoria e qualquer incerteza.
```

**Atalho 2 — registrar a execução**

```text
Ao terminar a revisão do Gmail, gere um relatório em um único PDF e envie-o por e-mail para mim. Registre a data da execução, o período analisado, as quantidades movidas por categoria, os itens preservados, as exceções e limitações encontradas.

Antes de mover mensagens, registre os metadados necessários para conferir o resultado (data, remetente, assunto e motivo), sem copiar corpos, anexos, códigos de autenticação, valores ou comprovantes. No relatório, apresente um resumo claro e proteja dados financeiros. 
```

### Minha Delegação

```text
Objetivo: revisar o Gmail a cada três dias e reduzir mensagens antigas que sejam claramente dispensáveis.

Contexto: analisar somente mensagens recebidas antes do limite de data definido para cada rotina. Classificar promoções comerciais, mensagens da MANUAL, avisos de driver AMD e reprovações explícitas de processos seletivos.

Recursos: usar a caixa do Gmail conectada e produzir um relatório em PDF enviado por e-mail para mim.

Limites: nunca mover mensagens com estrela para a Lixeira. Preservar mensagens sobre aluguel, pagamentos, bancos, segurança, compras, pedidos, entregas, cursos, certificados, etapas positivas de seleção, convites, segunda etapa, testes técnicos e qualquer mensagem ambígua. Não tocar em mensagens mais recentes que o limite. Não excluir permanentemente. Não expor conteúdo financeiro ou dados pessoais no relatório.

Critério de sucesso: somente mensagens antigas e claramente enquadradas nas categorias autorizadas vão para a Lixeira; nenhuma mensagem com estrela ou de categoria protegida é movida; o relatório informa período, contagens, exceções e limitações.
```

### O Plano da IA

Antes da execução, defini as categorias que poderiam ser movidas, as mensagens que precisavam ser preservadas e o limite de idade. Acrescentei a regra prioritária de nunca apagar mensagens com estrela. Também estabeleci que a ação deve ser apenas mover para a Lixeira, que é recuperável, e que mensagens ambíguas devem ser mantidas.

### O Resultado

Na execução registrada em 18 de novembro de 2026, 74 mensagens foram movidas para a Lixeira do Gmail, sem exclusão permanente:

- 16 reprovações explícitas de processos seletivos;
- 16 mensagens promocionais da MANUAL;
- 23 avisos antigos de driver AMD;
- 19 promoções comerciais claras.

Nenhuma mensagem com estrela foi movida. A busca por spam antigo não encontrou mensagens. Mensagens protegidas ou ambíguas foram mantidas.

Um relatório em PDF foi enviado por e-mail para mim. Nesta execução, a ferramenta não permitiu recuperar todos os metadados individuais depois da movimentação; por isso, o PDF registra as contagens e a limitação, mas não contém uma lista completa de remetentes e assuntos. A instrução foi ajustada para que as próximas rotinas registrem data, remetente, assunto e motivo **antes** de mover cada mensagem.


> As capturas originais da caixa de entrada não foram publicadas para proteger mensagens pessoais e financeiras. Este registro apresenta apenas critérios e totais; o PDF foi enviado de forma privada.

### Como Foi para Você

A revisão reduziu mensagens promocionais e avisos antigos sem remover mensagens sinalizadas com estrela. Ao organizar o processo, aprendi a transformar preferências em critérios claros, definir exceções e conferir o que foi feito. Também identifiquei uma melhoria importante: registrar os dados de cada mensagem antes de movê-la, para que os próximos relatórios tenham uma trilha de conferência mais completa.
