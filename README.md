# Assistente Portaria 1070 - Cálculo Automático de Resíduo e Complemento de Pensão por Morte

Assistente especializado para servidores do INSS que calcula automaticamente Complemento Positivo (CP) ou Complemento Negativo (CN) em pensão por morte (B21), gerando despachos prontos para copiar e colar conforme Portaria DIRBEN/INSS Nº 1.070/2022.

## Objetivo Principal

Este projeto visa auxiliar servidores do INSS na análise e cálculo de valores de pensão por morte (B21), identificando automaticamente se há **Complemento Positivo (CP)** ou **Complemento Negativo (CN)** pós-óbito, conforme os itens 7 e 8 do Anexo I da Portaria DIRBEN/INSS Nº 1.070/2022. A ferramenta gera **despachos prontos no formato "copiar e colar"**, economizando tempo e reduzindo erros de cálculo.

## Funcionalidades Principais

* **Cálculo Automático de Resíduo**: Processa dados do HISCRE, Data do Óbito (DO) e Mensalidade Reajustada (MR) para calcular valores a receber versus valores recebidos.
* **Identificação de CP ou CN**: Determina automaticamente se o caso se enquadra no Item 7 (Resíduo - CP) ou Item 8 (Recebimento após óbito - CN).
* **Despacho Pronto**: Gera texto formatado para copiar e colar diretamente no sistema, incluindo cálculos simplificados e fundamentação legal.
* **Separação de 13º Salário**: Deduz automaticamente valores proporcionais de 13º salário dos cálculos.
* **Consultoria sobre Portaria 1070**: Responde dúvidas sobre Pesquisa Externa, Justificação Administrativa, Ofícios e outros procedimentos administrativos.

## Para Quem é Destinado

Esta ferramenta é destinada a **servidores do INSS** que trabalham com:
* Análise de Pensão por Morte (B21)
* Cálculo de resíduos e complementos pós-óbito
* Aplicação da Portaria DIRBEN/INSS Nº 1.070/2022
* Tarefas dos Serviços de Centralização da Análise de Benefícios (CEABS)

## Como Usar

### Para Cálculo de Resíduo/Complemento:

1. **Forneça os 3 dados essenciais**:
   - Data do Óbito (DO)
   - Valor da Mensalidade Reajustada (MR)
   - Dados do HISCRE do ano corrente (para verificar recebimentos pós-óbito. Eu copio todo o Hiscre do Sibepu e colo no chat do LLM)

2. **Receba o resultado automático** contendo:
   - Cálculo simplificado (formato manual)
   - Identificação se é CP ou CN
   - Despacho completo com fundamentação legal
   - Indicação de tarefa a ser criada (se CP)

3. **Copie e cole** o despacho diretamente no sistema.

### Para Consultas sobre Portaria 1070:

1. Faça sua pergunta específica sobre a Portaria ou procedimentos administrativos.
2. Receba resposta baseada estritamente no conteúdo oficial da norma.

## Requisitos

* Um Large Language Model (LLM) capaz de processar o prompt fornecido
* Acesso aos dados: Data do Óbito, MR e HISCRE
* Documento da Portaria DIRBEN/INSS Nº 1.070/2022 (incluído na base de conhecimento)

## Exemplo de Uso

**Entrada do servidor:**
```
DO: 30/09/2024
MR: R$ 1.518,00
HISCRE: [dados do histórico de crédito]
```

**Saída automática (exemplo CN):**
```
VALORES A RECEBER:
30 DIAS SETEMBRO = 1.518,00.
9 MESES 13º SALÁRIO = 1138,50.
TOTAL RECEBIDO = 2.656,50.

---

VALORES RECEBIDOS:
30 DIAS SETEMBRO = 1.518,00
12 MESES 13º SALÁRIO = 1.518,00
TOTAL RECEBIDO = 3.036,00

---

DIFERENÇA TOTAL:
COMPLEMENTO NEGATIVO DE R$ 379,50.

Obs.: não será lançado qualquer Complemento Negativo, pois...
[texto completo do Item 8]
```

## Limitações e Recomendações

⚠️ **IMPORTANTE**: Esta ferramenta foi desenvolvida para auxiliar o trabalho do servidor, mas **cada servidor é responsável pelo seu próprio trabalho**. 

Recomenda-se:
* Verificar todos os cálculos apresentados
* Checar a fundamentação legal aplicada
* Conferir se os dados informados estão corretos
* Validar o resultado antes de finalizar o despacho

A ferramenta **NÃO inventa dados ou alucina** - baseia-se estritamente no conteúdo da Portaria 1070 e nos dados fornecidos pelo servidor. No entanto, a responsabilidade final pela correção e adequação do trabalho é do servidor.

## Vantagens

✅ Economia significativa de tempo
✅ Redução de erros de cálculo manual
✅ Padronização dos despachos
✅ Fundamentação legal automática
✅ Formato pronto para "copiar e colar"
✅ Menos suscetível a falhas humanas

## Contato

Para dúvidas ou sugestões sobre esta ferramenta:
📧 **wanderleyamorim.com@gmail.com**

---

**Nota**: Esta ferramenta é um auxiliar administrativo e não substitui o conhecimento técnico e a responsabilidade do servidor do INSS na análise e decisão dos casos.
E eu tenho usado este GEN do GEMINI como LLM atualmente: https://gemini.google.com/gem/15DqxWjWRww1pcseAaocgxeKSaZND3nV2?usp=sharing 
