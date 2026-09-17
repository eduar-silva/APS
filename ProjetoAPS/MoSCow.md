Modelo do template: https://miro.com/pt/modelos/moscow-matrix-basic/

# 📋 Projeto de APS - Sistema de acolhida aos calouros da UDF

## Levantamento e Priorização de Requisitos

**Etapa:** Levantamento de Requisitos (Utilizar a ficha dos requisitos levantados)
**Técnica de Priorização:** MoSCoW
**Data:** 10/09/2026
**Turma:** Engenharia de Software UDF - D2

---

# 👥 1. Identificação do Grupo

| Integrante | Nome |
|---|---|
| 1 | Arthur Miguel Pinheiro |
| 2 | Artur Miguel Monteiro |
| 3 | Eduardo Brito |
| 4 | Marcos Guilherme |
| 5 | |

---

# 2. Identificação do Projeto

**Nome do projeto:**
> Sistema de acolhida aos calouros da UDF

**Descrição resumida do projeto:**
> O Sistema de Acolhida aos Calouros da UDF foi desenvolvido com o objetivo de facilitar a integração dos novos estudantes à vida acadêmica, oferecendo informações relevantes, suporte inicial e orientação sobre os principais serviços e recursos disponíveis na instituição.

---

# 3. Problema Identificado

## 3.1 Qual problema será resolvido?

> O Problema identificado é a falta de instrução aos novos alunos (calouros).

---

## 3.2 Quem é afetado pelo problema?

> Os principais usuários são alunos, tanto novos quanto veteranos, que precisam de orientações.

---

## 3.3 Como o problema é resolvido atualmente?

> Guardas, funcionários e alunos da instituição são consultados para orientar.

---

## 3.4 Principais dificuldades encontradas

1. Perda de tempo e risco de atrasos nas primeiras aulas ou atendimentos por não saber onde fica cada setor.
2. Escassez de pessoas disponíveis ou com tempo hábil para fornecer o suporte necessário no momento da dúvida.
3. Falta de sinalização clara ou de mapas acessíveis pelo campus para a localização autônoma.

---

# 🎯 4. Objetivo do Projeto

> Nosso projeto pretende oferecer um acesso rápido, digital e centralizado a informações e localizações da instituição para os estudantes, contribuindo para eliminar a dependência exclusiva de consultas verbais a funcionários, evitar atrasos nas aulas, garantir uma transição mais organizada, eficiente e sem estresse para a vida acadêmica, e promover sua rápida adaptação ao campus com maior autonomia.

---

# 👤 5. Stakeholders

| ID | Stakeholder | Papel | Necessidade/Interesse | Influência |
|---|---|---|---|---|
| ST01 | Alunos Calouros | Usuário Principal | Obter orientações rápidas. | Alta |
| ST02 | Alunos Veteranos | Usuário Secundário | Consulta a atualizações no campus. | Média |
| ST03 | Funcionários Administrativos | Informante | Redução de dúvidas repetitivas no atendimento. | Média |
| ST04 | Segurança do Campus | Informante de Rotas | Menos interrupções nas funções de segurança. | Baixa |
| ST05 | Coordenação | Gestor Institucional | Melhoria na experiência inicial e retenção dos alunos. | Alta |

---

## Stakeholder principal

**Stakeholder:**
> Alunos Calouros.

**Por que ele foi considerado o principal stakeholder?**
> Porque representam o público que mais enfrenta barreiras de adaptação, dependendo exclusivamente de orientações presenciais e sofrendo com a desorientação nos primeiros dias.

---

# 🗣️ 6. Levantamento de Informações

| Pergunta | Resposta |
|---|---|
| O que o usuário precisa fazer? | Localizar salas, blocos e setores do campus; descobrir qual setor resolve cada tipo de problema; consultar horários de atendimento; esclarecer dúvidas comuns dos primeiros dias sem precisar perguntar a alguém. |
| Qual problema enfrenta atualmente? | Depende de perguntar a guardas, funcionários ou veteranos, que nem sempre estão disponíveis ou sabem informar, o que gera atrasos, filas no balcão e sensação de desorientação. |
| Quais informações precisa consultar? | Mapa do campus, localização de salas e blocos, lista de setores e serviços (secretaria, biblioteca, tesouraria, coordenação, laboratórios), horários de funcionamento, contatos, calendário acadêmico, eventos de acolhida e avisos. |
| Quais informações precisa cadastrar ou alterar? | O aluno praticamente não cadastra nada (apenas envia dúvidas/feedback). O cadastro e a alteração de setores, locais, horários, avisos e perguntas frequentes são feitos pelo funcionário administrativo autorizado. |
| Quais tarefas são repetitivas? | Responder sempre às mesmas perguntas ("onde fica a secretaria?", "como tiro a carteirinha?", "qual a senha do Wi-Fi?") e indicar o caminho até os mesmos locais. |
| Quais tarefas consomem mais tempo? | Procurar uma sala pelo campus por tentativa e erro e enfrentar filas de atendimento presencial apenas para obter uma informação simples. |
| Quais erros acontecem atualmente? | Informações divergentes entre as pessoas consultadas, orientação para o bloco ou horário errado e uso de dados desatualizados (setor que mudou de lugar ou de horário). |
| Precisa receber notificações? | Sim, de forma simples: avisos sobre eventos de acolhida, mudanças de sala e datas importantes do calendário acadêmico. Notificações push não são essenciais na primeira versão. |
| Precisa gerar documentos ou relatórios? | Não para o aluno. Para a coordenação, é desejável um relatório simples com as buscas e dúvidas mais frequentes, para orientar melhorias na sinalização física. |
| Existem informações que precisam ser protegidas? | Sim: as credenciais de acesso da área administrativa e eventuais dados pessoais informados no envio de dúvidas (nome, matrícula, e-mail), protegidos conforme a LGPD. |
| O sistema precisará se comunicar com outros sistemas? | Não na primeira versão. É desejável, no futuro, integrar com o sistema acadêmico da UDF (calendário e grade de horários do aluno). |
| Existem regras obrigatórias que precisam ser respeitadas? | Sim: apenas pessoal autorizado pela coordenação pode publicar ou alterar informações institucionais; todo conteúdo deve ter responsável e data de atualização; o tratamento de dados pessoais deve seguir a LGPD (Lei 13.709/2018). |

---

# 💡 7. Necessidades Identificadas

| ID | Stakeholder | Necessidade Identificada | Problema Relacionado |
|---|---|---|---|
| N01 | ST01 | Localizar salas, blocos e setores do campus de forma autônoma. | 3.4.1 e 3.4.3 — perda de tempo e falta de sinalização/mapas. |
| N02 | ST01 | Encontrar rapidamente um local específico sem percorrer todo o mapa. | 3.4.1 — risco de atraso nas primeiras aulas. |
| N03 | ST01 | Saber a função, o horário de atendimento e o contato de cada setor. | 3.4.2 — dependência de pessoas para informações simples. |
| N04 | ST01 | Obter respostas para as dúvidas mais comuns dos primeiros dias. | 3.4.2 — escassez de pessoas disponíveis no momento da dúvida. |
| N05 | ST01 e ST05 | Conhecer datas importantes e eventos de acolhida do início do semestre. | 3.4.2 — informação dispersa e transmitida apenas verbalmente. |
| N06 | ST02 | Consultar mudanças e atualizações ocorridas no campus. | 3.4.3 — ausência de canal centralizado de informação. |
| N07 | ST03 e ST05 | Manter as informações do campus atualizadas de forma simples e centralizada. | 3.4.2 e erros por informação desatualizada. |
| N08 | ST04 | Reduzir as interrupções para orientação de rotas durante o trabalho. | 3.4.2 — segurança usada como serviço de informação. |

---

# ⚙️ 8. Requisitos Funcionais

## Requisitos Funcionais do Projeto

| ID | Requisito Funcional | Stakeholder/Fonte | Necessidade | Prioridade |
|---|---|---|---|---|
| RF01 | O sistema deve permitir que o usuário visualize o mapa digital do campus com a identificação dos blocos, andares e setores. | ST01 / ST04 | N01 | M |
| RF02 | O sistema deve permitir que o usuário busque um local pelo nome do setor, número da sala ou serviço desejado. | ST01 | N02 | M |
| RF03 | O sistema deve exibir a rota sugerida entre a entrada principal (ou ponto selecionado) e o local consultado. | ST01 / ST04 | N01, N08 | S |
| RF04 | O sistema deve permitir que o usuário consulte a lista de setores e serviços com descrição da função, horário de atendimento e contato. | ST01 / ST03 | N03 | M |
| RF05 | O sistema deve disponibilizar uma seção de perguntas frequentes (FAQ) com as dúvidas mais comuns dos calouros. | ST01 / ST03 | N04 | M |
| RF06 | O sistema deve exibir um mural com avisos, eventos de acolhida e datas do calendário acadêmico. | ST01 / ST02 / ST05 | N05, N06 | S |
| RF07 | O sistema deve permitir que o funcionário autorizado cadastre, altere e remova setores, locais, horários, avisos e perguntas frequentes. | ST03 / ST05 | N07 | M |
| RF08 | O sistema deve permitir que o usuário envie dúvidas ou sugestões e que o administrador visualize as mensagens recebidas. | ST01 / ST05 | N04, N07 | C |

---

# ⭐ 9. Requisitos de Qualidade

## Requisitos de Qualidade do Projeto

| ID | Característica de Qualidade | Requisito | Como será verificado? |
|---|---|---|---|
| RQ01 | Desempenho | O sistema deve apresentar o resultado das buscas por local em até 2 segundos para 95% das requisições, considerando conexão de 3 Mbps. | Teste de carga com 50 buscas simultâneas, medindo o tempo de resposta e verificando o percentil 95. |
| RQ02 | Segurança | O sistema deve exigir autenticação por login e senha para acesso à área administrativa, armazenar as senhas com hash e encerrar a sessão após 15 minutos de inatividade. | Teste de tentativa de acesso direto à URL administrativa sem login, inspeção do banco de dados e teste de expiração de sessão. |
| RQ03 | Usabilidade/Interação | Um usuário sem treinamento prévio deve conseguir localizar um setor do campus em até 1 minuto e no máximo 3 cliques/toques, em pelo menos 90% dos casos. | Teste de usabilidade com 10 calouros, cronometrando a tarefa e contando os cliques. |
| RQ04 | Confiabilidade | O sistema deve ficar disponível em pelo menos 99% do horário letivo (07h às 23h) e, em caso de falha no carregamento do mapa, exibir mensagem de erro e a lista de setores como alternativa. | Monitoramento de disponibilidade por 30 dias e teste de falha simulada desativando o componente do mapa. |
| RQ05 | Compatibilidade/Portabilidade | O sistema deve funcionar via navegador nas duas versões mais recentes de Chrome, Firefox e Edge e em telas a partir de 320px de largura (Android 8+ e iOS 13+), sem necessidade de instalação. | Execução do roteiro de testes nos navegadores indicados e em emuladores de dispositivos móveis. |

---

# 🚧 10. Restrições

| ID | Restrição | Categoria | Justificativa/Fonte |
|---|---|---|---|
| RES01 | O projeto deve ser concluído e entregue dentro do semestre letivo, conforme o cronograma da disciplina. | Prazo | Cronograma da APS definido pela professora da disciplina. |
| RES02 | O desenvolvimento deve utilizar apenas ferramentas gratuitas ou de código aberto e hospedagem sem custo, pois o grupo não dispõe de orçamento. | Orçamento/Recursos | Projeto acadêmico sem verba institucional. |
| RES03 | O sistema deve ser executado via navegador web, sem exigir instalação, e funcionar com a conexão Wi-Fi disponível no campus. | Tecnologia/Infraestrutura | Grande parte dos calouros usa o celular e tem pouco espaço de armazenamento; a rede do campus é instável em alguns blocos. |
| RES04 | O tratamento de dados pessoais dos usuários deve respeitar a LGPD (Lei nº 13.709/2018). | Legislação | Exigência legal aplicável ao envio de dúvidas com identificação do aluno. |

---

# 📜 11. Regras de Negócio

| ID | Regra de Negócio | Fonte |
|---|---|---|
| RN01 | A consulta ao mapa, aos setores e às perguntas frequentes é de acesso público e não exige autenticação do usuário. | Coordenação (ST05) |
| RN02 | Somente usuários com perfil administrativo, autorizados pela coordenação, podem cadastrar, alterar ou excluir informações institucionais publicadas no sistema. | Coordenação (ST05) |
| RN03 | Toda informação publicada deve registrar o responsável pela publicação e a data da última atualização; informações sem atualização há mais de 6 meses devem ser sinalizadas para revisão. | Funcionários Administrativos (ST03) |
| RN04 | Dados pessoais informados no envio de dúvidas só podem ser utilizados para responder à solicitação e devem ser excluídos mediante pedido do titular. | Legislação (LGPD) |

---

# 🔗 12. Rastreabilidade Inicial

| Necessidade | Stakeholder | Requisito(s) relacionado(s) |
|---|---|---|
| N01 | ST01 | RF01, RF03, RQ03 |
| N02 | ST01 | RF02, RQ01 |
| N03 | ST01, ST03 | RF04, RQ04 |
| N04 | ST01 | RF05, RF08 |
| N05 | ST01, ST05 | RF06 |
| N06 | ST02 | RF06, RF01 |
| N07 | ST03, ST05 | RF07, RF08, RQ02 |
| N08 | ST04 | RF03, RF01 |

---

# 🏷️ 13. Priorização dos Requisitos — Técnica MoSCoW

| Categoria | Significado |
|---|---|
| 🔴 **M — Must Have** | Requisito indispensável |
| 🟠 **S — Should Have** | Muito importante, mas pode esperar temporariamente |
| 🟢 **C — Could Have** | Desejável se houver tempo e recursos |
| ⚪ **W — Won't Have Now** | Não será implementado nesta entrega |

---

## Matriz de Priorização

| ID | Requisito | MoSCoW | Justificativa |
|---|---|:---:|---|
| RF01 | Visualizar o mapa digital do campus | 🔴 M | É o núcleo da solução; sem o mapa o sistema não resolve a dificuldade principal de localização. |
| RF02 | Buscar local por nome, sala ou serviço | 🔴 M | Sem busca, o aluno precisaria percorrer todo o mapa, mantendo a perda de tempo que o projeto quer eliminar. |
| RF03 | Exibir rota até o local | 🟠 S | Agrega muito valor e reduz a dependência da segurança, mas o aluno já se orienta com o mapa e a busca. |
| RF04 | Consultar setores, horários e contatos | 🔴 M | Saber onde fica não basta: o aluno precisa saber o que cada setor faz e quando está aberto. |
| RF05 | Perguntas frequentes (FAQ) | 🔴 M | Responde diretamente às dúvidas repetitivas, que são a principal causa de procura por funcionários. |
| RF06 | Mural de avisos e calendário | 🟠 S | Importante para a acolhida e para os veteranos, mas o conteúdo pode ser divulgado por outros canais temporariamente. |
| RF07 | Cadastro e atualização pelo administrador | 🔴 M | Sem manutenção, o conteúdo fica desatualizado e o sistema passa a reproduzir o erro de informação incorreta. |
| RF08 | Envio de dúvidas e sugestões | 🟢 C | Desejável para evoluir o FAQ, porém o aluno ainda pode recorrer ao atendimento presencial. |
| RQ01 | Busca em até 2s (95% das requisições) | 🟠 S | O sistema precisa ser ágil para valer a pena, mas um pequeno atraso não inviabiliza o uso na primeira versão. |
| RQ02 | Autenticação e proteção da área administrativa | 🔴 M | Sem controle de acesso, qualquer pessoa poderia alterar informações institucionais, violando a RN02. |
| RQ03 | Usabilidade: localizar setor em até 1 min e 3 cliques | 🔴 M | O público-alvo usa o sistema justamente quando está com pressa e perdido; complexidade anula o benefício. |
| RQ04 | Disponibilidade de 99% no horário letivo | 🟠 S | Fundamental a médio prazo, mas depende de infraestrutura de hospedagem que o grupo não controla totalmente (RES02). |
| RQ05 | Compatibilidade com navegadores e celulares | 🔴 M | O uso ocorre em deslocamento pelo campus, pelo celular; sem responsividade o sistema não é utilizável. |

---

# 🚀 14. Requisitos da Primeira Versão

| Ordem | ID | Requisito | Por que deve estar na primeira versão? |
|:---:|---|---|---|
| 1 | RF01 | Visualizar o mapa digital do campus | Resolve a dificuldade central do problema investigado: a localização autônoma dos setores. |
| 2 | RF02 | Buscar local por nome, sala ou serviço | Torna o mapa realmente útil sob pressão de tempo, evitando atrasos nas primeiras aulas. |
| 3 | RF04 | Consultar setores, horários e contatos | Substitui a consulta verbal a funcionários, que é a forma atual de resolver o problema. |
| 4 | RF05 | Perguntas frequentes (FAQ) | Elimina de imediato as dúvidas repetitivas que sobrecarregam o atendimento presencial. |
| 5 | RF07 | Cadastro e atualização pelo administrador | Garante que o conteúdo permaneça confiável e atualizado, sustentando todos os demais requisitos. |

> Requisitos de qualidade que acompanham a primeira versão: RQ02 (segurança da área administrativa), RQ03 (usabilidade) e RQ05 (compatibilidade com dispositivos móveis).

---

# ⏭️ 15. Requisitos para Versões Futuras

| ID | Requisito | Motivo para adiar | Impacto |
|---|---|---|---|
| RF03 | Exibir rota sugerida até o local | Exige mapeamento detalhado dos percursos internos e mais tempo de desenvolvimento do que o prazo da disciplina permite (RES01). | Baixo/Médio: o aluno ainda se localiza pelo mapa e pela busca, com um pouco mais de esforço. |
| RF06 | Mural de avisos e calendário acadêmico | Depende do fornecimento contínuo de conteúdo pela coordenação e, idealmente, de integração com o sistema acadêmico, indisponível agora. | Médio: os avisos continuam sendo divulgados por e-mail e redes sociais institucionais. |
| RF08 | Envio de dúvidas e sugestões | Envolve tratamento de dados pessoais (RES04/RN04) e rotina de resposta que ainda não está definida com os setores. | Baixo: o atendimento presencial e o FAQ cobrem provisoriamente essa necessidade. |
| RQ04 | Disponibilidade de 99% no horário letivo | Depende de hospedagem paga e monitoramento, incompatíveis com a restrição de orçamento (RES02). | Médio: eventuais indisponibilidades obrigam o aluno a recorrer ao meio atual (perguntar a alguém). |

---

# 🔍 16. Revisão por Pares

**Grupo responsável pela revisão:** __________________________

| ID do Requisito | Problema Encontrado | Sugestão de Melhoria |
|---|---|---|
| RF01 | A redação inicial dizia apenas "mostrar o mapa do campus", sem indicar o nível de detalhe esperado. | Especificar que o mapa identifica blocos, andares e setores, tornando o requisito verificável. |
| RF04 | O requisito reunia consulta de setores, horários e contatos com o envio de mensagens, ferindo o critério de capacidade única. | Separar o envio de mensagens em um requisito próprio (RF08). |
| RQ01 | O termo "rápido" era ambíguo e não permitia teste. | Definir métrica objetiva: até 2 segundos em 95% das requisições, com condição de rede declarada. |
| RQ04 | A disponibilidade estava definida como "sempre disponível", o que é inviável com hospedagem gratuita. | Ajustar para 99% no horário letivo e prever comportamento alternativo em caso de falha. |
| RF07 | Não estava claro quem seria o "funcionário autorizado". | Vincular o requisito à regra de negócio RN02, que define a autorização pela coordenação. |

---

# ✅ 17. Checklist de Qualidade dos Requisitos

- [x] Os requisitos estão completos?
- [x] Os requisitos estão corretos em relação às necessidades?
- [x] Cada requisito representa uma única capacidade ou característica?
- [x] Os requisitos são necessários?
- [x] Os requisitos são viáveis?
- [x] Todos possuem prioridade?
- [x] Termos ambíguos foram eliminados?
- [x] Os requisitos podem ser verificados ou testados?
- [x] A fonte ou stakeholder está identificado?
- [x] As necessidades estão relacionadas aos requisitos?
- [x] Os requisitos de qualidade são mensuráveis sempre que possível?
- [x] As prioridades MoSCoW possuem justificativa?

---

# 💭 18. Reflexão do Grupo

## 18.1 Qual requisito gerou mais discussão durante o levantamento? Por quê?

> O RF03 (exibir rota até o local). Parte do grupo defendia que a navegação passo a passo era o grande diferencial do sistema, enquanto a outra parte argumentou que mapear todos os percursos internos dos blocos exigiria muito mais tempo do que o prazo da disciplina permite (RES01). A discussão terminou com o entendimento de que o mapa somado à busca já resolve a dificuldade principal, ficando a rota para uma versão futura.

---

## 18.2 Qual necessidade inicialmente parecia simples, mas gerou vários requisitos?

> A necessidade N01 ("saber onde fica cada lugar"). No início parecia se resolver com uma única tela de mapa, mas ao detalhar percebemos que ela se desdobrava em visualizar o mapa (RF01), buscar um local específico (RF02), traçar a rota (RF03) e ainda saber o que o setor faz e em que horário atende (RF04) — além de exigir usabilidade e responsividade (RQ03 e RQ05), já que a consulta acontece com o aluno andando pelo campus.

---

## 18.3 O grupo identificou algum requisito implícito durante a discussão?

> Sim. O RF07 (cadastro e atualização das informações) e o RQ02 (autenticação da área administrativa) não apareceram em nenhuma fala dos usuários, mas ficaram evidentes quando percebemos que informações desatualizadas fariam o sistema repetir o erro que ele pretende corrigir. Também surgiu de forma implícita a exigência de funcionamento no celular, já que ninguém consulta um mapa pelo computador enquanto procura uma sala.

---

## 18.4 Qual requisito foi mais difícil de priorizar utilizando MoSCoW? Por quê?

> O RF06 (mural de avisos e calendário). Para a coordenação (ST05) ele é altamente estratégico e seria um Must, mas para o aluno calouro (ST01), stakeholder principal, ele não resolve a dor imediata de se localizar. Como a priorização foi feita a partir do stakeholder principal e do problema declarado, o requisito ficou como Should Have.

---

## 18.5 Houve algum requisito inicialmente considerado Must que mudou de prioridade?

> Sim. O RQ04 (disponibilidade de 99%) foi inicialmente classificado como Must, mas foi rebaixado para Should ao confrontarmos a restrição de orçamento (RES02): sem hospedagem paga e monitoramento, o grupo não conseguiria garantir nem verificar esse nível de disponibilidade. O RF03 também começou como Must e passou a Should pelo mesmo tipo de análise, agora relacionada ao prazo.

---

# 📝 19. Conclusão

**Conclusão:**

> Este trabalho investigou a falta de orientação enfrentada pelos calouros da UDF, que atualmente dependem de consultas verbais a guardas, funcionários e veteranos para localizar setores e resolver dúvidas básicas, o que provoca perda de tempo, atrasos e sobrecarga do atendimento presencial. O levantamento identificou como stakeholders os alunos calouros (principal), os alunos veteranos, os funcionários administrativos, a segurança do campus e a coordenação, e revelou oito necessidades, com destaque para a localização autônoma de salas e setores, o conhecimento sobre a função e o horário de cada serviço, o esclarecimento das dúvidas mais comuns e a manutenção das informações atualizadas.
>
> A partir dessas necessidades foram especificados oito requisitos funcionais, cinco requisitos de qualidade mensuráveis, quatro restrições e quatro regras de negócio, todos rastreados até a necessidade e o stakeholder que os originaram. Consideramos essenciais o mapa digital do campus (RF01), a busca por local (RF02), a consulta de setores e horários (RF04), as perguntas frequentes (RF05) e a área de administração de conteúdo (RF07), acompanhados dos requisitos de segurança, usabilidade e compatibilidade.
>
> A técnica MoSCoW foi decisiva para separar o que é indispensável do que é apenas desejável. Ao obrigar o grupo a justificar cada classificação, ela expôs conflitos entre o interesse da coordenação e a dor real do calouro e evidenciou o peso das restrições de prazo e orçamento, levando ao adiamento consciente da rota guiada, do mural de avisos, do canal de dúvidas e da meta de disponibilidade. O resultado foi uma primeira versão enxuta, viável dentro do semestre e ainda assim capaz de resolver o problema central: dar ao calouro autonomia para se localizar e se informar no campus.

---

# 📦 Entregável

O repositório deverá apresentar, no mínimo:

- identificação do projeto e dos integrantes;
- descrição do problema;
- objetivo do projeto;
- stakeholders;
- levantamento das necessidades;
- **8 requisitos funcionais**;
- **5 requisitos de qualidade**;
- **3 restrições**;
- **3 regras de negócio**;
- rastreabilidade entre necessidades e requisitos;
- priorização utilizando **MoSCoW**;
- definição dos requisitos da primeira versão;
- revisão dos requisitos;
- reflexão e conclusão do grupo.

---

# 📚 Referência

REINEHR, Sheila. **Requisitos de Software**. Material de apoio utilizado na disciplina Engenharia de Requisitos.

---

**Disciplina:** Engenharia de Requisitos
**Projeto:** Levantamento e Priorização de Requisitos
**Profª Kadidja Valéria**
