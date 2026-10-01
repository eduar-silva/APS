# Ficha de Elicitação de Requisitos

**Curso:** Engenharia de Software  
**Disciplina:** Análise e Projeto de Sistemas  
**Instituição:** UDF Centro Universitário  
**Grupo/integrantes:** [Arthur Miguel Pinheiro](https://github.com/thurzxdev) | [Artur Miguel Monteiro](https://github.com/arturmm-s) | [Eduardo Brito](https://github.com/eduar-silva) | Marcos Guilherme | Daniel Gomes Lima 

**Turma:** D2 - Engenharia de Software  **Data:** 27/09/2026  **Versão:** 1.0

## 1. Identificação do projeto

| Campo | Preenchimento |
|---|---|
| Nome do projeto | Sistema de acolhida aos calouros da UDF. |
| Objetivo do projeto | O Sistema de Acolhida aos Calouros da UDF foi desenvolvido com o objetivo de facilitar a integração dos novos estudantes à vida acadêmica, oferecendo informações relevantes, suporte inicial e orientação sobre os principais serviços e recursos disponíveis na instituição. |
| Contexto e escopo | O sistema permite que os calouros da UDF tenham acesso facilitado a informações sobre os campus, serviços disponíveis e situações comuns que podem ocorrer durante a rotina acadêmica. |

## 2. Stakeholder e fonte

| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | ST01 — Alunos da UDF, principalmente os °calouros°. |
| Relação com o projeto | Usuário alvo: Aqueles que necessitam de uma informação de forma rápida e simples e que encontram dificuldades em consegui-las. |
| Contato ou setor (se aplicável) | Corpo discente da UDF (com foco principal nos calouros). |
| Técnica e data da elicitação | Contexto e Observação do Problema (Setembro de 2026). |
| Responsável pelo registro | Grupo do projeto (integrantes listados no cabeçalho). |

## 3. Requisito elicitado

| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-001 (refere ao RF-01 do levantamento de requisitos). |
| Necessidade relatada pelo stakeholder | Permitir buscar e visualizar a localização geográfica interna de salas, blocos, laboratórios e setores.administrativos. |
| Descrição consolidada | O sistema deve fornecer uma busca com visualização da planta interna dos campus como , salas, blocos, laboratórios e setores.administrativos. |
| Justificativa ou benefício esperado | Eliminar a dependência exclusiva de consultas verbais a funcionários e guardas, reduzir o estresse na adaptação ao campus e agilizar a chegada dos estudantes aos locais corretos. |
| Tipo | Funcional |
| Dependências ou dúvidas | Depende da disponibilidade inicial de dados cadastrais corretos sobre a infraestrutura da instituição (inseridos via RF05). |

## 4. Regras de negócio

| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-001 | Unicidade de Salas: Não pode haver duas salas cadastradas com o mesmo identificador (código/número) dentro do mesmo bloco. (Associado a: RF01, RF05) | Coordenação de Infraestrutura / Administrador do Sistema |
| RN-002 | Validação de Alocação: O sistema não deve permitir que duas turmas diferentes sejam alocadas na mesma sala no mesmo dia e horário. (Associado a: RF02) | Setor de Horários e Ensalamento / Coordenação Acadêmica |
| RN-003 | Permissão de Notificação: Apenas usuários cadastrados com o perfil "Administrador" ou "Coordenador" podem disparar comunicados para os estudantes. (Associado a: RF03) | Gestão Institucional / Coordenação |
| RN-004 | Tempo de Resposta da Busca: O motor de busca por salas e blocos deve carregar as sugestões de auto-completar em menos de 1 segundo. (Associado a: RNF02) | Equipe de Desenvolvimento / Requisitos de Desempenho |

## 5. Prioridade

**Classificação MoSCoW (marque uma):** [ ] Must have (essencial)  [X] Should have (importante)  [ ] Could have (desejável)  [ ] Won't have nesta versão (fora do escopo atual)

**Justificativa da prioridade:** O requisito é indispensável e constitui o núcleo da solução, sendo fundamental para resolver diretamente o problema central de localização, orientação ou segurança dos estudantes. Sem ele, o sistema perde sua utilidade principal e não atinge o objetivo de eliminar as principais dificuldades enfrentadas pelos calouros no campus.

## 6. Critérios de aceitação

Escreva condições verificáveis que permitam decidir se o requisito foi atendido.

| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | | | |
| CA-02 | | | |
| CA-03 | | | |

## 7. Validação e rastreabilidade

| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [ ] Validado  [ ] Necessita revisão |
| Validado por / data | |
| Observações e decisões | |
| Links relacionados | Issue, protótipo, caso de uso ou documento de origem. |

## Exemplo breve (fictício)

**Projeto:** Sistema de agendamento de atendimento acadêmico. **Objetivo:** permitir que estudantes reservem horários disponíveis. **Stakeholder:** estudante; entrevista em 24/09/2026. **REQ-001:** “Quero escolher um horário de atendimento pelo celular”. **Descrição:** O sistema deve permitir ao estudante autenticado reservar um horário disponível de atendimento. **RN-001:** um horário não pode receber mais de uma reserva ativa. **Prioridade:** Must have, pois a reserva é a função central. **CA-01:** dado um horário disponível, quando o estudante confirmar a reserva, então o sistema registra a reserva e retira o horário da lista de disponibilidade. **CA-02:** dado um horário já reservado, quando outro estudante tentar reservá-lo, então o sistema impede a duplicidade e apresenta uma mensagem clara.

## Como organizar no GitHub

1. No repositório do projeto, crie a pasta `docs/requisitos/`.
2. Salve esta ficha preenchida como `docs/requisitos/ficha-elicitacao-REQ-001.md`. Crie um arquivo por requisito, alterando o ID de forma sequencial. Guarde a versão PDF de cada ficha na mesma pasta, se a entrega também exigir PDF.
3. Pelo site do GitHub, use **Add file > Upload files** (ou crie/edite o Markdown com **Add file > Create new file**). Confirme os arquivos com uma mensagem de commit descritiva, como `docs: adiciona ficha de elicitação REQ-001`.
4. Atualize o `README.md` na raiz do repositório com uma seção de documentação e o link relativo:

```md
## Documentação de requisitos

- [Ficha de elicitação REQ-001](docs/requisitos/ficha-elicitacao-REQ-001.md)
- [Versão para impressão (PDF)](docs/requisitos/ficha-elicitacao-REQ-001.pdf)
```

5. Confira no GitHub se os links abrem e se o ID do arquivo coincide com o ID registrado na ficha. Atualize a ficha após validação, preservando o histórico de commits.
