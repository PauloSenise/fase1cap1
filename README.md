# Faculdade de Informática e Administração Paulista

<p align="center">
  <img src="https://github.com/Luiz-FIAP/Fase_06_Cap_1_Despertar_da_Rede_Neural/blob/main/Ir_alem2/docs/examples/logo-fiap.png?raw=true" width="45%">
</p>

<h1 align="center">A Busca de Dados: Preparando o Terreno para a Inteligência Cardiológica</h1>

<p align="center">
  <strong>FIAP • Tecnólogo em Inteligência Artificial • Fase 1 • Capítulo 1 • 1º Semestre 2026</strong>
</p>

---

## Equipe

### Grupo 3 – Capítulo 1 - Fase 1

| Integrante | GitHub |
|---|---|
| Felipe Sabino da Silva | [@FelipeSabinoTMRS](https://github.com/FelipeSabinoTMRS) |
| Juan Felipe Voltolini | [@juanvoltolini-rm562890](https://github.com/juanvoltolini-rm562890) |
| Luiz Henrique Ribeiro de Oliveira | [@Luiz-FIAP](https://github.com/Luiz-FIAP) |
| Marco Aurélio Eberhardt Assimpção | [@marcofiap](https://github.com/marcofiap) |
| Paulo Henrique Senise | [@PauloSenise](https://github.com/PauloSenise) |

### Professores

- Tutor:
- Coordenador: [André Godoi](https://github.com/agodoi)

---

## Projeto CardioIA – Fase 1: Batimentos de Dados

Este repositório consolida a base de dados inicial do projeto **CardioIA**, reunindo dados numéricos, textuais e visuais para apoiar as próximas fases de Machine Learning, NLP e Visão Computacional.

### Objetivo da atividade

Preparar três tipos de dados para o ecossistema de IA em cardiologia:

- Dados numéricos (IoT/estruturados) com variáveis clínicas.
- Dados textuais para análises com NLP.
- Dados visuais para análises com Visão Computacional.

---

## Estrutura do repositório

- `README.md`: documentação principal da atividade.
- `docs/`: textos utilizados na parte de NLP.

---

## Parte 1 – Dados Numéricos (IoT)

### 1. Descrição do dataset

O conjunto de dados utilizado é o **Heart Disease UCI**, amplamente empregado em pesquisas de predição de doença cardíaca. Ele reúne registros reais e anonimizados de pacientes submetidos a avaliação cardiológica, contendo variáveis clínicas e exames que ajudam a identificar a presença ou ausência de doença cardíaca.

O arquivo preparado para este projeto está em formato `.csv` e pode ser acessado publicamente neste link:

- **Nome do arquivo:** `heart_disease_uci_fiap.csv`
- **Quantidade de linhas:** mais de 100 registros de pacientes
- **Formato:** dados tabulares separados por vírgula
- **Link público (OneDrive):** <https://fiapcom-my.sharepoint.com/:x:/g/personal/rm563348_fiap_com_br/IQAT-Vjp7l7kR5zIWhHUSeC_Adrphnq-Az6Y-vAk-Nx_384?e=BMm1KE>

### 2. Origem e governança dos dados

Este dataset é uma versão do banco de dados de doença cardíaca disponibilizado originalmente pelo **UCI Machine Learning Repository**, também amplamente utilizado em projetos públicos no GitHub e no Kaggle.

Os dados foram coletados em instituições de saúde e são fornecidos de forma anonimizada, sem identificação direta de pacientes, o que permite uso acadêmico e de pesquisa.

Para manter aderência aos princípios de governança e privacidade:

- Os dados são usados apenas em contexto acadêmico.
- Não há informações de identificação pessoal.
- O arquivo publicado está em modo de leitura.

### 3. Variáveis disponíveis

As principais colunas do arquivo são:

- **`age`**: idade do paciente.
- **`sex`**: sexo biológico.
- **`cp`**: tipo de dor torácica.
- **`trestbps`**: pressão arterial de repouso.
- **`chol`**: colesterol sérico total.
- **`fbs`**: glicemia em jejum.
- **`restecg`**: resultado do eletrocardiograma de repouso.
- **`thalach`**: frequência cardíaca máxima atingida no teste de esforço.
- **`exang`**: angina induzida por exercício.
- **`oldpeak`**: depressão do segmento ST em relação ao repouso.
- **`slope`**: inclinação do segmento ST no pico do exercício.
- **`ca`**: número de vasos principais visíveis na fluoroscopia.
- **`thal`**: tipo de talassemia.
- **`target`**: presença de doença cardíaca.

### 4. Variáveis clinicamente mais relevantes para IA

Do ponto de vista clínico e para modelos de IA aplicados à cardiologia, as variáveis mais relevantes são:

- **Idade (`age`)**: auxilia a estratificação do risco basal cardiovascular.
- **Pressão arterial de repouso (`trestbps`)**: representa risco relacionado à hipertensão.
- **Colesterol sérico (`chol`)**: variável-chave para risco de doença arterial coronariana.
- **Glicemia em jejum (`fbs`)**: contribui para identificar perfis cardiometabólicos de maior risco.
- **Frequência cardíaca máxima (`thalach`)**: indica resposta funcional ao esforço.
- **Angina induzida por exercício (`exang`)**: marcador clínico importante de isquemia.
- **Segmento ST (`oldpeak` e `slope`)**: captura alterações eletrocardiográficas associadas à isquemia.
- **Variável-alvo (`target`)**: permite treinamento supervisionado para classificação.

### 5. Importância para o projeto CardioIA

Esse conjunto de dados numéricos é relevante para:

- Treinar modelos de Machine Learning para predição de risco de doença cardíaca.
- Simular sistemas de triagem automática em pronto atendimento.
- Explorar vieses e limitações de modelos em saúde, como diferenças entre sexos e faixas etárias.

### Fontes de referência e créditos

- UCI Machine Learning Repository (Heart Disease Dataset).
- Repositório de apoio: <https://github.com/aqlopes/Kaggle-s-Heart-Disease-UCI-Dataset-Project/tree/master>
- Instituto Húngaro de Cardiologia (Andras Janosi, MD).
- Hospital Universitário de Zurique (William Steinbrunn, MD).
- Hospital Universitário da Basileia (Matthias Pfisterer, MD).
- Cleveland Clinic Foundation e VA Medical Center (Robert Detrano, MD, PhD).

---

## Parte 2 – Dados Textuais (NLP)

### Arquivos textuais selecionados

- `docs/sintomas_e_remomendacoes_cardio`
- `docs/taxa_sobrevivencia_taxa_reinter`

### Como os textos podem ser explorados por NLP

- **Extração de entidades (NER):** sintomas, exames, biomarcadores e tratamentos.
- **Classificação de tópicos:** sintomas, diagnóstico, prognóstico e condutas terapêuticas.
- **Análise de gravidade textual:** priorização de casos por descrição clínica.

### Relevância para o CardioIA

Esses textos permitem trabalhar com dados não estruturados, cenário comum em prontuários e literatura médica, ampliando a capacidade analítica dos módulos inteligentes de saúde cardiovascular.

---

## Parte 3 – Dados Visuais (VC)

### Dataset de imagens de ECG para análise com IA

Este repositório contém as informações e a estrutura do dataset de eletrocardiogramas (ECG) utilizado para o desenvolvimento de modelos de classificação e análise baseados em Inteligência Artificial e Visão Computacional.

### Fonte do dataset

O dataset utilizado neste projeto contém imagens de eletrocardiogramas (ECG) organizadas em diferentes categorias de condições cardíacas.

- **Dataset original (Kaggle)**: [ECG Images Dataset](https://www.kaggle.com/datasets/jayaprakashpondy/ecgimages)
- **Dataset utilizado no projeto (Google Drive)**: [Link Público](https://drive.google.com/file/d/1JOOX7FmhFE6hO973BTJDF2UP2vJyXfHv/view?usp=drive_link)
- **Tipo de exame escolhido:** ECG

---

### Estrutura do dataset

O dataset original foi distribuído no arquivo compactado `archive.zip`. Após a extração, os dados são organizados na seguinte estrutura:

```text
archive
│
├── train
│   ├── Normal Person ECG Images
│   ├── ECG Images of Patient that have abnormal heartbeat
│   ├── ECG Images of Patient that have History of MI
│   └── ECG Images of Myocardial Infarction Patients
│
└── test
    ├── Normal Person ECG Images
    ├── ECG Images of Patient that have abnormal heartbeat
    ├── ECG Images of Patient that have History of MI
    └── ECG Images of Myocardial Infarction Patients
```

### Divisão dos dados
A separação entre `train` e `test` é fundamental para o fluxo de aprendizado de máquina:
- **Treinamento (train):** Utilizado para o ajuste dos pesos do modelo.
- **Avaliação (test):** Utilizado para validar a capacidade de generalização do modelo em dados não vistos.

---

### Descrição das classes

Cada subpasta representa uma condição clínica específica identificada nos exames de ECG:

1. **Normal Person ECG Images:** Imagens de eletrocardiogramas considerados normais.
2. **ECG Images of Patient that have abnormal heartbeat:** Imagens com batimentos cardíacos anormais (arritmias).
3. **ECG Images of Patient that have History of MI:** Imagens de pacientes com histórico prévio de infarto do miocárdio.
4. **ECG Images of Myocardial Infarction Patients:** Imagens de pacientes atualmente sofrendo um infarto do miocárdio.

---

### Metodologia de análise

#### Visão computacional
As imagens de ECG são analisadas utilizando técnicas de visão computacional para extrair informações digitais diretamente dos traçados. Algumas operações comuns incluem:
- **Detecção de bordas:** Para isolar o traçado do fundo.
- **Extração de características:** Identificação de picos (P, QRS, T).
- **Segmentação de padrões:** Divisão do exame em ciclos cardíacos.
- **Classificação automática:** Atribuição de uma categoria clínica à imagem.

#### Redes neurais convolucionais (CNN)
O modelo principal para este projeto é a **Rede Neural Convolucional (CNN)**, ideal para reconhecimento de padrões visuais. O fluxo de processamento envolve:

1. **Camadas Convolucionais:** Identificação de padrões visuais como linhas, curvas e formas do traçado.
2. **Camadas de Pooling:** Redução da dimensão da imagem mantendo as características mais relevantes.
3. **Camadas Densas:** Processamento final para a classificação em uma das quatro categorias mencionadas.

---

### Objetivo
Automatizar a triagem de exames de ECG, auxiliando profissionais de saúde na detecção rápida de anomalias cardíacas, especialmente casos críticos de Infarto do Miocárdio.

---

## Entregáveis da atividade

- README detalhado com descrição das três partes.
- Pasta `docs/` ou `assets/` com os arquivos textuais.
- Links públicos para os conjuntos numérico, textual e visual.

---

## Governança de dados e viés

Para manter aderência à proposta da atividade:

- Priorizar fontes confiáveis e rastreáveis.
- Evitar uso de dados com identificação pessoal.
- Considerar representatividade de sexo, idade e perfil clínico.
- Documentar claramente origem, limitações e possíveis vieses.

