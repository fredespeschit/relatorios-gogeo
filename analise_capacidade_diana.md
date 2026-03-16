# 📄 Estudo de Caso: Planejamento de Capacidade (Diana de Souza Rosalino)
## Tutorial Didático com Análise de Dados Reais

Este documento apresenta uma análise técnica e pedagógica do relatório de **Planejamento de Capacidade**, utilizando como exemplo prático os dados reais da vendedora **Diana de Souza Rosalino**.

---

### 1. Seção: Filtros de Seleção
**O que esta seção representa:**
É a área de controle do relatório. Aqui o gestor define o escopo da análise (quem será analisado) e a margem de erro aceitável (**Tolerância**).

**Análise usando os dados da Diana:**
*   **Vendedor selecionado:** Diana de Souza Rosalino.
*   **Tolerância:** 0.10 (10%).
*   **Interpretação:** A tolerância de 10% significa que o sistema só marcará Diana como "Acima da Capacidade" se a demanda de clientes exceder em mais de 10% a capacidade diária dela. É uma gordura de segurança para variações naturais do dia a dia.

---

### 2. Seção: KPI Cards (Resumo da Equipe)
**O que esta seção representa:**
Fornece uma visão macro da saúde do planejamento de toda a equipe sob a responsabilidade dos supervisores selecionados.

**Análise usando os dados da Diana:**
*   **Vend. Cadastrados:** 28
*   **Vend. sem agendamento:** 19
*   **Vend. com agendamento:** 9
*   **Interpretação:** Embora estejamos focados na Diana, este bloco revela que apenas 9 vendedores (incluindo a Diana) possuem uma agenda ativa. Isso indica que a Diana faz parte do grupo minoritário da empresa que está efetivamente com o motor de vendas ligado no sistema.

---

### 3. Seção: Tabela Principal (Todos os Vendedores)
**O que esta seção representa:**
É o coração do relatório. Cruza os dados da carteira (demanda) com a força de trabalho (capacidade).

**Análise usando os dados da Diana:**
*   **Status do Planejamento:** 🔴 **CLIENTES ACIMA DA CAPACIDADE**
*   **Total de Clientes na Carteira:** 80
*   **Capacidade de Atendimento Diário:** 0
*   **Demanda de Atendimento Diário:** 37
*   **Disponibilidade Diária:** -37
*   **Interpretação:** Aqui encontramos o problema crítico. Diana tem uma carteira de 80 clientes, dos quais **37 precisam de atendimento hoje**. No entanto, a **Capacidade Diária dela está configurada como 0**. Isso gera uma disponibilidade negativa de -37. Na prática, a Diana está "proibida" pelo sistema de atender, mas tem uma fila de 37 pessoas esperando.

---

### 4. Seção: Clientes por Tipo de Classificação
**O que esta seção representa:**
Explica a origem da "Demanda". Mostra como os clientes da carteira estão divididos pela frequência de contato programada (Frequência Diária, Quinzenal, Mensal, etc.).

**Análise usando os dados da Diana:**
*   **F. Diária:** 37 clientes
*   **F. Quinzenal:** 43 clientes
*   **Total:** 80 clientes
*   **Interpretação:** Os 37 clientes de "Frequência Diária" são exatamente os que geram a demanda de 37 atendimentos por dia vista na seção anterior. Os outros 43 são quinzenais, ou seja, aparecem na agenda apenas em dias específicos.

---

### 5. Seção: Situação do Vendedor (Gráfico de Termômetro)
**O que esta seção representa:**
Uma representação visual rápida para o gestor identificar o nível de urgência da correção.

**Análise usando os dados da Diana:**
*   **Status:** CLIENTES ACIMA DA CAPACIDADE.
*   **Potencial de Aumento:** 0.00%.
*   **Interpretação:** O potencial de aumento em 0% indica que Diana não pode receber nem mais um único cliente. Ela já ultrapassou o limite máximo de segurança definido pela tolerância.

---

### 6. Seção: Possibilidades de Ajuste (Sugestão do Sistema)
**O que esta seção representa:**
O GoVendas atua como um consultor, sugerindo as ações imediatas que o gestor deve tomar para resolver o desequilíbrio.

**Análise usando os dados da Diana:**
O sistema sugere duas ações para o caso dela:
1.  **Aumentar a capacidade diária:** Atualmente está em 0. O gestor precisa configurar quantos contatos Diana realmente consegue fazer (ex: 20 ou 30 por dia).
2.  **Reduzir a Carteira:** Se mesmo aumentando a capacidade para um nível humano (ex: 25) a demanda continuar alta, alguns dos 80 clientes devem ser passados para outro vendedor.

---

### 7. Conclusão da Análise — Caso Diana
A situação da vendedora Diana de Souza Rosalino é um exemplo clássico de **erro de configuração de sistema que gera falso alerta de sobrecarga**.

*   **Diagnóstico:** Diana tem clientes (80) e tem trabalho diário (37), mas o sistema entende que ela tem "zero" braços para trabalhar (**Capacidade 0**).
*   **Risco Gerencial:** O gestor pode achar que ela está sendo ineficiente, quando na verdade o sistema não está permitindo que o planejamento dela seja medido corretamente.
*   **Ação Recomendada:** Entrar no cadastro da vendedora Diana e definir uma **Capacidade de Atendimento Diário** realista (ex: 40 contatos/dia). Assim que isso for feito, o status dela passará de Vermelho (Acima da Capacidade) para Verde (Dentro da Capacidade), pois 37 está abaixo de 40.
