# Matrix Calculator — ICCOM 2026

Projeto interdisciplinar desenvolvido para a unidade curricular ICCOM, com foco em desenvolvimento colaborativo, organização de equipa e boas práticas de engenharia de software.

Este repositório contém:
- API em C para operações com matrizes
- Relatório web (HTML/CSS/JS)
- Testes manuais e automáticos
- Documentação técnica e organizacional

---

## 📂 Estrutura do Repositório

```
matrix-calculator-iccom-2026/
├── api/
│   ├── main.c
│   ├── matrix_ops.c
│   └── matrix_ops.h
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── tests/
│   ├── manual/
│   └── robot/
├── docs/
│   ├── fluxograma.png
│   ├── casos_uso.png
│   └── plano_testes.md
├── LICENSE
└── README.md
```

---

## 👥 Equipa

### Frontend
- **Elizandro Paquete**
- **Gabriel Souza**

### Backend
- **Catarina**
- **David Evidência**

### Fullstack
- **David Evidência**

### QA
- **Gabriel Souza**

---

## 🔧 Tecnologias Utilizadas

- **C** — Lógica da aplicação
- **HTML/CSS/JavaScript** — Relatório web
- **Robot Framework** — Testes automáticos
- **Git & GitHub** — Controlo de versão e colaboração
- **GitHub Projects** — Gestão de tarefas

---

## 🧭 Fluxo de Trabalho (Git)

Para manter o projeto organizado, seguimos este fluxo simples:

### Branches principais
- `main` → Versão final e estável
- `dev` → Desenvolvimento contínuo

### Branches de trabalho
Cada tarefa tem a sua própria branch:

- `feature/...` → Novas funcionalidades
- `fix/...` → Correções
- `qa/...` → Testes e documentação

### Criar uma branch

```bash
git checkout dev
git pull
git checkout -b feature/nome-da-tarefa
```

### Enviar alterações

```bash
git add .
git commit -m "Descrição da tarefa"
git push -u origin feature/nome-da-tarefa
```

### Pull Request
Todos os PRs devem ser feitos para a branch `dev`.

---

## 📋 Fluxo de Trabalho (Quadro GitHub)

O projeto utiliza um quadro simples com 4 colunas:

| Coluna | Descrição |
|--------|-----------|
| **To do** | Tarefas ainda não iniciadas |
| **In progress** | Alguém está a trabalhar |
| **Review** | Pull Request aberto |
| **Done** | Tarefa concluída e PR aprovado |

### Regras
- Cada tarefa é criada como **Issue**
- Quando alguém começa a trabalhar → mover para **In progress**
- Quando abrir PR → mover para **Review**
- Quando o PR for aprovado → mover para **Done**

---

## 🧪 Testes

### Testes manuais
Localizados em: `/tests/manual`

### Testes automáticos (Robot Framework)
Localizados em: `/tests/robot`

Para executar:
```bash
robot tests/robot
```

---

## 🧠 Funcionalidades da API (Sprint 1)

- ✅ Criar e ler matrizes
- ✅ Validar dimensões
- ✅ Soma de matrizes
- ✅ Subtração de matrizes
- ✅ Menu inicial em consola

---

## 📌 Objetivo do Projeto

Desenvolver uma aplicação modular em C para operações com matrizes, acompanhada de documentação, testes e relatório web, aplicando boas práticas de desenvolvimento colaborativo.

---

## 📄 Licença

Projeto académico — uso livre para fins educativos.

---

# 📋 Templates e Documentação

## 🔖 Template de Issue

Quando criares uma nova Issue no GitHub, usa este formato:

```markdown
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
Issue relacionada: #
Pull Request relacionado: #
```

---

## 📥 Template de Pull Request

Quando criares um Pull Request, usa este formato:

```markdown
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
```

---

## 🗂️ README do Project Board

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

1. **Criar Issue** → aparece em **To do**
2. **Começar a trabalhar** → mover para **In progress**
3. **Abrir Pull Request** → mover para **Review**
4. **PR aprovado** → mover para **Done**

## 🧪 Regras

- Cada tarefa deve ter Issue
- Cada Issue deve ter branch própria
- Todos os PRs vão para `dev`
- Só o QA move para Done

---

## 📊 Fluxograma da Aplicação

```
┌──────────────────┐
│     INÍCIO       │
└────────┬─────────┘
         │
         ▼
┌─────────────────────┐
│ Mostrar menu        │
│ principal           │
└────────┬────────────┘
         │
    ┌────┴────┬───────────┬────────────┐
    │         │           │            │
    ▼         ▼           ▼            ▼
┌───────┐ ┌──────┐ ┌───────────┐ ┌──────┐
│ [1]   │ │ [2]  │ │   [3]     │ │ [4]  │
│Criar  │ │Somar │ │ Subtrair  │ │Sair  │
│matriz │ │      │ │           │ │      │
└───┬───┘ └──┬───┘ └─────┬─────┘ └──┬───┘
    │        │            │           │
    ▼        ▼            ▼           ▼
┌──────┐ ┌──────┐   ┌──────┐    ┌──────┐
│Ler   │ │Valid.│   │Valid.│    │Encer-│
│dimen.│ │dimen.│   │dimen.│    │rar   │
└──┬───┘ └──┬───┘   └──┬───┘    └──────┘
   │        │           │
   ▼        ▼           ▼
┌──────┐ ┌──────┐   ┌──────┐
│Valid.│ │Calcu-│   │Calcu-│
│      │ │lar   │   │lar   │
└──┬───┘ └──┬───┘   └──┬───┘
   │        │           │
   ▼        ▼           ▼
┌──────┐ ┌──────────────┐
│Guar- │ │Mostrar       │
│dar   │ │resultado     │
└──────┘ └──────────────┘
         │
         ▼
    ┌────────┐
    │  FIM   │
    └────────┘
```

### Descrição das operações:

1. **Criar matrizes** → Ler dimensões → Validar → Guardar matriz
2. **Somar matrizes** → Validar dimensões → Calcular → Mostrar resultado
3. **Subtrair matrizes** → Validar dimensões → Calcular → Mostrar resultado
4. **Sair** → Encerrar programa

---

## 👤 Diagrama de Casos de Uso

```
                    ┌─────────────────┐
                    │                 │
                    │  Utilizador     │
                    │                 │
                    └────────┬────────┘
                             │
           ┌─────────────────┼─────────────────┐
           │                 │                 │
           ▼                 ▼                 ▼
    ┌──────────┐      ┌──────────┐     ┌──────────┐
    │  Criar   │      │  Somar   │     │ Subtrair │
    │  matriz  │      │ matrizes │     │ matrizes │
    └──────────┘      └──────────┘     └──────────┘
           │                 │                 │
           └─────────────────┼─────────────────┘
                             │
                             ▼
                      ┌──────────┐
                      │Visualizar│
                      │resultado │
                      └──────────┘
                             │
                             ▼
                      ┌──────────┐
                      │   Sair   │
                      │aplicação │
                      └──────────┘
```

### Casos de uso:

**Ator:** Utilizador

**Casos de uso:**
- Criar matriz
- Ler matriz
- Somar matrizes
- Subtrair matrizes
- Visualizar resultado
- Sair da aplicação

**Relações:**
- Utilizador → Criar matriz
- Utilizador → Somar matrizes
- Utilizador → Subtrair matrizes
- Utilizador → Visualizar resultado
- Utilizador → Sair

---

## 🧪 Plano de Testes Completo

### 1. Objetivo
Garantir que todas as funcionalidades da aplicação funcionam corretamente e sem erros.

### 2. Tipos de Testes
- Testes funcionais
- Testes de validação
- Testes de erro
- Testes automáticos (Robot Framework)

### 3. Funcionalidades a testar

#### 3.1 Criar matriz

| Teste | Entrada | Resultado Esperado |
|-------|---------|-------------------|
| Dimensões válidas | 3x3 | Matriz criada com sucesso |
| Dimensões inválidas (0) | 0x0 | Erro: Dimensão inválida |
| Dimensões negativas | -2x3 | Erro: Dimensão inválida |
| Dimensões muito grandes | 31x31 | Erro: Dimensão máxima excedida (>30) |
| Valores válidos | Números inteiros/decimais | Valores guardados corretamente |
| Valores inválidos | Letras ou caracteres especiais | Erro: Valor inválido |

#### 3.2 Soma de matrizes

| Teste | Entrada | Resultado Esperado |
|-------|---------|-------------------|
| Matrizes compatíveis | 2x2 + 2x2 | Soma calculada corretamente |
| Matrizes incompatíveis | 2x3 + 3x2 | Erro: Dimensões incompatíveis |
| Resultados corretos | A[1,2] + B[3,4] = C[4,6] | Valores corretos |

#### 3.3 Subtração de matrizes

| Teste | Entrada | Resultado Esperado |
|-------|---------|-------------------|
| Matrizes compatíveis | 3x3 - 3x3 | Subtração calculada corretamente |
| Matrizes incompatíveis | 2x2 - 3x3 | Erro: Dimensões incompatíveis |
| Resultados corretos | A[5,6] - B[2,3] = C[3,3] | Valores corretos |

#### 3.4 Menu

| Teste | Entrada | Resultado Esperado |
|-------|---------|-------------------|
| Opção válida | 1, 2, 3 ou 4 | Funcionalidade correspondente executada |
| Opção inválida | 0, 5, letras | Erro: Opção inválida |
| Sair corretamente | 4 | Programa encerra sem erros |

### 4. Critérios de Aceitação
- ✅ Todas as operações funcionam
- ✅ Não existem crashes
- ✅ Mensagens de erro claras
- ✅ Testes automáticos passam

### 5. Testes Automáticos

**Localização:** `/tests/robot`

**Comando para executar:**
```bash
robot tests/robot
```

**Estrutura dos testes:**
```
tests/robot/
├── test_criar_matriz.robot
├── test_soma.robot
├── test_subtracao.robot
└── test_menu.robot
```

### 6. Checklist de Testes

Antes de fazer merge para `dev` ou `main`, verificar:

- [ ] Todos os testes manuais passam
- [ ] Todos os testes automáticos passam
- [ ] Código compilado sem erros
- [ ] Sem memory leaks (valgrind)
- [ ] Documentação atualizada
- [ ] PR revisto por pelo menos 1 pessoa

---

## 📞 Contactos e Suporte

Para questões ou problemas, abre uma [Issue](../../issues) no GitHub ou contacta a equipa através do grupo do projeto.

---

**Desenvolvido com 💻 pela equipa ICCOM 2026**

