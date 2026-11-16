# Análise Econômica e Machine Learning

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24286946.svg)](https://doi.org/10.5281/zenodo.24286946)

Material didático das aulas práticas da disciplina Análise Econômica e Machine Learning, da Universidade Católica de Pernambuco - Unicap: dez laboratórios em Python, cada um com um notebook de exercícios e os slides da aula. Os exemplos usam dados econômicos reais, em boa parte brasileiros e pernambucanos.

Autor: Prof. Flavius Sodré.

## Aulas

| Aula | Tema | Notebook | Slides |
| --- | --- | --- | --- |
| 01 | Laboratório: a primeira coleta de dados econômicos | [Aula01_Aluno.ipynb](Notebooks/Aula01_Aluno.ipynb) | [Aula01.pdf](Slides/Aula01.pdf) |
| 02 | Laboratório: o que o dado mostra antes do modelo | [Aula02_Aluno.ipynb](Notebooks/Aula02_Aluno.ipynb) | [Aula02.pdf](Slides/Aula02.pdf) |
| 03 | Previsão e causalidade: prever e explicar não são a mesma conta | [Aula03_Aluno.ipynb](Notebooks/Aula03_Aluno.ipynb) | [Aula03.pdf](Slides/Aula03.pdf) |
| 04 | Regularização e seleção de variáveis: muitas variáveis, poucas que importam | [Aula04_Aluno.ipynb](Notebooks/Aula04_Aluno.ipynb) | [Aula04.pdf](Slides/Aula04.pdf) |
| 05 | Árvores, florestas e boosting: quem paga e quem não paga | [Aula05_Aluno.ipynb](Notebooks/Aula05_Aluno.ipynb) | [Aula05.pdf](Slides/Aula05.pdf) |
| 06 | Nowcasting e previsão macroeconômica: o PIB de hoje, antes do IBGE | [Aula06_Aluno.ipynb](Notebooks/Aula06_Aluno.ipynb) | [Aula06.pdf](Slides/Aula06.pdf) |
| 07 | Aprendizagem não supervisionada: quem se parece com quem | [Aula07_Aluno.ipynb](Notebooks/Aula07_Aluno.ipynb) | [Aula07.pdf](Slides/Aula07.pdf) |
| 08 | Validação de modelos preditivos: quanto o modelo erra de verdade | [Aula08_Aluno.ipynb](Notebooks/Aula08_Aluno.ipynb) | [Aula08.pdf](Slides/Aula08.pdf) |
| 09 | Introdução ao machine learning causal: prever não é responder "e se?" | [Aula09_Aluno.ipynb](Notebooks/Aula09_Aluno.ipynb) | [Aula09.pdf](Slides/Aula09.pdf) |
| 10 | Machine learning causal e políticas públicas: para quem a política funciona | [Aula10_Aluno.ipynb](Notebooks/Aula10_Aluno.ipynb) | [Aula10.pdf](Slides/Aula10.pdf) |

Cada notebook traz explicações, código pronto e exercícios para completar.

## Como usar

1. Instale o Python 3.12 ou mais recente e o VS Code, com as extensões Python e Jupyter.
2. Baixe o repositório (botão Code › Download ZIP, ou `git clone`) e abra a pasta no VS Code.
3. No terminal do VS Code, crie o ambiente e instale os pacotes:

```bash
python3 -m venv .venv
source .venv/bin/activate        # no Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

4. Abra um notebook da pasta `Notebooks`, escolha o ambiente `.venv` como kernel e rode as células em ordem.

As Aulas 01 e 02 consultam APIs públicas (Banco Central, IBGE e Banco Mundial). As demais usam primeiro os arquivos da pasta `Dados`. Sem internet e sem arquivo, cada notebook segue com um plano B, com dados simulados e aviso na tela.

## Dados

| Arquivo | Conteúdo | Fonte | Aulas |
| --- | --- | --- | --- |
| `ames_housing.csv` | Vendas de imóveis em Ames, Iowa (De Cock, 2011) | Rdatasets (pacote modeldata) | 04 |
| `credito_taiwan.csv` | 30 mil clientes de cartão de crédito em Taiwan (Yeh e Lien, 2009) | UCI Machine Learning Repository | 05 e 08 |
| `indicadores_mensais.csv` | Indicadores mensais de atividade e preços do Brasil | Banco Central (SGS) e IBGE (SIDRA) | 06 |
| `pib_trimestral.csv` | PIB trimestral do Brasil | IBGE (SIDRA) | 06 |
| `municipios_pe.csv` | Indicadores dos 185 municípios de Pernambuco | IBGE (Censo 2022, PIB dos Municípios, Cadastro Central de Empresas) | 07 |
| `mapa_municipios_pe.json` | Contornos dos municípios de Pernambuco | Malha do IBGE, na versão GeoJSON do projeto geodata-br | 07 |
| `401k.csv` | 9.915 famílias americanas, SIPP de 1991 | Repositório de replicação do DML (Chernozhukov e outros, 2018) | 09 e 10 |

Os direitos sobre os dados são das fontes originais; cite-as ao reutilizá-los.

## Gabaritos

As soluções dos exercícios não ficam neste repositório, para que os estudantes façam os exercícios por conta própria. Professores que quiserem usar o material podem pedir os gabaritos ao autor.

## Como citar

Use o botão "Cite this repository", na coluna da direita do GitHub, ou:

> SODRÉ, Flavius Raymundo Arruda. **Análise Econômica e Machine Learning: notebooks e slides das aulas práticas**. Versão 1.0. Recife: Universidade Católica de Pernambuco, 2026. Material didático. Disponível em: https://doi.org/10.5281/zenodo.24286946.

## Licença

Copyright (c) 2026 Flavius Raymundo Arruda Sodré.

Este material está sob a licença Creative Commons Atribuição-NãoComercial-CompartilhaIgual 4.0 Internacional (CC BY-NC-SA 4.0), cujo texto completo está no arquivo `LICENSE` e cujo resumo em português está em https://creativecommons.org/licenses/by-nc-sa/4.0/deed.pt-br. Você pode copiar, adaptar e usar o material em aula, desde que cite o autor, não o use para fins comerciais e distribua as adaptações sob a mesma licença.

A marca e o logotipo da Universidade Católica de Pernambuco que aparecem nos slides não estão cobertos por esta licença.