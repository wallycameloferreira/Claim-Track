# Problema de Negócio

> Documentação da etapa de identificação e definição do problema de negócio do Claim Track.

## 1. Contexto
Empresas que realizam a gestão e tratamento de sinistros precisam coordenar diferentes atividades desde a comunicação de um sinistro até sua conclusão, envolvendo clientes, analistas, prestadores de serviço, oficinas, áreas financeiras e gestores.

O processo pode envolver o registro das informações do sinistro, análise da ocorrência, solicitação e recebimento de documentos, avaliação dos danos, realização de orçamentos, aprovação dos serviços, execução do reparo e posterior cobrança de valores ao cliente quando aplicável.

Quando essas informações são controladas por diferentes canais e ferramentas, como e-mail, telefone, planilhas, mensagens e sistemas isolados, torna-se mais difícil acompanhar o andamento de cada sinistro e garantir que todas as etapas sejam executadas corretamente.

O Claim Track surge como uma proposta de plataforma para centralizar e organizar esse processo.

## 2. Cenário Atual
No cenário atual, a comunicação e o tratamento dos sinistros podem ocorrer de forma descentralizada.

Um fluxo típico pode envolver:

Cliente comunica o sinistro
        ↓
Equipe recebe a comunicação
        ↓
Informações são registradas
        ↓
Sinistro é analisado
        ↓
Documentos são solicitados
        ↓
Danos são avaliados
        ↓
Orçamento é solicitado
        ↓
Orçamento é elaborado
        ↓
Orçamento é analisado/aprovado
        ↓
Serviço é realizado
        ↓
Custos são consolidados
        ↓
Valor devido pelo cliente é identificado
        ↓
Cobrança é realizada
        ↓
Sinistro é encerrado

Durante esse processo, diferentes participantes podem precisar consultar e atualizar informações do mesmo sinistro.

A ausência de um fluxo centralizado pode fazer com que informações importantes permaneçam distribuídas entre diferentes canais e ferramentas.

## 3. Problema
A empresa possui dificuldade em centralizar, acompanhar e controlar o ciclo de vida dos sinistros, desde sua comunicação até a tratativa, geração de orçamento e cobrança dos valores devidos pelo cliente.

A falta de uma visão única do processo pode dificultar:

o registro padronizado dos sinistros;
o acompanhamento do status de cada ocorrência;
o controle das atividades pendentes;
a comunicação entre os envolvidos;
o acompanhamento de documentos;
a elaboração e aprovação de orçamentos;
o controle dos serviços realizados;
a identificação dos valores a serem cobrados;
o acompanhamento das cobranças;
a geração de informações gerenciais.

Como consequência, o processo pode depender excessivamente de controles manuais e informações distribuídas em planilhas.

## 4. Impactos
O problema pode gerar impactos operacionais e financeiros, tais como:

**Operacionais**
dificuldade de acompanhar o andamento dos sinistros;
retrabalho na atualização de informações;
perda ou duplicidade de informações;
dificuldade para identificar atividades pendentes;
atrasos na tratativa;
comunicação descentralizada entre as equipes;
dificuldade para identificar responsáveis pelas atividades.
**Financeiros**
dificuldade no controle dos valores dos orçamentos;
divergências entre valores orçados e valores efetivamente realizados;
dificuldade na identificação dos valores a serem cobrados;
atrasos no processo de cobrança;
dificuldade para acompanhar valores recebidos e pendentes.
**Gerenciais**
dificuldade para obter indicadores do processo;
baixa visibilidade sobre o volume de sinistros;
dificuldade para identificar gargalos;
dificuldade para acompanhar prazos;
dificuldade para analisar custos e resultados.

## 5. Público Afetado
O processo pode envolver diferentes perfis de usuários e áreas.

**Público**	Participação no processo
**Cliente**	Comunica o sinistro, fornece informações/documentos, acompanha a tratativa e realiza pagamentos quando aplicável
**Analista de Sinistros**	Registra, analisa e acompanha o sinistro
**Gestor de Sinistros**	Supervisiona a operação, aprova tratativas e acompanha indicadores
**Prestador de Serviço**	Realiza serviços relacionados ao sinistro e fornece informações/orçamentos
**Oficina / Fornecedor**	Elabora orçamentos e executa serviços
**Financeiro**	Realiza ou acompanha o processo de cobrança
**Gestor Financeiro**	Acompanha valores, cobranças e indicadores financeiros
**Administrador do Sistema**	Gerencia usuários, permissões e configurações

## 6. Objetivo do Projeto
Desenvolver uma plataforma capaz de centralizar, controlar e dar rastreabilidade ao processo de gestão e tratativa de sinistros, permitindo acompanhar o sinistro desde sua comunicação até seu encerramento.

O sistema deverá apoiar principalmente:

1-comunicação do sinistro;
2-registro das informações;
3-análise e triagem;
4-controle da tratativa;
5-solicitação e gerenciamento de documentos;
6-geração e acompanhamento de orçamentos;
7-aprovação dos serviços;
8-acompanhamento da execução;
9-consolidação dos custos;
10-geração da cobrança ao cliente;
11-acompanhamento do pagamento;
12-encerramento do sinistro.

## 7. Visão da Solução

O Claim Track será uma plataforma centralizada para gerenciamento do ciclo de vida dos sinistros.

A solução deverá permitir que as informações sejam registradas e acompanhadas dentro de um fluxo estruturado.

**Visão inicial:**

                    CLAIM TRACK
                         │
                         ▼
              ┌────────────────────┐
              │ Comunicação        │
              │ do Sinistro        │
              └─────────┬──────────┘
                        ▼
              ┌────────────────────┐
              │ Registro e         │
              │ Triagem            │
              └─────────┬──────────┘
                        ▼
              ┌────────────────────┐
              │ Análise e          │
              │ Tratativa           │
              └─────────┬──────────┘
                        ▼
              ┌────────────────────┐
              │ Orçamento          │
              └─────────┬──────────┘
                        ▼
              ┌────────────────────┐
              │ Aprovação          │
              └─────────┬──────────┘
                        ▼
              ┌────────────────────┐
              │ Execução do        │
              │ Serviço            │
              └─────────┬──────────┘
                        ▼
              ┌────────────────────┐
              │ Apuração de        │
              │ Valores            │
              └─────────┬──────────┘
                        ▼
              ┌────────────────────┐
              │ Cobrança           │
              │ ao Cliente         │
              └─────────┬──────────┘
                        ▼
              ┌────────────────────┐
              │ Encerramento       │
              └────────────────────┘
A plataforma deverá manter o histórico das movimentações do sinistro, permitindo identificar o status atual, responsáveis, atividades realizadas, documentos, orçamentos, valores e demais informações relacionadas.

### Dentro do escopo
Dentro do escopo

O MVP do Claim Track deverá contemplar:

**Gestão de clientes**

cadastro de clientes;
consulta de dados;
histórico de sinistros relacionados ao cliente.

**Comunicação de sinistros**

abertura de sinistro;
registro da data e local da ocorrência;
descrição do evento;
identificação do cliente;
identificação do bem/veículo relacionado;
anexação de documentos e evidências.

**Gestão do sinistro**

classificação;
priorização;
atribuição de responsável;
alteração de status;
registro de atividades;
histórico do sinistro;
controle de pendências.

**Tratativa**

registro das ações realizadas;
solicitação de documentos;
acompanhamento de pendências;
registro de pareceres;
acompanhamento dos responsáveis.

**Orçamento**

solicitação de orçamento;
cadastro de itens e serviços;
valores;
fornecedores/prestadores;
envio para aprovação;
aprovação ou rejeição;
histórico das alterações.

**Execução**

acompanhamento dos serviços;
registro de execução;
custos realizados;
conclusão do serviço.

**Cobrança**

identificação do valor devido pelo cliente;
geração da cobrança;
acompanhamento do status da cobrança;
registro do pagamento;
controle de valores pendentes.

**Gestão**

consulta de sinistros;
filtros;
indicadores;
histórico;
acompanhamento de prazos e status.


### Fora do escopo

Nesta primeira versão, ficam fora do escopo:

processamento bancário próprio;
emissão de nota fiscal;
integração com instituições financeiras;
inteligência artificial para análise automática de sinistros;
aplicativos mobile nativos;
integração automática com seguradoras externas;
sistemas contábeis completos;
gestão completa de estoque;
gestão completa de oficina;
processamento de pagamentos diretamente pela plataforma.

Essas funcionalidades poderão ser avaliadas posteriormente como possíveis evoluções do produto.

## 9. Indicadores de Sucesso

A efetividade da solução poderá ser acompanhada por indicadores como:

**Operacionais**

tempo médio entre comunicação e registro do sinistro;
tempo médio de tratamento;
quantidade de sinistros em aberto;
quantidade de sinistros encerrados;
quantidade de sinistros pendentes;
percentual de sinistros tratados dentro do prazo;
quantidade de atividades pendentes.

**Orçamentários**

tempo médio para geração do orçamento;
quantidade de orçamentos aprovados;
quantidade de orçamentos rejeitados;
valor total dos orçamentos;
diferença entre valor orçado e valor realizado.

**Financeiros**

valor total a cobrar;
valor cobrado;
valor recebido;
valor pendente;
tempo médio de recebimento;
quantidade de cobranças em atraso.

**Qualidade do processo**

percentual de sinistros com documentação completa;
quantidade de retrabalhos;
quantidade de ocorrências sem responsável;
quantidade de sinistros sem atualização dentro do prazo definido.

## 10. Hipóteses

As seguintes hipóteses serão utilizadas inicialmente e deverão ser validadas durante as etapas de entrevistas e elicitação.

H1 — Centralização

A centralização das informações em uma única plataforma reduzirá a dispersão de dados relacionados aos sinistros.

H2 — Rastreabilidade

O registro do histórico de movimentações permitirá identificar quem realizou cada atividade e quando ela ocorreu.

H3 — Controle de prazos

A utilização de status, responsáveis e atividades pendentes permitirá melhorar o acompanhamento dos prazos de tratamento.

H4 — Orçamentos

A centralização dos orçamentos permitirá melhorar o controle dos valores previstos e realizados.

H5 — Cobrança

A integração do processo de cobrança ao fluxo do sinistro permitirá melhorar o acompanhamento dos valores devidos pelos clientes.

H6 — Visibilidade gerencial

A disponibilidade de indicadores permitirá aos gestores acompanhar o volume, situação, custos e desempenho dos sinistros.

H7 — Padronização

A utilização de um fluxo estruturado permitirá reduzir variações no processo de tratamento dos sinistros.
