# Análise da Meta do Valorant - Estudo de Efetividade dos Agentes

> Projeto de Data Science analisando a efetividade dos agentes no Valorant competitivo usando dados reais do VLR.gg

![Valorant](https://img.shields.io/badge/Game-Valorant-FF4655?style=for-the-badge&logo=riot-games)
![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python)
![Data Science](https://img.shields.io/badge/Data-Science-FF6B6B?style=for-the-badge)

## 🎮 Visão Geral do Projeto

Este projeto analisa a efetividade dos agentes do Valorant no cenário competitivo usando dados reais coletados do VLR.gg. O objetivo é identificar:

- **Agentes meta-dominantes** (alto pick rate + alto win rate)
- **Joias escondidas** (baixo pick rate + alta performance) 
- **Agentes superestimados** (alto pick rate + baixa performance)
- **Equilíbrio entre funções** no jogo

## 🔍 Principais Descobertas

### 🏆 Agentes Mais Eficientes por Função:
- **Duelista**: Yoru (Eficiência: 9.808)
- **Controlador**: Clove (Eficiência: 12.708) 
- **Iniciador**: Gekko (Eficiência: 5.36)
- **Sentinela**: Vyse (Eficiência: 16.154)

### 💎 Joias Escondidas Descobertas:
- **Vyse**: 16.154 de eficiência com apenas 2.9% de pick rate
- **Clove**: 12.708 de eficiência com apenas 3.8% de pick rate
- **Yoru**: Maior eficiência entre duelistas apesar do baixo uso

### 📊 Insights Principais:
1. **Agentes novos tendem a ser subvalorizados** pelo cenário competitivo
2. **Alta eficiência nem sempre se correlaciona com alto pick rate**
3. **Função Sentinela tem o maior potencial inexplorado** (Vyse)
4. **Agentes meta tradicionais** (Jett, Omen) dominam pick rates mas nem sempre são os mais eficientes

## 📈 Visualizações

### Efetividade dos Agentes
![Efetividade dos agentes por role](imagem/efetividades-agentes.png)

### Pick rate medio por role
![Pick rate medio por role](pickrate-role.png)

## 🛠️ Stack Tecnológico

- **Python 3.8+**
- **Pandas** - Manipulação de dados
- **BeautifulSoup** - Web scraping do VLR.gg
- **Plotly** - Visualizações interativas
- **Requests** - Requisições HTTP para coleta de dados

## 📊 Metodologia

1. **Coleta de Dados**: Web scraping de partidas competitivas do VLR.gg
2. **Processamento**: Cálculo de pick rates, win rates e métricas de eficiência
3. **Análise**: Identificação de padrões e classificação de agentes por tiers
4. **Visualização**: Criação de gráficos interativos para insights
5. **Insights**: Geração de recomendações acionáveis para coaches

## 🎯 Valor para E-Sports

Esta análise fornece:
- **Vantagens estratégicas** identificando agentes subvalorizados
- **Decisões de draft baseadas em dados** ao invés de seguir a meta cegamente  
- **Inteligência competitiva** sobre tendências emergentes
- **Otimização de performance** para equipes profissionais

## 📁 Estrutura do Projeto

```
valorant-meta-analysis/
├── README.md                    # Documentação do projeto
├── valorant_analysis.py         # Código principal da análise
├── requirements.txt             # Dependências Python
├── images/                      # Visualizações geradas
└── data/                        # Dados coletados
```

## 🚀 Como Executar

1. Clone o repositório:
```bash
git clone https://github.com/Gaab-elle/valorant-meta-analysis.git
cd valorant-meta-analysis
```

2. Instale as dependências:
```bash
pip install -r requirements.txt
```

3. Execute a análise:
```bash
python valorant_e_analise_de_dados.py
```

## 🔮 Melhorias Futuras

- [ ] **Análise específica por mapa** (efetividade de agentes por mapa)
- [ ] **Análise temporal** (evolução da meta ao longo do tempo)
- [ ] **Comparação regional** (diferenças de meta entre NA vs EU vs APAC)
- [ ] **Dashboard interativo** com Streamlit
- [ ] **Modelagem preditiva** para resultados de partidas

## 💡 Principais Recomendações para Coaches

### 🔍 Agentes para Testar:
- **Vyse** em composições defensivas (16.154 efficiency, apenas 2.9% pick rate)
- **Clove** como controlador alternativo (12.708 efficiency, 3.8% pick rate)
- **Yoru** para estratégias específicas (maior efficiency entre duelistas)

### ⚠️ Insights Estratégicos:
- Não seguir apenas a meta mainstream pode gerar vantagens competitivas
- Agentes novos frequentemente têm potencial inexplorado
- Eficiência é mais importante que popularidade para performance

## 📊 Definições de Métricas

- **Pick Rate**: Porcentagem de partidas onde o agente foi escolhido
- **Win Rate**: Porcentagem de vitórias quando o agente foi usado
- **Efficiency Score**: Relação Win Rate / Pick Rate (indica se é sub/supervalorizado)
- **Hidden Gem**: Alto win rate + baixo pick rate (oportunidade!)
- **Meta Dominante**: Alto pick rate + alto win rate (confiável)

## 📧 Contato

Sinta-se à vontade para entrar em contato para colaborações ou dúvidas sobre analytics em e-sports!

**Gabrielle Ribeiro** - Cientista de Dados especializado em E-Sports Analytics
- LinkedIn: www.linkedin.com/in/gabz-ribeiro
- Email: contato.gabriellerib@gmail.com

---

## 🎮 Sobre o Valorant

O Valorant é um FPS tático da Riot Games com 4 funções principais:
- **🔥 Duelista**: Entrada e frags (Jett, Raze, Phoenix, etc.)
- **💨 Controlador**: Controle de mapa com smokes (Omen, Astra, Brimstone, etc.)
- **🔍 Iniciador**: Reconhecimento e suporte (Sova, Fade, Skye, etc.)
- **🛡️ Sentinela**: Defesa e controle de área (Sage, Cypher, Killjoy, etc.)

---
