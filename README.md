# ⭐ Modelo Dimensional Estrela - Projeto DIO

Este repositório apresenta um projeto de modelagem dimensional no formato estrela, criado como exercício prático a partir de um modelo relacional proposto pela DIO (Digital Innovation One).

## 📌 Objetivo

Transformar um modelo relacional de uma base acadêmica em um modelo dimensional, com foco na tabela fato **Professor** e as demais tabelas e granularidade por minha responsabilidade, conforme instrução do desafio.

---

## 🗂️ Estrutura do Projeto

### 🔷 Imagem 1 - Modelo Relacional (fornecido pela DIO)
![Modelo Relacional](https://github.com/DaDosValle/Imagens/blob/main/Modelo%20Relacional%20DIO.png)

O modelo relacional representa um banco de dados universitário com tabelas como:
- Professor
- Curso
- Departamento
- Disciplina
- Matrícula
- Aluno
- Pré-requisitos

Para este projeto, **a tabela Aluno e Matrícula foram desconsideradas**, pois o foco é a análise dos **professores**, suas **avaliações**, **cursos**, **departamentos** e **datas** relacionadas.

---

### 🌟 Imagem 2 - Modelo Dimensional em Estrela (proposto)

![Modelo Dimensional Estrela](https://github.com/DaDosValle/Imagens/blob/main/MOdelo%20DImensional%20-Estrela.png)

O modelo estrela gerado contém:

#### ✅ Tabela Fato
- **Professor**
  - Contém as chaves estrangeiras para as dimensões: Data, Curso, Departamento e Avaliação.
  - Inclui informações para análises como: formação, localização, CPF, e-mail, telefone etc.

#### 📊 Tabelas Dimensão
- **D_Data**: permite análises por data, semestre, mês, trimestre e ano.
- **D_Curso**: permite análises por curso, disciplinas e requisitos do curso.
- **D_Departamento**: permite segmentações por campus e localização do departamento.
- **D_Avaliação**: permite análises por tipo, data de aplicação e pontuação máxima.

---

## 🔍 Por que um Modelo Dimensional?

Modelos dimensionais são ideais para análise de dados (BI/Data Warehousing) por:

- Simplicidade na estrutura (fácil leitura e manutenção).
- Melhora na performance em consultas OLAP.
- Otimização para agregações e análises temporais ou categóricas.

---

## 🛠️ Ferramentas Utilizadas

- 💻 MySQL Workbench (modelagem visual)
- 🧠 Conceitos de Data Warehouse
- 🧱 Modelagem Estrela (Star Schema)

---

## 📫 Contato

Se você tiver dúvidas, sugestões ou quiser trocar ideias, fique à vontade para me chamar por aqui ou criar um issue!

---
