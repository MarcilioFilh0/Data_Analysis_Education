# Data_Analysis_Education

## 1. Ideia do Projeto

Este projeto foi desenvolvido como parte da avaliação A3 da unidade curricular de **Análise de Dados e Big Data** da Universidade Salvador (UNIFACS). O objetivo central é investigar o fenômeno da evasão escolar no Brasil, mapeando como a infraestrutura básica e digital, a disparidade entre as redes pública e privada, e os fatores de gestão interna influenciam tanto a permanência do estudante quanto o seu desempenho acadêmico final no ENEM.

A partir do cruzamento de microdados públicos do INEP de 2024 (Censo Escolar, Notas do ENEM e Taxas de Rendimento), a pesquisa busca quebrar mitos educacionais e fornecer insights preditivos e acionáveis para apoiar gestores públicos na tomada de decisões proativas.

---

## 2. Links Úteis

| Recurso | Descrição | Link |
| :--- | :--- | :--- |
| **Relatório** | Documentação completa do processo de gerenciamento de equipe, metodologia de ETL, análise exploratória (EDA) e conclusões teóricas. | [Acessar Documento](https://docs.google.com/document/d/1MQSFskGGij4UCF5LLO_ckwod_lkNSz8H6WlncSnyGV0/edit?usp=sharing) |
|  **Site** | Dashboard criado para a visualização interativa dos gráficos de dispersão, boxplots e cruzamentos de dados estruturados para o projeto. | [Visualizar Dashboard](https://86xr29yrk4puzyvpdzxnzg.streamlit.app/) |
|  **Google Colab** | Scripts automatizados em Python utilizados na extração, limpeza, tratamento de nulos e modelagem dos dados. | [Abrir Notebook](https://colab.research.google.com/drive/1HpX57meQgTR0CvXsif2MDJuEelHJtuXX?usp=sharing) |

---

## 3. Integrantes do Projeto

*  **Marcilio Batista Filho**
*  **Maria Clara Daltro** 
*  **Rodson de Souza Junior**

---

## 4. Arquitetura do Projeto
```markdown
 Data_Analysis_Education
 ├── 📂 data
 │    ├──📂 01_cleaned
 │	  │	  ├── 📊 Tabela_censo_Escolar_2024.csv
 │	  │   ├── 📊 Tabela_ENEM_2024.csv
 │	  │   └── 📊 Tabela_Evasao_2024.csv
 │    └──📂 02_filtered
 │	  	  ├── 📊 Maiores_Taxas_Evasao_e_Reprovacao_2024.csv
 │	  	  ├── 📊 Menores_Taxas_Evasao_e_Reprovacao_2024.csv
 │	  	  ├── 📊 Tabela_Censo_Escolar_Maior_Evasao_2024.csv
 │	      └── 📊 Tabela_Censo_Escolar_Menor_Evasao_2024.csv
 ├── 📂 notebooks
 │    ├──📂 01_data_cleaning
 │	  │	  ├── 📄 Codigo_Censo_INEP_Escolar_2024.ipynb
 │	  │	  ├── 📄 Codigo_INEP_ENEM_2024.ipynb
 │	  │   └── 📄 Codigo_Taxa_Evasao_2024.ipynb
 │    ├──📂 02_data_filtering
 │	  │	  ├── 📄 Código_Maiores_Taxas_Evasao_e_Reprovacao_2024.ipynb
 │	  │	  ├── 📄 Código_Menores_Taxas_Evasao_e_Reprovacao_2024.ipynb
 │	  │	  ├── 📄 Código_Tabela_Censo_Escolar_Maior_Evasao.ipynb
 │	  │	  └── 📄 Código_Tabela_Censo_Escolar_Menor_Evasao.ipynb
 │    ├──📂 03_stats_analysis
 │	  │	  ├── 📄 01_analise_evasao_enem.ipynb
 │	  │	  ├── 📄 02_analise_permanencia_enem.ipynb
 │	  │	  ├── 📄 03_analise_boxplot_evasao.ipynb
 │	  │	  ├── 📄 04_analise_efeito_u_reprovacao.ipynb
 │	  │	  └── 📄 05_analise_infraestrutura_extremos.ipynb
 │    └──📂 04_graphs_and_relations
 │	  	  ├── 📄 Analise_Comparativa_De_Quartis.ipynb
 │	  	  ├── 📄 Analise_Entre_Infraesturura_Evasao.ipynb
 │	  	  ├── 📄 Analise_Maiores_Evasao.ipynb
 │	  	  ├── 📄 Analise_Maiores_Taxas_Com_Moda.ipynb
 │	  	  ├── 📄 Analise_Menores_Evasao.ipynb
 │	  	  ├── 📄 Analise_Menores_Taxas_Com_Moda.ipynb
 │	  	  ├── 📄 Analise_Padrao.ipynb
 │	  	  ├── 📄 Analise_Taxa_Permanencia_Com_Media.ipynb
 │	  	  └── 📄 Analise_Todas_Escolas.ipynb
 └──📑 README.md
