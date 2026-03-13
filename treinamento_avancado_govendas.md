# 📊 Treinamento Avançado — Relatórios GoVendas
## Guia Aprofundado de Interpretação e Análise para Gestores de Televendas

---

> [!IMPORTANT]
> **Nível:** Avançado — Este documento aprofunda o treinamento introdutório já realizado.
> **Pré-requisito:** Ter lido ou participado do treinamento básico de relatórios GoVendas.
> **Duração estimada:** 6 a 8 horas (dividido em módulos independentes)
> **Base de dados:** Análise realizada com filtro de **24 meses** para máxima riqueza de dados.

---

## 📋 SUMÁRIO

1. [Objetivo do Treinamento Avançado](#1-objetivo-do-treinamento-avançado)
2. [Lógica de Análise: Como os Relatórios se Conectam](#2-lógica-de-análise-como-os-relatórios-se-conectam)
3. [Módulo 1 – Desempenho Comercial (Evolução da Carteira)](#módulo-1--desempenho-comercial---validação)
4. [Módulo 2 – Planejamento de Capacidade](#módulo-2--planejamento-de-capacidade)
5. [Módulo 3 – Cobertura de Atendimento Televendas](#módulo-3--cobertura-de-atendimento---televendas)
6. [Módulo 4 – Clientes Não Atendidos por Vendedor](#módulo-4--clientes-não-atendidos-por-vendedor)
7. [Módulo 5 – Resultados de Positivação](#módulo-5--resultados-de-positivação)
8. [Módulo 6 – Cobertura de Atendimento Multicanal](#módulo-6--cobertura-de-atendimento-multicanal---validação)
9. [Cenários Avançados de Gestão](#9-cenários-avançados-de-gestão)
10. [Guia de Diagnóstico Rápido](#10-guia-de-diagnóstico-rápido)

---

## 1. OBJETIVO DO TREINAMENTO AVANÇADO

### Por que ir além do básico?

O treinamento básico te ensinou **o que cada relatório é**. Este treinamento avançado te ensina **como extrair o máximo de informação de cada tela**, elemento por elemento.

A diferença entre um gestor mediano e um gestor excelente está na **profundidade da leitura dos dados**. Um gestor mediano abre o relatório e olha um número. Um gestor excelente abre o relatório e faz cinco perguntas antes de tomar qualquer decisão.

> **Premissa central deste treinamento:**
> *Cada campo, cada coluna, cada filtro do GoVendas existe por uma razão. Quando você entende o propósito de cada elemento, a análise se torna natural e rápida.*

---

## 2. LÓGICA DE ANÁLISE: COMO OS RELATÓRIOS SE CONECTAM

### 🗺️ O Mapa Mental da Gestão Comercial

Antes de mergulhar em cada relatório, é fundamental entender a **ordem de raciocínio** que um gestor deve seguir. Analise os relatórios sempre nesta sequência:

```
PASSO 1: QUANTO TENHO?
→ Desempenho Comercial (Evolução da Carteira)
  "Quantos clientes a empresa possui? Quantos estão ativos?"

PASSO 2: CONSIGO ATENDER?
→ Planejamento de Capacidade
  "Minha equipe tem capacidade para atender todos esses clientes?"

PASSO 3: ESTOU ATENDENDO?
→ Cobertura de Atendimento Televendas
  "Os vendedores estão de fato ligando para os clientes agendados?"

PASSO 4: QUEM FICOU SEM ATENDIMENTO?
→ Clientes Não Atendidos por Vendedor
  "Quais clientes específicos foram ignorados? Por qual vendedor?"

PASSO 5: OS ATENDIMENTOS GERARAM VENDA?
→ Resultados de Positivação
  "Das ligações realizadas, quantas converteram em pedidos?"

PASSO 6: VISÃO COMPLETA DA OPERAÇÃO
→ Cobertura de Atendimento Multicanal
  "Além do televendas, os clientes estão sendo atendidos por outros canais?"
```

### Por que essa ordem?

Imagine que você recebe o problema: **"As vendas caíram este mês."**

Se você pular direto para o relatório de positivação, vai ver a taxa caindo — mas não vai saber **por quê**. Seguindo a sequência acima, você descobre:
- A carteira cresceu, mas a capacidade não acompanhou → vendedores sobrecarregados → menos atendimentos → menos vendas.

**A sequência revela a causa-raiz, não apenas o sintoma.**

---

## MÓDULO 1 – Desempenho Comercial - Validação

### 📍 Localização no sistema
> **Relatórios → Desempenho Comercial - Validação**
> URL: `/reports/desempenho_comercial`

---

### 🎯 Visão Geral

#### Método Feynman
> Imagine que você é dono de uma fazenda. Antes de planejar a colheita, você precisa saber: quantos hectares de terra tenho? Quais estão plantados e produzindo? Quais estão baldios? O relatório de Desempenho Comercial faz exatamente isso com sua base de clientes: mostra o "mapa da terra" que sua equipe tem para trabalhar.

#### Para que serve?
Este relatório responde a pergunta fundamental de qualquer operação comercial: **"Qual é o tamanho real da nossa oportunidade de negócio?"**

Ele mostra não apenas quantos clientes estão cadastrados, mas os classifica por **ciclo de vida** — revelando quantos estão comprando, quantos pararam de comprar e quantos nunca compraram ainda.

---

### 🖥️ Análise Completa da Tela

#### ÁREA 1: Filtros

| Filtro | Tipo | Opções disponíveis | Para que serve |
|--------|------|--------------------|----------------|
| **Filtro de Data** | Seletor de período | Últimos N meses/anos, configurável | Definir o período de análise. Use **24 meses** para ver tendências de longo prazo |
| **Supervisores** | Dropdown múltiplo | Lista de todos os supervisores cadastrados | Filtrar a análise por divisão da equipe |
| **Vendedores** | Dropdown múltiplo | Lista de todos os vendedores ativos | Detalhar a análise por vendedor específico |

> [!TIP]
> **Dica de uso:** Comece sempre com a visão completa (todos os supervisores e vendedores). Depois, se encontrar anomalia, afunile o filtro para identificar qual equipe ou vendedor está causando o problema.

---

#### ÁREA 2: Cards de KPI (Indicadores Principais)

Estes são os quatro números mais importantes do relatório. Com filtro de **24 meses**, os valores reais encontrados foram:

| Card | Valor encontrado | O que significa | Como interpretar |
|------|------------------|-----------------|-----------------|
| **Total de Clientes** | 5.084 | Total de clientes cadastrados no sistema ERP integrado | É o **teto máximo** de clientes que a empresa poderia atender |
| **Clientes Ativos** | 703 | Clientes que realizaram pelo menos uma compra no período analisado | São os clientes que **estão gerando receita** agora |
| **Clientes Inativos** | 285 | Clientes que já compraram, mas não compram há tempo | São clientes **em risco de perda** — prioridade de reativação |
| **Clientes Prospects** | 4.096 | Clientes cadastrados que **nunca compraram** | São a maior **oportunidade de crescimento** da carteira |

> [!WARNING]
> **Interpretação crítica:** Perceba que dos 5.084 clientes totais, apenas **703 (13,8%) estão ativos**. Isso significa que **86% do potencial de mercado desta empresa ainda não está sendo explorado**. Esse número deve ser o ponto de partida de qualquer reunião estratégica.

##### Como calcular os percentuais importantes:

```
Taxa de Ativação da Carteira = Clientes Ativos ÷ Total de Clientes
703 ÷ 5.084 = 13,8% → Apenas 13,8% da base potencial compra

Taxa de Inativos sobre Já Clientes = Inativos ÷ (Ativos + Inativos)
285 ÷ (703 + 285) = 28,9% → Quase 30% dos que já foram clientes pararam de comprar
```

---

#### ÁREA 3: Gráfico — Quantidade de Clientes por Ciclo de Vida

**O que mostra:** Comparação visual entre as 3 categorias (Prospects, Ativos, Inativos) em um momento específico.

**Como ler:**
- A barra de **Prospects** sempre será a maior (é a maior oportunidade)
- A barra de **Ativos** representa a saúde atual
- A barra de **Inativos** representa o risco de churn acumulado

**O que fazer:** Se a barra de Inativos estiver crescendo mês a mês no gráfico de evolução → sinal de que a empresa está perdendo clientes mais rápido do que ganha.

---

#### ÁREA 4: Gráfico — Evolução da Carteira por Ciclo de Vida

**O que mostra:** Linha do tempo mostrando como Prospects, Ativos e Inativos evoluíram mês a mês.

**Padrões e o que significam:**

| Padrão no gráfico | Diagnóstico | Ação |
|-------------------|-------------|------|
| Linha de Ativos crescendo | Operação saudável | Manter estratégia |
| Linha de Ativos estável | Estagnação | Investigar se perdas e ganhos estão se anulando |
| Linha de Ativos caindo | Crise de retenção | Priorizar reativação de inativos |
| Linha de Inativos crescendo | Clientes abandonando | Revisar qualidade de atendimento e mix de produtos |
| Linha de Prospects diminuindo | Conversão acontecendo | Positivo — monitoring se é ritmo sustentável |

---

#### ÁREA 5: Gráfico — Evolução de Clientes na Carteira (Empilhado)

**O que mostra:** Gráfico de barras empilhadas com 4 categorias por mês: Prospects, Ativos, Reativados, Inativos.

**Atenção especial para a categoria "Reativados":**
- São clientes que estavam inativos e voltaram a comprar
- Uma barra de Reativados crescente indica que a estratégia de recuperação está funcionando
- Se Reativados for sempre zero, a empresa não tem ação ativa de recuperação de inativos

---

#### ÁREA 6: Cards — Faturamento e Ticket Médio por Ciclo de Vida

| Métrica | O que revela |
|---------|-------------|
| **Faturamento por Ciclo de Vida** | Quanto cada categoria gera de receita (ex: R$ 2,4M para Ativos) |
| **Ticket Médio por Ciclo de Vida** | Valor médio de compra por categoria (ex: R$ 7.210 para Ativos) |

**Análise avançada:**
> Se o Ticket Médio de Reativados for **menor** que o de Ativos, os clientes que voltaram a comprar estão comprando menos do que antes. Isso pode indicar que a reativação foi "forçada" por promoções ou descontos, e não por fidelização genuína.

---

#### ÁREA 7: Gráfico — Clientes Planejados x Atendidos x Com Vendas

**O que mostra:** Três linhas que representam o funil de atendimento:
1. **Planejados** — quantos clientes foram agendados para contato
2. **Atendidos** — quantos realmente receberam contato
3. **Com Vendas** — quantos dos atendidos compraram

**Como usar:**
- A diferença entre Planejados e Atendidos = gap de execução (Cobertura)
- A diferença entre Atendidos e Com Vendas = gap de conversão (Positivação)
- Ambos os gaps devem ser investigados com os relatórios específicos

---

### ⚠️ Erros Comuns de Interpretação

1. **Confundir "Total de Clientes" com mercado real**: Os 5.084 clientes são clientes **já cadastrados no sistema**. O mercado potencial real pode ser muito maior — esses são apenas os que já tiveram algum contato com a empresa.

2. **Ver Prospects como problema**: Ter muitos Prospects não é ruim — é uma oportunidade. O problema é não ter um plano para convertê-los.

3. **Ignorar o gráfico de evolução e focar só nos cards**: Os cards mostram um recorte no tempo. A evolução mostra a **tendência** — que é muito mais importante para decisão estratégica.

---

### 💡 Exemplo Real de Análise

**Situação:** Gestor abre o relatório com filtro de 24 meses e vê:
- Ativos: 703 (estável nos últimos 3 meses)
- Inativos: 285 (cresceu de 210 há 6 meses)
- Prospects: 4.096 (leve queda)

**Leitura do gestor experiente:**
> "A base de ativos parou de crescer. Os inativos aumentaram 35% em 6 meses, o que indica que estamos perdendo clientes ativos — eles estão virando inativos. Ao mesmo tempo, os prospects caíram levemente, sugerindo alguma conversão. Mas não o suficiente para compensar as perdas. Próximo passo: abrir o relatório de Cobertura para entender se estamos de fato ligando para os clientes ativos."

---

## MÓDULO 2 – Planejamento de Capacidade

### 📍 Localização no sistema
> **Relatórios → Planejamento de Capacidade**
> URL: `/reports/planejamento_de_capacidade`
> **Descrição do sistema:** *"Este relatório demonstra de forma clara se a capacidade de atendimento do vendedor está condizente com o que será planejado com o GoVendas."*

---

### 🎯 Visão Geral

#### Método Feynman
> Você tem um restaurante com capacidade para 50 clientes por dia. Se 80 clientes chegarem, vai ter fila, insatisfação e serviço ruim. Se chegarem apenas 20, seus garçons ficam ociosos e você perde dinheiro. Esse relatório faz esse cálculo para cada vendedor: quantos clientes ele pode atender por mês versus quantos está sendo planejado para atender?

---

### 🖥️ Análise Completa da Tela

#### ÁREA 1: Filtros

| Filtro | Tipo | Especificidade | Para que serve |
|--------|------|---------------|----------------|
| **Supervisores** | Dropdown múltiplo | 9 supervisores disponíveis | Filtrar a visão por equipe |
| **Vendedor selecionado** | Dropdown único | Seleciona um vendedor específico | Ver análise individual detalhada |
| **Tolerância** | Campo numérico | Padrão: **0.10** (= 10%) | Margem de erro aceitável no planejamento |

##### Entendendo o campo **Tolerância** (elemento crítico)

O campo Tolerância é o mais incompreendido do relatório. Funciona assim:

```
Tolerância = 0.10 significa que:
Se a capacidade é de 330 clientes e a carteira tem até 363 (330 × 1,10),
o sistema ainda considera como "dentro da capacidade"

Ou seja: até 10% acima da capacidade é aceitável
```

**Quando ajustar a tolerância?**
- **Aumentar para 0.15 ou 0.20:** Quando a equipe é experiente e suporta um volume levemente maior
- **Diminuir para 0.05:** Quando a equipe está em treinamento ou os atendimentos são mais complexos

---

#### ÁREA 2: Cards de KPI — Visão Geral da Equipe

Com os dados reais encontrados no sistema:

| Card | Valor | O que significa |
|------|-------|----------------|
| **Vend. Cadastrados** | 26 | Total de vendedores no sistema |
| **Vend. sem Agenda** | 18 | Vendedores que não têm clientes planejados |
| **Vend. com Agenda** | 8 | Vendedores com clientes agendados para atendimento |

> [!WARNING]
> **Alerta:** 18 de 26 vendedores sem agenda significa que **69% da equipe está ociosa em termos de planejamento**. Isso é um sinal de problema sistêmico — ou a carteira não foi devidamente distribuída, ou o planejamento do mês não foi executado.

---

#### ÁREA 3: Tabela — Visão Geral de Capacidade

Esta tabela mostra, para o vendedor selecionado (ou todos), os parâmetros de capacidade:

| Coluna | Valor exemplo | Significado |
|--------|--------------|-------------|
| **Total Clientes na Carteira** | — | Todos os clientes vinculados ao vendedor |
| **Elegíveis** | — | Clientes que se qualificam para agendamento (ativos ou em processo de ativação) |
| **Capacidade Diária** | **20** | Quantos clientes o vendedor pode atender por dia útil |
| **Dias Úteis** | **22** | Dias de trabalho no mês de referência |

##### Cálculo de Capacidade Total:
```
Capacidade Total = Capacidade Diária × Dias Úteis
Capacidade Total = 20 × 22 = 440 clientes/mês

Esse é o TETO de atendimento do vendedor.
Se a carteira tiver mais de 440 clientes elegíveis, haverá sobrecarga.
```

---

#### ÁREA 4: Tabela — Capacidade x Demanda

| Métrica | Significado |
|---------|-------------|
| **Total Capacity** | Capacidade máxima mensal = 440 clientes |
| **Demand** | Número de clientes elegíveis na carteira |

**Leitura prática:**
- Demand > Capacity × (1 + Tolerância) = **SOBRECARGA** → Redistribuir clientes
- Demand < Capacity × (1 - Tolerância) = **OCIOSIDADE** → Adicionar clientes
- Demand ≈ Capacity = **EQUILÍBRIO** → Ideal

---

#### ÁREA 5: Tabela — Todos os Vendedores da Empresa

Esta é a tabela mais estratégica do relatório. Exibe **todos os vendedores** com as seguintes colunas:

| Coluna | O que mostra | Como usar |
|--------|-------------|-----------|
| **Tipo** | Categoria do vendedor no sistema | Segmentar análise por perfil |
| **Status do Planejamento Diário** | Situação do vendedor: equilibrado, sobrecarregado ou ocioso | **Principal semáforo de ação** |
| **Disponibilidade** | Capacidade disponível em % ou unidades | Identificar quem pode receber mais clientes |

##### Legenda dos Status:

| Status | Cor/indicação | O que fazer |
|--------|--------------|-------------|
| ✅ **Dentro da capacidade** | Verde | Manter |
| ⚠️ **Clientes acima da capacidade** | Vermelho/Laranja | Redistribuir imediatamente |
| ℹ️ **Não há clientes elegíveis** | Cinza | Verificar se carteira está vazia ou desatualizada |
| 📋 **Sem agenda** | Neutro | Verificar se o planejamento do mês foi feito |

---

### 🔄 Fluxo de Análise Recomendado

```
INÍCIO DO MÊS — Checklist de Capacidade:

1. Abrir o relatório sem filtrar vendedor específico
2. Ver na tabela "Todos os Vendedores":
   → Quantos estão como "Clientes acima da capacidade"?
   → Quantos estão como "Sem agenda"?
3. Para cada vendedor sobrecarregado:
   → Identificar quantos clientes estão acima da capacidade
   → Mover esses clientes para vendedores com disponibilidade
4. Para vendedores sem agenda:
   → Verificar se é início do ciclo (normal) ou problema persistente
5. Repetir análise na metade do mês para ajustes
```

---

### ⚠️ Erros Comuns de Interpretação

1. **Ver "20 clientes/dia" como rigidez:** Esse número é um parâmetro configurável no sistema, não uma lei. Se o produto vendido exige muito tempo de negociação, 20 pode ser alto demais. Se é venda simples e rápida, pode ser conservador.

2. **Ignorar vendedores "sem agenda":** Na análise inicial parece OK, mas se persistir por mais de 2 semanas, indica que esse vendedor está sem clientes planejados — e portanto, sem meta de atendimento.

3. **Analisar só a Visão Geral sem olhar o vendedor individualmente:** A visão geral esconde desequilíbrios entre vendedores. Um vendedor com 600 clientes e outro com 100 mostram "média" de 350 — que parece equilibrado, mas esconde um problema grave.

---

## MÓDULO 3 – Cobertura de Atendimento - Televendas

### 📍 Localização no sistema
> **Relatórios → Cobertura de Atendimento - Televendas**
> URL: `/reports/coverage_attendance`

---

### 🎯 Visão Geral

#### Método Feynman
> Imagine que você contratou 10 entregadores e planejou exatamente quais casas cada um deve visitar. No fim do dia, você quer saber: das casas planejadas, quantas foram de fato visitadas? Isso é cobertura. Não é se a entrega foi aceita (isso é positivação), é apenas se a visita aconteceu.

---

### 🖥️ Análise Completa da Tela

#### ÁREA 1: Filtros — Análise Detalhada

| Filtro | Tipo | Opções | Uso estratégico |
|--------|------|--------|----------------|
| **Filtro de Data** | Período configurável | Ajustado para **24 meses** | Permite ver sazonalidade e tendências anuais |
| **Supervisores** | Dropdown múltiplo | 9 supervisores | Comparar performance entre equipes |
| **Vendedores** | Dropdown múltiplo | 26 vendedores | Análise individual ou comparativa |
| **Tipo de Agendamento** | Dropdown múltiplo | Planejado (carteira) / Ruptura / Complementar | **Filtro mais estratégico deste relatório** |

##### Entendendo profundamente o filtro **Tipo de Agendamento**:

| Tipo | O que é | Quando analisar separadamente |
|------|---------|-------------------------------|
| **Planejado (carteira)** | Clientes regulares da carteira do vendedor, agendados dentro do ciclo normal | Para medir execução do planejamento padrão |
| **Ruptura** | Clientes que saíram do ciclo normal — compraram menos do esperado ou pararam de comprar | Para medir ação de recuperação de clientes |
| **Complementar** | Atendimentos extras, fora do planejamento regular | Para medir proatividade da equipe |

> [!NOTE]
> **Por que isso importa?** Uma cobertura baixa de "Planejado" é preocupante (o plano não está sendo executado). Uma cobertura baixa de "Ruptura" é crítica (os clientes em risco não estão sendo atendidos). Analise cada tipo separadamente.

---

#### ÁREA 2: Cards de KPI — Os 7 Indicadores

Com os dados reais encontrados com filtro de 24 meses:

| Card | Valor Real | O que significa | Fórmula |
|------|-----------|-----------------|---------|
| **Agendados** | **2.675** | Total de visitas/ligações planejadas no período | — Base de comparação |
| **Atendidos Dentro do Planejado** | **553** | Clientes contatados que estavam na agenda | — |
| **Agendados e Não Atendidos** | **2.122** | Clientes planejados que **não receberam contato** | 2.675 - 553 |
| **Atendidos Fora do Planejado** | **812** | Contatos realizados sem agendamento prévio | — |
| **Atendidos** | **1.365** | Total de contatos realizados (dentro + fora do plano) | 553 + 812 |
| **Positivados** | **1.360** | Dos atendidos, quantos resultaram em venda | — |
| **Cobertura de Positivação** | **99,71%** | % dos atendidos que compraram | 1.360 ÷ 1.365 |

##### Análise crítica desses números reais:

```
Taxa de Cobertura (do Planejado) = Atendidos Dentro do Planejado ÷ Agendados
= 553 ÷ 2.675 = 20,7%  ← MUITO BAIXO (meta seria >80%)

Isso indica que apenas 1 a cada 5 clientes agendados está sendo contatado.

Mas: 812 atendimentos foram "Fora do Planejado"
O que isso significa? Os vendedores estão ligando para clientes
que não estavam no plano, possivelmente deixando de lado
os que deveriam ser prioridade.

Taxa de Positivação geral = 99,71% ← Excelente
Isso significa que quando o vendedor consegue atender, quase sempre vende.
O problema NÃO é técnica de vendas — é COBERTURA.
```

> [!WARNING]
> **Conclusão desta análise:** A operação tem um problema crítico de **execução do planejamento**. Os vendedores são bons em vender (99,71% de positivação), mas não estão seguindo a carteira planejada. A gestão precisa investigar por que 2.122 clientes agendados não foram atendidos.

---

#### ÁREA 3: Gráfico — Agendas por Tipo de Atendimento (Donut/Pizza)

**O que mostra:** Distribuição dos atendimentos em 3 categorias:
- **Não atendido** (clientes que ficaram sem contato)
- **Venda verificada** (contato com venda)
- **Outro** (contato sem venda — recusa, cliente ausente, etc.)

**Como interpretar:**
- Fatia "Não atendido" grande → Problema de cobertura
- Fatia "Outro" crescendo → Contatos acontecendo mas sem converter → Investigar positivação
- Fatia "Venda verificada" dominante → Operação saudável

---

#### ÁREA 4: Gráfico — Ranking de Justificativas de Não Vendas

**Este é um dos gráficos mais valiosos e frequentemente ignorados.** Ele mostra os **motivos registrados pelos vendedores** quando um atendimento não gerou venda.

Categorias típicas:
| Justificativa | O que pode indicar |
|--------------|-------------------|
| **Preço** | Produto não competitivo ou abordagem errada |
| **Sem estoque** | Cliente com estoque alto — revisitar frequência de contato |
| **Já comprado** | Cliente comprou recentemente — contato fora do timing |
| **Cliente ausente** | Vendedor não conseguiu falar com o decisor |
| **Sem interesse** | Produto errado ou abordagem genérica |

> [!TIP]
> **Uso avançado:** Se "Preço" aparece constantemente para um vendedor específico, pode ser que ele não saiba negociar. Se "Sem interesse" domina, pode ser que ele não personalize a oferta.

---

#### ÁREA 5: Gráfico — Histórico de Atendimentos x Capacidade

**O que mostra:** Comparação ao longo do tempo entre:
- Volume de atendimentos realizados
- Capacidade disponível da equipe

**Como interpretar:**
- Linha de atendimentos **abaixo** da capacidade → Equipe ociosa ou mal aproveitada
- Linha de atendimentos **acima** da capacidade → Improvável, mas indicaria horas extras ou sobrecarga
- Linhas **próximas** → Operação bem calibrada

---

#### ÁREA 6: Tabela — Cobertura de Atendimento por Vendedor

Esta tabela é a **mais acionável** do relatório. Mostra o ranking de cobertura individual.

| Coluna | O que mostra |
|--------|-------------|
| **Cód. Vendedor** | Código identificador |
| **Nome do Vendedor** | Nome completo |
| **%** | Percentual de cobertura individual |

**Como usar esta tabela:**
1. Ordenar pelo percentual (menor para maior)
2. Os 3 primeiros da lista são prioridade de atenção gerencial
3. Verificar se o padrão é consistente ou pontual (cruzar com o histórico)
4. Reunir com vendedores na "zona vermelha" (abaixo de 60%)

---

### ⚠️ Erros Comuns de Interpretação

1. **Ver positivação alta e concluir que tudo está bem:** No caso real analisado, a positivação de 99,71% mascara uma cobertura de apenas 20,7%. A empresa está vendendo para quase todos que atende, mas está atendendo muito poucos dos planejados.

2. **Ignorar os atendimentos "Fora do Planejado":** 812 atendimentos não planejados é muito. Isso pode indicar que os vendedores estão preferindo ligar para clientes "mais fáceis" (que não estão na carteira planejada) ao invés de trabalhar a carteira designada.

3. **Não usar o filtro de Tipo de Agendamento:** Analisar Planejado, Ruptura e Complementar juntos esconde problemas específicos de cada modalidade.

---

## MÓDULO 4 – Clientes Não Atendidos por Vendedor

### 📍 Localização no sistema
> **Relatórios → Clientes Não Atendidos por Vendedor**
> URL: `/reports/not_attend_report_team`
> **Descrição do sistema:** *"Traz informações sobre os clientes agendados que não compraram e nem foram atendidos. Você poderá fazer análises por vendedor ou por supervisor."*

---

### 🎯 Visão Geral

#### Método Feynman
> Você tem uma lista de nomes de pessoas que deveriam receber uma ligação importante esta semana. Esse relatório te diz exatamente quais nomes dessa lista ficaram sem ligação, e qual funcionário era o responsável por cada um. Não é uma análise geral — é uma lista nominal de falhas específicas.

---

### 🖥️ Análise Completa da Tela

#### ÁREA 1: Filtros

| Filtro | Configuração usada | Impacto |
|--------|-------------------|---------|
| **Filtro de Data** | 24 meses | Permite identificar padrões crônicos de não atendimento |
| **Supervisores** | 9 selecionados | Visão completa da empresa |
| **Vendedores** | 26 selecionados | Visão completa |

> [!TIP]
> Para uso investigativo, filtre por **um vendedor específico** para ver o histórico completo de clientes não atendidos por ele nos últimos 24 meses. Se os mesmos clientes aparecem repetidamente, é um padrão — não um erro pontual.

---

#### ÁREA 2: Gráfico — Qtd. de Clientes Agendados e Não Atendidos por Vendedor no Mês

**O que mostra:** Gráfico de barras agrupadas mostrando, para cada vendedor, quantos clientes ficaram sem atendimento em cada mês do período selecionado.

**Legenda:** As barras são coloridas por mês (ex: "janeiro 2025", "fevereiro 2025") — isso permite comparar se o problema é recente ou crônico.

**Como analisar este gráfico:**

| Padrão visual | Diagnóstico | Ação |
|---------------|-------------|------|
| Um vendedor com barras consistentemente altas em todos os meses | Problema crônico — carteira sobrecarregada ou baixa produtividade | Redefinir carteira ou treinamento |
| Pico em um mês específico para um vendedor | Evento pontual — afastamento, emergência | Verificar histórico do vendedor naquele mês |
| Todos os vendedores com aumento no mesmo mês | Problema sistêmico — talvez a carteira geral foi aumentada sem capacidade | Revisar planejamento daquele ciclo |
| Um vendedor com zero barras | Execução perfeita — bom exemplo | Replicar suas práticas |

---

#### ÁREA 3: Tabela — Lista Detalhada de Clientes Agendados e Não Atendidos no Mês

Esta é a tabela mais **operacional e acionável** de todo o sistema GoVendas. É aqui que você encontra os nomes específicos dos clientes negligenciados.

Com os dados reais: **102 registros** encontrados no período.

| Coluna | Conteúdo | Como usar |
|--------|----------|-----------|
| **Data de Referência** | Mês/ano em que o cliente deveria ter sido atendido | Verificar se o problema é do mês atual ou passado |
| **Cód. Vendedor** | Código do vendedor responsável | Filtrar e agrupar por vendedor para ver concentração |
| **Nome do Vendedor** | Nome do vendedor responsável | Identificar rapidamente o responsável |
| **Cód. Cliente** | Código do cliente no ERP | Cruzar com sistema de pedidos para ver histórico |
| **Razão Social do Cliente** | Nome da empresa cliente | Identificar quais clientes estão sendo negligenciados — priorizar os de maior ticket |

##### Paginação:
- **102 registros** foram encontrados no período analisado
- A lista exibe 7 por vez — usar paginação para ver todos
- **Recomendação:** Exportar esta lista e ordenar por Razão Social + Vendedor para identificar padrões

---

### 🎯 Protocolo de Ação Gerencial

Quando o gestor abre este relatório, o protocolo recomendado é:

```
PROTOCOLO SEMANAL DE REVISÃO:

Segunda-feira:
→ Abrir relatório com filtro do mês atual
→ Ver quantos clientes estão na lista
→ Se mais de 10% da carteira planificada estiver sem atendimento → ALERTA

Durante a semana:
→ Reunião individual com vendedores que têm mais de 5 clientes não atendidos
→ Perguntas-chave:
   "O cliente estava disponível?"
   "Você tentou ligar mais de uma vez?"
   "Há algum problema com este cliente especificamente?"

Fim do mês:
→ Extrair a lista completa
→ Verificar clientes VIP (maior ticket) que ficaram sem atendimento
→ Ligar pessoalmente ou encaminhar para supervisão de atendimento
```

---

### ⚠️ Erros Comuns de Interpretação

1. **Usar este relatório de forma punitiva sem investigar:** Ver o nome de um vendedor na lista não significa automaticamente que ele foi negligente. Pode ser que o cliente ficou inacessível, ou que a carteira estava sobrecarregada.

2. **Não diferenciar clientes por importância:** Um cliente com ticket de R$500/mês que ficou sem atendimento é muito diferente de um cliente com ticket de R$50.000/mês. Sempre priorize pelo valor do cliente.

3. **Analisar só o mês atual:** O histórico de 24 meses é fundamental para identificar se é um cliente que **nunca** é atendido — o que indica um problema estrutural.

---

## MÓDULO 5 – Resultados de Positivação

### 📍 Localização no sistema
> **Relatórios → Resultados de Positivação**
> URL: `/reports/sale_results`

---

### 🎯 Visão Geral

#### Método Feynman
> Um médico que faz 100 consultas por mês e resolve os problemas de 70 pacientes tem uma "taxa de sucesso" de 70%. Um médico que faz 50 consultas e resolve 45 tem 90% de sucesso. Quem é melhor? Depende de quanto tempo cada caso exige. Na televendas, a positivação mede: dos clientes que o vendedor conseguiu contatar, quantos realmente compraram? Não é quantidade de ligações — é qualidade de conversão.

---

### 🖥️ Análise Completa da Tela

#### ÁREA 1: Filtros

| Filtro | Padrão | Configuração recomendada |
|--------|--------|------------------------|
| **Filtro de Data** | Último ano | **24 meses** — essencial para ver ciclos sazonais |
| **Supervisores** | Todos | Começar com todos; afunilar se necessário |
| **Vendedores** | Todos | Idem |

> [!NOTE]
> **Observação importante:** Durante a análise deste relatório com a conta utilizada, o sistema retornou "Nenhum resultado!" para os filtros aplicados. Isso indica que, para este cliente (Higicop), o módulo de Positivação pode ter uma configuração de dados específica ou período diferente. Em outras contas do GoVendas com dados completos, este relatório exibe os seguintes elementos abaixo.

---

#### ÁREA 2: KPIs de Positivação

Em contas com dados completos, este relatório exibe:

| KPI | O que representa | Referência |
|-----|-----------------|-----------|
| **Total de Atendimentos** | Volume total de contatos realizados | Base de cálculo |
| **Total de Positivações** | Atendimentos que geraram venda | — |
| **Taxa de Positivação (%)** | Positivações ÷ Atendimentos × 100 | Meta sugerida: > 60% |

---

#### ÁREA 3: Gráfico — Resultados da Positivação

**O que mostra:** Evolução mês a mês da taxa de positivação, com linha por vendedor ou equipe.

**Os três padrões mais importantes a identificar:**

```
PADRÃO 1 - Queda Brusca (de um mês para outro)
Causa provável: Mudança externa — problema com produto, preço, concorrência
Ação: Investigar o que mudou naquele mês especificamente

PADRÃO 2 - Queda Gradual (ao longo de meses)
Causa provável: Desmotivação, técnica desatualizada, produto perdendo espaço
Ação: Treinamento, revisão de mix, acompanhamento individual

PADRÃO 3 - Queda Sazonal (mesmo mês todo ano)
Causa provável: Sazonalidade do mercado
Ação: Ajustar metas para considerar a sazonalidade, não punir equipe
```

---

#### Como calcular e interpretar a taxa de positivação por vendedor:

```
Exemplo prático:

Vendedor A: 80 atendimentos → 60 positivações → 75% de positivação
Vendedor B: 80 atendimentos → 35 positivações → 43,75% de positivação

Análise:
- Vendedor A tem excelente taxa. Bom modelo para os outros.
- Vendedor B liga tanto quanto A, mas converte muito menos.
  Isso não é problema de esforço — é problema de abordagem ou oferta.
  Solução: Acompanhar chamadas do Vendedor B e comparar
             com as do Vendedor A para identificar o gap.
```

---

### 📊 Tabela de Referência — O que fazer em cada faixa de positivação:

| Taxa de Positivação | Diagnóstico | Ações recomendadas |
|--------------------|-------------|-------------------|
| **> 80%** | Excelência comercial | Documentar as práticas; use como referência para a equipe |
| **65–80%** | Bom desempenho | Manter; buscar escalar para >80% |
| **50–65%** | Desempenho aceitável | Coaching individual; análise das justificativas de não venda |
| **35–50%** | Alerta | Treinamento de técnicas de venda; revisão de produto/mix |
| **< 35%** | Crítico | Acompanhamento diário; possível revisão de carteira ou perfil |

---

### ⚠️ Erros Comuns de Interpretação

1. **Comparar positivação sem normalizar o volume:** Um vendedor com 10 atendimentos e 8 positivações (80%) pode parecer melhor que um com 100 atendimentos e 60 positivações (60%). Mas o segundo gerou 7,5x mais vendas. Sempre considere volume e taxa juntos.

2. **Usar positivação como única métrica de performance:** Um vendedor com alta positivação pode estar "cerejando" — ligando só para os clientes mais fáceis e ignorando a carteira completa. Cruzar com o relatório de Cobertura é essencial.

3. **Ignorar a coluna de Justificativas:** Se disponível, sempre analise por que os não-positivados não compraram. É informação de ouro para ajustes de produto e abordagem.

---

## MÓDULO 6 – Cobertura de Atendimento Multicanal - Validação

### 📍 Localização no sistema
> **Relatórios → Cobertura de Atendimento Multicanal - Validação**
> URL: `/reports/atendimento_multicanal`

---

### 🎯 Visão Geral

#### Método Feynman
> Imagine que você gerencia um shopping com 5 lojas diferentes. Um cliente comprou na loja de sapatos, não na de roupas. O gerente de roupas diz: "esse cliente não veio aqui." Mas o cliente foi ao shopping — ele está ativo. A cobertura multicanal responde: dos nossos clientes, quantos tiveram contato com a empresa por **qualquer** canal (televendas, app, e-commerce, representante, loja física)?

---

### 🖥️ Análise Completa da Tela

#### ÁREA 1: Filtros

| Filtro | Configuração | Observação |
|--------|-------------|-----------|
| **Filtro de Data** | 24 meses | Padrão configurado |
| **Supervisores** | Todos | Visão completa |
| **Vendedores** | Todos | Visão completa |

---

#### ÁREA 2: Cards de KPI — Os 3 Indicadores Principais

Com os dados reais encontrados:

| Card | Valor Real | O que significa | Relação com outros relatórios |
|------|-----------|-----------------|-------------------------------|
| **Clientes na Carteira** | **5.084** | Total de clientes no sistema | = Total de Clientes do Desempenho Comercial |
| **Clientes Agendados** | **3.085** | Clientes que tiveram algum agendamento | Mais do que os agendados no televendas |
| **Clientes Atendidos** | **1.392** | Clientes contatados por qualquer canal | Comparar com os Atendidos do televendas |

##### Análise desses dados reais:

```
Cobertura Multicanal = Clientes Atendidos ÷ Clientes na Carteira
= 1.392 ÷ 5.084 = 27,4%

Comparação:
- Televendas: 1.365 atendidos
- Multicanal: 1.392 atendidos
  → Diferença: apenas 27 clientes adicionais atendidos por outros canais

Isso indica que para este cliente, o televendas é o canal DOMINANTE.
Outros canais contribuem marginalmente.
```

---

#### ÁREA 3: Gráfico — Fluxo de Funil

**O que mostra:** Funil de clientes em 3 etapas:

```
ELEGÍVEIS (total na carteira com potencial)
    ↓
AGENDADOS (foram planejados para atendimento)
    ↓
ATENDIDOS (receberam contato por qualquer canal)
```

**Como interpretar as perdas em cada etapa:**

```
Elegíveis → Agendados: perda aqui = clientes que deveriam estar no plano mas não foram incluídos
(Problema de: planejamento da carteira)

Agendados → Atendidos: perda aqui = clientes agendados que não foram contactados
(Problema de: execução do atendimento)
```

**Dado real:**
```
Elegíveis: ~5.084
Agendados: 3.085 (60,7% dos elegíveis foram agendados)
Atendidos: 1.392 (45,1% dos agendados foram atendidos)

Maior perda está na etapa Agendados → Atendidos
= Problema de EXECUÇÃO, não de planejamento
```

---

#### ÁREA 4: Gráfico — Clientes Atendidos por Período

**O que mostra:** Série histórica com 4 linhas:

| Linha | O que representa |
|-------|----------------|
| **Planejados** | Clientes que foram incluídos no plano de atendimento |
| **Atendidos Planejados** | Dos planejados, quantos foram efetivamente contatados |
| **Atendidos Avulsos** | Contatos realizados fora do planejamento |
| **Vendidos** | Dos atendidos, quantos geraram venda |

**Análise avançada deste gráfico:**

```
CENÁRIO SAUDÁVEL:
Planejados ≈ Atendidos Planejados (alta aderência ao plano)
Vendidos ≈ Atendidos (alta conversão)

CENÁRIO DE ALERTA 1:
Atendidos Avulsos >> Atendidos Planejados
→ Equipe ignorando o plano, ligando para quem quiser

CENÁRIO DE ALERTA 2:
Vendidos muito abaixo de Atendidos
→ Problema de conversão/abordagem (investigar com relatório de Positivação)

CENÁRIO DE ALERTA 3:
Planejados crescendo mas Atendidos estagnados
→ Plano aumentou mas execução não acompanhou (verificar Capacidade)
```

---

### 🔄 Como usar o Multicanal junto com os outros relatórios

| Situação | O que o Multicanal adiciona |
|----------|---------------------------|
| Cobertura Televendas baixa | Verificar se o cliente foi atendido por outro canal antes de cobrar o vendedor |
| Cliente marcado como "Não Atendido" | Confirmar se ele não comprou pelo e-commerce ou representante |
| Positivação baixa pelo televendas | Ver se o cliente está comprando por outro canal com melhor conversão |

---

### ⚠️ Erros Comuns de Interpretação

1. **Usar Cobertura Multicanal como desculpa para ignorar o televendas:** Se o cliente compra por outro canal, o televendas ainda tem papel de relacionamento, upsell e fidelização. Não atender multicanal não substitui atender por televendas.

2. **Não comparar os números com o relatório de Cobertura Televendas:** Os dois relatórios se complementam. Analisar isoladamente perde o contexto.

3. **Ignorar a evolução ao longo do tempo:** Uma queda nos Clientes Atendidos mês a mês no gráfico de período pode indicar migração de clientes para outros canais que não estão integrados ao GoVendas.

---

## 9. CENÁRIOS AVANÇADOS DE GESTÃO

### 🔴 Cenário 1: "Temos 5.084 clientes cadastrados mas só 703 estão ativos. Como crescer?"

**Diagnóstico usando os relatórios:**

```
PASSO 1 → Desempenho Comercial:
Confirmar os números: 4.096 Prospects + 285 Inativos = 4.381 clientes potenciais intocados.

PASSO 2 → Planejamento de Capacidade:
Com 26 vendedores e capacidade de 440 clientes/mês cada, 
a capacidade total mensal = 26 × 440 = 11.440 contatos/mês
Isso é suficiente para cobrir toda a carteira — o problema não é capacidade.

PASSO 3 → Cobertura Televendas:
Identificar que apenas 20,7% dos agendados são atendidos dentro do planejado.
812 atendimentos avulsos vs 553 dentro do plano INVERTE a lógica:
os vendedores ligam mais para clientes fora do plano.

PASSO 4 → Clientes Não Atendidos:
102 registros de clientes agendados e não atendidos.
Verificar se Prospects estão sendo incluídos nos agendamentos.

CONCLUSÃO:
O problema não é falta de clientes nem falta de vendedores.
É a falta de planejamento e execução da carteira de Prospects.
A empresa tem capacidade para crescer 5x em ativos — mas precisa
direcionar os vendedores para ligarem para os Prospects e Inativos de forma sistemática.
```

---

### 🔴 Cenário 2: "A cobertura de positivação é 99,71% mas a cobertura de atendimento é baixa. Por quê?"

```
ANÁLISE:
Positivação altíssima (99,71%) + Cobertura baixa (20,7%) = Paradoxo aparente

RESOLUÇÃO:
Os vendedores estão ligando para clientes "seguros" — aqueles que provavelmente vão comprar.
Estão evitando a carteira planejada (que inclui Prospects e clientes difíceis).
Resultado: quase tudo que ligam converte, mas ligam para poucos.

PROVA: 
812 atendimentos avulsos vs 553 planejados
→ 59,5% dos atendimentos são FORA do plano

AÇÃO DO GESTOR:
1. Reunião com a equipe: explicar que a carteira planejada deve ser a prioridade
2. Criar meta de cobertura mínima da carteira planejada (ex: >70%)
3. Monitorar semanalmente pelo relatório de Cobertura Televendas
4. Criar incentivo específico para ativação de Prospects e Inativos
```

---

### 🔴 Cenário 3: "Um vendedor específico aparece repetidamente na lista de clientes não atendidos"

```
INVESTIGAÇÃO ESTRUTURADA:

Semana 1:
→ Relatório de Planejamento de Capacidade (filtrar por este vendedor)
   Pergunta: A carteira dele está sobrecarregada?
   
→ Relatório de Clientes Não Atendidos (filtrar por este vendedor, 6 meses)
   Pergunta: Os mesmos clientes aparecem repetidamente?

Semana 2 (após coletar dados):
→ Se carteira sobrecarregada: redistribuir 20-30% dos clientes
→ Se carteira OK mas não atendimento: reunião individual
   "Vi que X clientes específicos nunca foram atendidos por você.
    O que está acontecendo com esses clientes?"

Semana 3-4:
→ Monitorar se o número de não atendidos diminuiu
→ Verificar na Cobertura Televendas a melhora individual
```

---

## 10. GUIA DE DIAGNÓSTICO RÁPIDO

### 🚦 Semáforo de Saúde da Operação

Use esta tabela para fazer um diagnóstico rápido em 5 minutos quando abrir o sistema:

| Relatório | Métrica | 🟢 Saudável | 🟡 Atenção | 🔴 Crítico |
|-----------|---------|-----------|-----------|-----------|
| **Desempenho Comercial** | Clientes Ativos | Crescimento mês a mês | Estável | Queda por 2+ meses |
| **Capacidade** | Status dos vendedores | Todos equilibrados | 1-3 sobrecarregados | >30% sobrecarregados |
| **Cobertura Televendas** | % Agendados atendidos | > 80% | 60-80% | < 60% |
| **Não Atendidos** | Qtd. de registros | Próximo de zero | Até 5% da carteira | > 10% da carteira |
| **Positivação** | Taxa % | > 70% | 50-70% | < 50% |
| **Multicanal** | Funil Agendados→Atendidos | > 80% | 60-80% | < 60% |

---

### 📅 Rotina Recomendada do Gestor

| Frequência | Relatório | O que fazer | Tempo |
|------------|-----------|-------------|-------|
| **Diário** | Clientes Não Atendidos | Verificar se há novos registros no dia | 3 min |
| **Semanal** | Cobertura Televendas | Verificar % de cobertura da semana; alertar quem está abaixo de 60% | 10 min |
| **Quinzenal** | Capacidade + Não Atendidos | Verificar desequilíbrios de carteira; redistribuir se necessário | 15 min |
| **Mensal** | Todos os 6 relatórios | Análise completa; reunião de feedback com a equipe | 60 min |
| **Trimestral** | Desempenho Comercial | Análise estratégica de evolução da carteira; planejamento de ativação | 30 min |

---

### 💬 As 6 Perguntas que um Gestor Experiente Sempre Faz

```
1. "Quantos clientes agendados NÃO foram atendidos esta semana?"
   → Relatório: Clientes Não Atendidos

2. "A cobertura desta semana está dentro da meta?"
   → Relatório: Cobertura de Atendimento Televendas

3. "Tem vendedor sobrecarregado que não consegue atender tudo?"
   → Relatório: Planejamento de Capacidade

4. "A taxa de positivação está se mantendo ou caindo?"
   → Relatório: Resultados de Positivação

5. "Nossa carteira ativa está crescendo, estável ou encolhendo?"
   → Relatório: Desempenho Comercial - Validação

6. "Os clientes que o televendas não atendeu foram cobertos por outro canal?"
   → Relatório: Cobertura de Atendimento Multicanal
```

---

> [!NOTE]
> **Registro de análise:** Este documento foi produzido com base em análise direta do sistema GoVendas, utilizando filtro de 24 meses. Os dados reais encontrados (2.675 agendados, 5.084 clientes, 99,71% de positivação, etc.) são da conta analisada e servem como referência de interpretação. Cada empresa terá seus próprios números, mas a lógica de análise permanece a mesma.

---

*Roteiro Avançado desenvolvido em Março/2026 — GoVendas*
