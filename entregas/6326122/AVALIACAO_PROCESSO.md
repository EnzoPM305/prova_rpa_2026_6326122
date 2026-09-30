# Ficha de Avaliação de Processo (PDD) — Questão 5

> MOLDE. Copie para `entregas/SEU_RA/` e preencha. Escolha **um** cenário (A ou B).

**Cenário escolhido:** A

1. **Nome do processo e descrição resumida:**
   Nome: Renomeação e Arquivamento Automático de Comprovantes em PDF.

   Descrição: Processo que realiza a varredura diária de um diretório contendo comprovantes recebidos em formato PDF, identifica informações específicas no nome do arquivo (como data e número do documento), renomeia-os seguindo um padrão institucional pré-definido e os organiza em subpastas por ano/mês no diretório de destino.

2. **Volume / frequência estimados:**
   Frequência diária, com volume estimado de dezenas a centenas de comprovantes processados por lote todos os dias ao final do expediente.

3. **As entradas são estruturadas?** (sim/não + justificativa)
   Sim. O formato de arquivo é padronizado em PDF e as informações necessárias para o processamento seguem uma regra estipulada de nomenclatura (padrão legível de data e número do documento no nome do arquivo).

4. **As regras são claras e determinísticas?** (sim/não + justificativa)
   Sim. A lógica é 100% baseada em regras condicionais e expressões regulares (regex) sem necessidade de julgamento humano ou tomada de decisão subjetiva: se o arquivo for PDF e contiver o padrão esperado, aplica-se a transformação de nome e a movimentação de pasta.

5. **Veredito — o processo é elegível a RPA?** (justifique com base em regras
   claras, dados estruturados e repetibilidade)
   Sim, o processo é altamente elegível a RPA. Ele cumpre todos os pilares essenciais para automação: lida com dados estruturados (entradas em PDF com padrão de nome fixo), executa tarefas altamente repetitivas baseadas em regras estritamente determinísticas (extração, renomeação e movimentação de arquivos) e elimina tarefas manuais operacionais de baixo valor agregado com taxa de erro zero.
