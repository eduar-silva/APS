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

**Classificação MoSCoW (marque uma):** [X] Must have (essencial)  [ ] Should have (importante)  [ ] Could have (desejável)  [ ] Won't have nesta versão (fora do escopo atual)

**Justificativa da prioridade:** O requisito é indispensável e constitui o núcleo da solução, sendo fundamental para resolver diretamente o problema central de localização, orientação ou segurança dos estudantes. Sem ele, o sistema perde sua utilidade principal e não atinge o objetivo de eliminar as principais dificuldades enfrentadas pelos calouros no campus.

## 6. Critérios de aceitação


| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado que o usuário está na tela de protocolo. Quando cadastra um novo documento preenchendo todos os campos obrigatórios. | O sistema registra a produção/recepção e gera um número de protocolo único. | Mensagem de sucesso na interface exibindo o número do protocolo gerado. |
| CA-02 | Dado que um documento está em tramitação. Quando o setor responsável encaminha o documento para o próximo destino. | O sistema atualiza a localização e o histórico de movimentação do documento. |Consulta à linha do tempo/histórico do documento mostrando o novo setor de destino. |
| CA-03 | Dado que o documento chegou ao destino final. Quando o responsável conclui a última etapa administrativa. | O sistema altera o status do documento para "Concluído" e encerra o trâmite. | Status atualizado visível na listagem de protocolos finalizados. |
| CA-04 | Dado que o usuário tenta tramitar um documento sem preencher o setor de destino. Quando aciona o botão de envio | O sistema bloqueia a ação e exibe um alerta de campo obrigatório pendente. | Alerta visual de erro na tela e o documento permanece no setor de origem. |

## 7. Validação e rastreabilidade

| Campo | Preenchimento |
|---|---|
| Situação | [X] Pendente de validação  [ ] Validado  [ ] Necessita revisão |
| Validado por / data |Ainda não validado. A revisão por pares e a validação com o stakeholder estão pendentes. |
| Observações e decisões | Requisito classificado como Must have e incluído na primeira versão (ordem 1). Pendências levantadas na revisão: definir o tempo máximo para confirmação de recebimento no setor de destino (RQ04) e as regras para documentos de trâmite prioritário (RF02). |
| Links relacionados | Rastreabilidade: Rastreabilidade: N01 → ST01 → REQ-001 (RF01), relacionado a RF08, RQ01, RQ03, RQ04 e RQ05. |
