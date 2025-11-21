# 🚨 Detecção de Anomalias em Vendas (Séries Temporais)

## 💡 Visão Geral do Projeto

Este projeto implementa uma solução de Machine Learning **Não Supervisionado** para monitorar a série temporal de vendas e identificar desvios anormais (anomalias). O objetivo é sinalizar eventos críticos como **fraudes**, **erros de sistema** ou **mudanças abruptas** no padrão de consumo antes que causem prejuízos significativos.

A solução garante a estabilidade financeira e a integridade dos dados operacionais da empresa.

---

## ⚙️ Metodologia e Arquitetura

| Componente | Técnica | Vantagem para o Projeto |
| :--- | :--- | :--- |
| **Algoritmo** | **Isolation Forest** | Modelo robusto e eficiente para isolar *outliers* em dados multidimensionais (Vendas + Tráfego), aprendendo o "padrão normal" sem a necessidade de rótulos. |
| **Dados de Entrada** | Vendas (R$) e Tráfego do Site | Permite detecção de anomalias que ocorrem na **relação** entre as variáveis, não apenas nas vendas isoladas. |
| **Output** | **Score de Anomalia** | Entrega um ranking de risco (quanto mais negativo, mais anômalo), permitindo priorizar a investigação. |



---

## ✅ Resultados e Ação Preventiva (Aplicações de Negócio)

O modelo identificou dois eventos de alto risco que exigiram ação imediata:

| Data | Tipo de Anomalia | Ação Preventiva / Mitigação | Foco Estratégico |
| :--- | :--- | :--- | :--- |
| **2024-10-10** | **Pico Inesperado de Vendas (R$ 1.200)** | **Investigação de Fraude/Bug Fiscal.** Verificar *logs* de transações e regras de precificação para evitar perdas ou auditorias fiscais. | **Segurança e Conformidade** |
| **2024-10-25** | **Queda Drástica de Vendas (R$ 50,00)** | **Verificação de Sistemas Críticos.** Alerta a TI e Estoque para corrigir falhas no *checkout* ou falta de produtos. | **Minimização da Perda de Receita** |

A solução de **Isolation Forest** demonstrou ser uma ferramenta poderosa para a **supervisão proativa** da saúde das vendas, transformando o Machine Learning em uma camada de proteção financeira.

---
