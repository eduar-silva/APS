Introdução à Análise e Projeto de Sistemas de Informação.
Conceitos e elementos fundamentais da engenharia de software - definição, características e tipos de
modelagens. Ferramentas Case de apoio ao desenho dos diagramas UML


# Ficha de Requisitos — Aula 02

## Análise e Projeto de Sistemas

**Unidade:** II — Introdução à Análise e Projeto de Sistemas  
**Atividade:** Transformação do levantamento do sistema em requisitos funcionais e não funcionais  
**Objetivo:** Registrar, de forma estruturada, o que o sistema deve fazer e quais características de qualidade deve atender.

---

## 1. Identificação do Sistema

| Campo | Preenchimento |
|---|---|
| Nome do sistema | Acolhida de calouros |
| Objetivo | Recepcionar da melhor maneira os calouros |
| Público-alvo | Calouros |
| Responsável pelo levantamento | 
| 1 | [Arthur Miguel Pinheiro](https://github.com/thurzxdev) |
| 2 | [Artur Miguel Monteiro](https://github.com/arturmm-s) |
| 3 | [Eduardo Brito](https://github.com/eduar-silva) |
| 4 | [Marcos Guilherme](https://github.com/guima-Eng) |
| 5 | [Daniel Gomes Lima](https://github.com/DanielGomesSoftwer) |


| Versão | 1.0 |

---

# 2. Requisitos Funcionais

> Requisitos funcionais descrevem **funcionalidades ou serviços que o sistema deve oferecer**.

## RF01 — Cadastrar calouro

| Campo | Descrição |
|---|---|
| **Identificação** | RF01 |
| **Descrição** | O sistema deve permitir que usuários autorizados cadastrem novos calouros. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Deve permitir informar nome, matrícula, e-mail, telefone e curso. 2. Deve impedir cadastro sem nome e matrícula. 3. Deve impedir o cadastro de uma matrícula já existente. 4. Deve informar ao usuário quando o cadastro for concluído. |
| **Exemplo** | O responsável informa os dados de um novo calouro e seleciona **Cadastrar**. O sistema valida os dados e registra o novo aluno. |

## RF02 — Consultar informações do calouro

| Campo | Descrição |
|---|---|
| **Identificação** | RF02 |
| **Descrição** | O sistema deve permitir que o calouro consulte suas informações cadastradas. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Deve permitir consultar nome, matrícula, e-mail, telefone e curso. 2. Deve apresentar os dados cadastrados do calouro. 3. Deve informar quando os dados não forem encontrados. |
| **Exemplo** | O calouro acessa seu perfil e o sistema apresenta seus dados pessoais e acadêmicos cadastrados. |

## RF03 — Cadastrar atividade de acolhida

| Campo | Descrição |
|---|---|
| **Identificação** | RF03 |
| **Descrição** | O sistema deve permitir que usuários autorizados cadastrem atividades de acolhida para os calouros. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Deve permitir informar nome da atividade, descrição, data, horário e local. 2. Deve impedir o cadastro sem nome, data e local. 3. Deve apresentar confirmação após o cadastro. |
| **Exemplo** | O responsável cadastra uma palestra de boas-vindas, informa a data, o horário e o local, e o sistema registra a atividade. |

## RF04 — Consultar programação

| Campo | Descrição |
|---|---|
| **Identificação** | RF04 |
| **Descrição** | O sistema deve permitir que os calouros consultem a programação das atividades de acolhida. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Deve permitir visualizar as atividades cadastradas. 2. Deve apresentar nome, data, horário e local de cada atividade. 3. Deve informar quando não houver atividades disponíveis. |
| **Exemplo** | O calouro acessa a programação e verifica as atividades de acolhida que acontecerão durante a semana. |

## RF05 — Realizar inscrição em atividade

| Campo | Descrição |
|---|---|
| **Identificação** | RF05 |
| **Descrição** | O sistema deve permitir que os calouros realizem inscrição nas atividades de acolhida disponíveis. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Deve permitir selecionar uma atividade disponível. 2. Deve registrar a inscrição do calouro. 3. Deve impedir inscrição em atividade que não esteja disponível. 4. Deve informar ao usuário quando a inscrição for concluída. |
| **Exemplo** | O calouro seleciona uma palestra de boas-vindas e confirma sua inscrição. O sistema registra a participação na atividade. |

## RF06 — Registrar presença em atividade

| Campo | Descrição |
|---|---|
| **Identificação** | RF06 |
| **Descrição** | O sistema deve permitir registrar a presença dos calouros nas atividades de acolhida. |
| **Prioridade** | Média |
| **Critérios de aceitação** | 1. Deve localizar o calouro cadastrado. 2. Deve registrar a presença na atividade. 3. Deve impedir o registro para um calouro inexistente. 4. Deve permitir consultar os participantes da atividade. |
| **Exemplo** | Durante uma palestra, o responsável localiza o calouro no sistema e registra sua presença na atividade. |

---

# 3. Requisitos Não Funcionais

> Requisitos não funcionais descrevem **características, restrições e condições de qualidade** que o sistema deve atender.

## RNF01 — Segurança

| Campo | Descrição |
|---|---|
| **Identificação** | RNF01 |
| **Descrição** | O sistema deve controlar o acesso às funcionalidades conforme o perfil do usuário. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Usuários devem autenticar-se antes de acessar funções restritas. 2. Funcionalidades administrativas devem estar disponíveis somente a perfis autorizados. 3. Os dados dos calouros devem ser protegidos contra acesso não autorizado. |
| **Exemplo** | Um calouro não pode acessar a funcionalidade de cadastro de atividades, disponível somente para usuários autorizados. |

## RNF02 — Usabilidade

| Campo | Descrição |
|---|---|
| **Identificação** | RNF02 |
| **Descrição** | A interface deve apresentar informações e comandos de forma clara, simples e consistente. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Os campos devem possuir rótulos claros. 2. Mensagens de erro devem orientar o usuário. 3. As ações principais devem ser facilmente identificáveis. |
| **Exemplo** | Ao deixar a matrícula vazia durante o cadastro, o sistema informa que o campo é obrigatório. |

## RNF03 — Desempenho

| Campo | Descrição |
|---|---|
| **Identificação** | RNF03 |
| **Descrição** | Consultas comuns devem apresentar resposta em tempo adequado para o uso cotidiano. |
| **Prioridade** | Média |
| **Critérios de aceitação** | Em condições normais de operação, consultas simples devem apresentar o resultado em até 3 segundos. |
| **Exemplo** | Ao consultar a programação de atividades, o resultado deve ser apresentado em até 3 segundos. |

## RNF04 — Disponibilidade

| Campo | Descrição |
|---|---|
| **Identificação** | RNF04 |
| **Descrição** | O sistema deve estar disponível durante o período de acolhida dos calouros. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | O sistema deve permanecer acessível durante o período definido pela instituição, exceto em manutenções previamente programadas. |
| **Exemplo** | Durante a semana de acolhida, os calouros conseguem acessar o sistema para consultar atividades e realizar inscrições. |

## RNF05 — Integridade dos dados

| Campo | Descrição |
|---|---|
| **Identificação** | RNF05 |
| **Descrição** | O sistema deve preservar a consistência dos dados registrados dos calouros e das atividades. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Não deve permitir duas matrículas iguais. 2. Não deve permitir inscrição em atividade inexistente. 3. Um registro de presença deve estar associado a um calouro e a uma atividade válidos. |
| **Exemplo** | Ao tentar cadastrar um calouro com uma matrícula já existente, o sistema bloqueia o cadastro e informa o motivo. |

---

# 4. Modelo para preenchimento pelos estudantes

## Requisito Funcional

| Campo | Resposta do grupo |
|---|---|
| Identificação | RF__ |
| Descrição | |
| Prioridade | Alta / Média / Baixa |
| Critérios de aceitação | |
| Exemplo | |

## Requisito Não Funcional

| Campo | Resposta do grupo |
|---|---|
| Identificação | RNF__ |
| Descrição | |
| Prioridade | Alta / Média / Baixa |
| Critérios de aceitação | |
| Exemplo | |

---

# 5. Orientações para elaboração

Para cada requisito, o grupo deve verificar:

- **Identificação:** possui código único?
- **Descrição:** está claro o que o sistema deve fazer ou qual característica deve apresentar?
- **Prioridade:** é essencial, importante ou pode ser implementado posteriormente?
- **Critérios de aceitação:** é possível verificar objetivamente se o requisito foi atendido?
- **Exemplo:** existe uma situação concreta que demonstra o requisito?

## Regra prática

Um bom requisito deve ser:

**Claro + específico + verificável + relevante**

---

# 6. Entregável da atividade

O grupo deverá entregar:

1. Identificação do sistema;
2. Pelo menos **5 requisitos funcionais**;
3. Pelo menos **3 requisitos não funcionais**;
4. Prioridade de cada requisito;
5. Critérios de aceitação;
6. Exemplo de utilização;
7. Identificação dos integrantes do grupo: (3 a 6 integrantes)
