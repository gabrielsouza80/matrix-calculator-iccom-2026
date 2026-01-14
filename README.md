# Matrix Calculator — ICCOM 2026

Projeto interdisciplinar desenvolvido para a unidade curricular ICCOM, com foco em desenvolvimento colaborativo, organização de equipa e boas práticas de engenharia de software.

Este repositório contém:
- API em C para operações com matrizes
- Relatório web (HTML/CSS/JS)
- Testes manuais e automáticos
- Documentação técnica e organizacional

---

## 📂 Estrutura do Repositório

/api Código-fonte da aplicação em C - main.c - matrix_ops.c - matrix_ops.h
/frontend Relatório web do projeto - index.html - style.css - script.js
/tests Testes manuais e automáticos /manual /robot
/docs Diagramas, fluxogramas e documentação adicional

---

## 👥 Equipa

### Frontend
- Elizandro Paquete  
- Gabriel Souza  

### Backend
- Catarina  
- David Evidência  

### Fullstack
- David Evidência  

### QA
- Gabriel Souza  

---

## 🔧 Tecnologias Utilizadas

- **C** (lógica da aplicação)
- **HTML/CSS/JavaScript** (relatório web)
- **Robot Framework** (testes automáticos)
- **Git & GitHub** (controlo de versão e colaboração)
- **GitHub Projects** (gestão de tarefas)

---

## 🧭 Fluxo de Trabalho (Git)

Para manter o projeto organizado, seguimos este fluxo simples:

### Branches principais
- `main` → versão final e estável  
- `dev` → desenvolvimento contínuo  

### Branches de trabalho
Cada tarefa tem a sua própria branch:

- `feature/...` → novas funcionalidades  
- `fix/...` → correções  
- `qa/...` → testes e documentação  

### Criar uma branch

```bash
git checkout dev
git pull
git checkout -b feature/nome-da-tarefa
```

###Enviar alterações
git add .
git commit -m "Descrição da tarefa"
git push -u origin feature/nome-da-tarefa

Pull Request
Todos os PRs devem ser feitos para a branch .

📋 Fluxo de Trabalho (Quadro GitHub)
O projeto utiliza um quadro simples com 4 colunas:
• 	To do → tarefas ainda não iniciadas
• 	In progress → alguém está a trabalhar
• 	Review → Pull Request aberto
• 	Done → tarefa concluída e PR aprovado
Regras
• 	Cada tarefa é criada como Issue
• 	Quando alguém começa a trabalhar → mover para In progress
• 	Quando abrir PR → mover para Review
• 	Quando o PR for aprovado → mover para Done

🧪 Testes

Testes manuais
Localizados em:
/tests/manual

Testes automáticos (Robot Framework)
Localizados em:
/tests/robot

Para executar:
robot tests/robot

🧠 Funcionalidades da API (Sprint 1)
• 	Criar e ler matrizes
• 	Validar dimensões
• 	Soma de matrizes
• 	Subtração de matrizes
• 	Menu inicial em consola

📌 Objetivo do Projeto
Desenvolver uma aplicação modular em C para operações com matrizes, acompanhada de documentação, testes e relatório web, aplicando boas práticas de desenvolvimento colaborativo.

📄 Licença
Projeto académico — uso livre para fins educativos.

✅ 1. TEMPLATE DE ISSUE
---
name: "Nova Tarefa"
about: Criar uma nova tarefa para o projeto
title: ""
labels: ""
assignees: ""
---

## 📌 Descrição
Descreve claramente o que deve ser feito.

## 🎯 Objetivo
Qual é o resultado esperado desta tarefa?

## 📂 Local do trabalho
- [ ] /api
- [ ] /frontend
- [ ] /tests
- [ ] /docs

## 🧪 Critérios de Aceitação
- [ ] Funciona como esperado
- [ ] Código limpo e organizado
- [ ] Testado manualmente
- [ ] PR aberto para `dev`

## 🔗 Ligações
Issue relacionada:  
Pull Request relacionado:

✅ 2. TEMPLATE DE PULL REQUEST
# 📥 Pull Request

## 📌 Descrição
Explica o que foi feito nesta branch.

## 🧩 Tipo de alteração
- [ ] Nova funcionalidade
- [ ] Correção de bug
- [ ] Documentação
- [ ] Testes
- [ ] Refatoração

## 📂 Áreas afetadas
- [ ] /api
- [ ] /frontend
- [ ] /tests
- [ ] /docs

## 🧪 Testes realizados
Descreve como testaste a funcionalidade.

## ✔ Critérios de aceitação
- [ ] Funciona corretamente
- [ ] Código limpo
- [ ] Sem erros de compilação
- [ ] Testes manuais feitos
- [ ] Revisão necessária

## 🔗 Issue relacionada
Closes #

✅ 3. README DO PROJECT BOARD
# 🧭 Quadro Scrum — Matrix Calculator

Este quadro organiza o fluxo de trabalho do projeto de forma simples e eficiente.

## 📌 Colunas

### To do
Tarefas ainda não iniciadas.

### In progress
Tarefas em desenvolvimento.

### Review
Tarefas com Pull Request aberto e à espera de revisão.

### Done
Tarefas concluídas e PR aprovado.

## 🔄 Fluxo de Trabalho
1. Criar Issue → aparece em **To do**  
2. Começar a trabalhar → mover para **In progress**  
3. Abrir Pull Request → mover para **Review**  
4. PR aprovado → mover para **Done**

## 🧪 Regras
- Cada tarefa deve ter Issue
- Cada Issue deve ter branch própria
- Todos os PRs vão para `dev`
- Só o QA move para Done

✅ 4. FLUXOGRAMA DA APLICAÇÃO (versão texto)
INÍCIO
   ↓
Mostrar menu principal
   ↓
[1] Criar matrizes → Ler dimensões → Validar → Guardar matriz
   ↓
[2] Somar matrizes → Validar dimensões → Calcular → Mostrar resultado
   ↓
[3] Subtrair matrizes → Validar dimensões → Calcular → Mostrar resultado
   ↓
[4] Sair → Encerrar programa
   ↓
FIM

✅ 5. DIAGRAMA DE CASOS DE USO (versão texto)
Ator: Utilizador

Casos de uso:
- Criar matriz
- Ler matriz
- Somar matrizes
- Subtrair matrizes
- Visualizar resultado
- Sair da aplicação

Relações:
Utilizador → Criar matriz
Utilizador → Somar matrizes
Utilizador → Subtrair matrizes
Utilizador → Visualizar resultado
Utilizador → Sair

✅ 6. PLANO DE TESTES COMPLETO
# Plano de Testes — Matrix Calculator

## 1. Objetivo
Garantir que todas as funcionalidades da aplicação funcionam corretamente e sem erros.

## 2. Tipos de Testes
- Testes funcionais
- Testes de validação
- Testes de erro
- Testes automáticos (Robot Framework)

## 3. Funcionalidades a testar

### 3.1 Criar matriz
- Inserir dimensões válidas
- Inserir dimensões inválidas (0, negativos, >30)
- Inserir valores válidos
- Inserir valores inválidos

### 3.2 Soma de matrizes
- Matrizes compatíveis
- Matrizes incompatíveis
- Resultados corretos

### 3.3 Subtração de matrizes
- Matrizes compatíveis
- Matrizes incompatíveis
- Resultados corretos

### 3.4 Menu
- Opções válidas
- Opções inválidas
- Sair corretamente

## 4. Critérios de Aceitação
- Todas as operações funcionam
- Não existem crashes
- Mensagens de erro claras
- Testes automáticos passam

## 5. Testes Automáticos
Localização:
/tests/robot

Comando:
robot tests/robot

