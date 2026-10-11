# Desafio de Projeto: Modelagem Dimensional (Star Schema) com Power BI

Repositório criado para a entrega do desafio de projeto da **DIO (Digital Innovation One)**, focado na transformação de um modelo relacional transacional em um modelo dimensional em estrela (**Star Schema**), com foco analítico na atuação docente.

## 🎯 Objetivo do Projeto
O objetivo principal foi redesenhar a arquitetura de dados de uma universidade para otimizar consultas analíticas no Power BI. O escopo foi direcionado para a **análise dos dados dos professores**, contemplando os cursos ministrados, departamentos, disciplinas e uma tabela dimensão de calendário criada para dar suporte às análises temporais.

---

## 🛠️ Arquitetura do Modelo (Star Schema)

O modelo dimensional final é composto por:

1. **Fato (`Fato_Professores`)**: Tabela central que armazena as métricas quantitativas e chaves estrangeiras de ligação:
   - Carga Ministrada, Quantidade de Alunos por Turma e Valor da Hora-Aula.
2. **Dimensões (`Dim_`)**:
   - **Dim_Professor**: Dados cadastrais dos docentes.
   - **Dim_Departamento**: Informações dos departamentos e campi.
   - **Dim_Curso**: Catálogo de cursos oferecidos pela instituição.
   - **Dim_Disciplina**: Detalhes das disciplinas associadas.
   - **Dim_Calendario**: Tabela dimensão de tempo customizada para análises temporais por ano, mês, trimestre e dia da semana.

---

## 📂 Estrutura do Repositório

```text
├── assets/          # Prints do modelo relacional original e do Star Schema no Power BI
├── data/            # Planilha Excel estructurada para a modelagem
├── powerbi/         # Arquivo do relatório em Power BI (.pbix)
└── README.md        # Documentação do projeto