# 🏋️ PowerOn Academia

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Academic Project](https://img.shields.io/badge/Academic-Project-blue?style=for-the-badge)
![Data Structures](https://img.shields.io/badge/Data%20Structures-Binary%20Tree-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Concluído-green?style=for-the-badge)

Sistema de **gestão acadêmica para uma academia**, desenvolvido em **Python com Flask**, utilizando o conceito de **arquivos indexados** e **árvore binária em memória** para simular um banco de dados simples e eficiente.

O projeto foi desenvolvido em **dupla**, com foco no aprendizado de **estruturas de dados**, **persistência em arquivos**, **organização de sistemas** e **boas práticas de programação**, sem o uso de ferramentas de geração automática de código.

---

## 📌 Descrição do Projeto

O sistema **PowerOn Academia** tem como objetivo gerenciar os dados de uma academia fictícia, mantendo registros de:

- Alunos
- Professores
- Modalidades
- Matrículas
- Cidades

A aplicação simula um **banco de dados próprio**, onde:

- A **área de índices** é implementada como uma **Árvore Binária**, mantida em memória
- A **área de dados** é persistida em **arquivos armazenados em disco**, garantindo a integridade dos dados entre execuções

---

## 🚀 Funcionalidades

### 🔹 Operações Básicas
- Inclusão de registros
- Consulta de registros
- Exclusão de registros
- Leitura exaustiva das tabelas
- Todas as operações utilizam **índice em árvore binária**

---

### 🔹 Regras de Negócio Implementadas

#### 👤 Alunos
- Exibição do **nome da cidade** e **estado** (consulta cruzada com Cidades)
- Cálculo automático do **IMC**
- Diagnóstico de IMC:
  - Abaixo do peso
  - Peso normal
  - Sobrepeso
  - Obesidade

#### 👨‍🏫 Professores
- Exibição do **nome da cidade** e **estado** associados ao professor

#### 🏃 Modalidades
- Exibição do **nome do professor**
- Exibição da **cidade do professor**
- Controle de limite de alunos por modalidade

#### 📝 Matrículas
- Verificação automática de **vagas disponíveis**
- Incremento/decremento do total de alunos matriculados
- Cálculo do **valor a ser pago**:

- Exibição de:
- Nome do aluno
- Cidade do aluno
- Descrição da modalidade
- Nome do professor

---

### 💰 Faturamento por Modalidade
- Consulta do faturamento total de uma modalidade específica
- Exibição de:
- Descrição da modalidade
- Nome do professor
- Cidade do professor
- Valor total faturado

---

### 📊 Relatório Geral de Matrículas
- Exibição de todas as matrículas em **ordem crescente do código**
- Dados exibidos:
- Código da Matrícula
- Nome do Aluno
- Cidade do Aluno
- Modalidade
- Professor
- Valor a ser pago
- Ao final:
- Total de alunos matriculados
- Valor total a ser pago

---

## 🗂️ Estruturas de Dados (Tabelas)

Cada tabela é armazenada em **arquivo separado**:

### 📍 Cidades
- Código da Cidade
- Descrição
- Estado

### 👤 Alunos
- Código do Aluno
- Nome
- Código da Cidade
- Data de Nascimento
- Peso
- Altura

### 👨‍🏫 Professores
- Código do Professor
- Nome
- Endereço
- Telefone
- Código da Cidade

### 🏃 Modalidades
- Código da Modalidade
- Descrição
- Código do Professor
- Valor da Aula
- Limite de Alunos
- Total de Alunos Matriculados

### 📝 Matrículas
- Código da Matrícula
- Código do Aluno
- Código da Modalidade
- Quantidade de Aulas

---

## 🛠️ Tecnologias Utilizadas

- **Python**
- **Flask**
- Arquivos Texto/Binários
- Árvore Binária (estrutura de índice)
- Programação Estruturada e Modular

---

## ▶️ Como Executar o Projeto

### Pré-requisitos
- Python 3.10 ou superior
- Ambiente virtual (opcional, recomendado)

### Execução
```bash
python app.py
