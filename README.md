# 📊 Análise de Feminicídios no RJ

Este notebook analisa dados de feminicídio e tentativa de feminicídio registrados no estado do Rio de Janeiro entre 2016 e 2025, com base em dados públicos do [ISP-RJ](https://www.ispdados.rj.gov.br/).

---

## 🎯 Objetivos

* Analisar evolução mensal e anual dos casos
* Observar a proporção entre feminicídios e tentativas
* Identificar padrões sazonais
* Mapear a distribuição por município

---

## 📁 Fonte dos Dados

* CSV: [BaseFeminicidioEvolucaoMensalCisp.csv](https://raw.githubusercontent.com/nanquinote/mvp-analise-feminicidios/main/BaseFeminicidioEvolucaoMensalCisp.csv)
* GeoJSON: `municipios_rj.json`

---

## 🛠️ Tecnologias

* Python 3
* Pandas, Matplotlib, Plotly

---

## 📌 Dicionário de Dados

| Variável                   | Descrição                                                              |
| -------------------------- | ---------------------------------------------------------------------- |
| `cisp`                     | Código da circunscrição da delegacia                                   |
| `Ano`                      | Ano da ocorrência                                                      |
| `Mês`                      | Mês da ocorrência                                                      |
| `Feminicídio`              | Casos consumados de feminicídio                                        |
| `Tentativa de feminicídio` | Tentativas registradas de feminicídio                                  |
| `Município`                | Município da ocorrência (adicionado posteriormente por enriquecimento) |
| `Data`                     | Data fictícia criada com dia 1 do mês da ocorrência                    |
| `Ocorrências`              | Soma de feminicídios e tentativas                                      |
| `Estacao`                  | Estação do ano correspondente ao mês (`Verão`, `Outono`, etc.)         |

---

## 🔍 Etapas

1. Coleta dos dados
2. Análise exploratória e estatística descritiva
3. Limpeza e enriquecimento
4. Criação de variáveis auxiliares
5. Visualizações:

---

## 🧭 Resultados

* Tentativas são mais frequentes que casos consumados
* Picos irregulares sugerem sazonalidade ou eventos externos
* Verão concentra mais ocorrências
* Municípios com maior população lideram em número de casos

---

## ⚠️ Limitações

* Dados restritos ao RJ
* Registros sujeitos a subnotificação
* Análise puramente descritiva
