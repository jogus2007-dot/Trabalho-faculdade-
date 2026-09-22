
PROJETO DE MODELAGEM DE BANCO DE DADOS
Corretora de Seguros — Bradesco

Integrantes
Nome	RGM
Mateus Martins Gonçalves	47812222
Raul Borges Sim	48247634
João Gustavo Bento de Souza	42283671
1. Caracterização da Organização
1.1 Nome e natureza da organização

A organização escolhida para o desenvolvimento deste projeto é uma corretora de seguros que atua junto ao Bradesco, identificada durante a visita como Bradesco.

A corretora atua no segmento de seguros, trabalhando com diferentes modalidades de produtos, como:

Seguro Auto
Seguro Residencial
Seguro Empresarial
Seguro de Vida
Seguro Saúde
Seguro Dental
Outros tipos de seguros disponibilizados pelas companhias parceiras

A organização possui fins lucrativos e está em funcionamento desde 2016.

1.2 Contexto e porte

Atualmente, a organização conta com aproximadamente 6 funcionários.

De acordo com as informações obtidas durante a pesquisa de campo:

Funcionários: aproximadamente 6
Clientes atendidos por mês: aproximadamente 50 a 100
Seguros comercializados por mês: aproximadamente 50 a 60
Faturamento médio mensal: aproximadamente R$ 60.000,00

Entre as principais atividades realizadas estão:

Cadastro de clientes
Atendimento
Elaboração de cotações
Acompanhamento de propostas
Contratação de seguros
Controle de apólices
Controle de parcelas e pagamentos
Atendimento de sinistros
Renovação de apólices
2. Problemas e Necessidades Identificados

Durante a pesquisa de campo, foi observado que grande parte das informações operacionais é controlada por meio de Excel e Google Planilhas.

As cotações, propostas, pagamentos, parcelas e atendimentos são acompanhados por planilhas.

Em determinadas situações, durante visitas aos clientes, as informações são inicialmente registradas em folhas de papel e posteriormente transferidas para os controles digitais.

A organização também utiliza um quadro de vidro para organizar as visitas previstas para a semana.

O acompanhamento dos sinistros é realizado por uma funcionária especializada, responsável pelas listagens e pelo acompanhamento dos casos.

As renovações são acompanhadas por Excel e Google Planilhas, além de informações disponibilizadas pela sucursal para identificar apólices próximas do vencimento.

Principais problemas
Informações distribuídas entre diferentes planilhas
Dependência de controles manuais
Utilização de papel durante determinados atendimentos
Necessidade de atualização manual das informações
Controle visual das visitas
Dificuldade de centralização do histórico dos clientes
Controle manual de parcelas e pagamentos
Necessidade de acompanhamento dos vencimentos
Controle das renovações por diferentes ferramentas
Informações de sinistros concentradas em controles específicos
Solução proposta

Diante desse cenário, o projeto propõe a criação de um banco de dados capaz de centralizar e organizar as principais informações da corretora.

3. Dados da Organização
Informação	Dado
Nome informado	Bradesco
Segmento	Corretora de seguros
Início das atividades	2016
Quantidade de funcionários	6
Endereço	Rua Rego Barros, 570
E-mail informado	alicelimna@gmail.com
Responsável entrevistada	Patrícia dos Santos Souza
Cargo	Sócia
Google Maps / Site / Rede Social	Não informado
4. Processos de Negócio
4.1 Cadastro de Clientes

O cadastro é realizado quando um cliente entra em contato com a corretora.

Informações principais
CPF
Nome
Data de nascimento

Essas informações são utilizadas para identificar o cliente e relacioná-lo aos demais processos da corretora.

4.2 Cotação

Após o levantamento das necessidades do cliente, a corretora realiza uma ou mais cotações.

A organização trabalha com diferentes tipos de seguros e consulta diversas seguradoras.

A Bradesco Seguros é priorizada nas cotações. Quando não é encontrada uma condição adequada, outras companhias são consultadas.

Fluxo

Cliente → Levantamento das necessidades → Cotação → Análise das opções → Escolha da opção

4.3 Proposta

Após a realização da cotação, caso o cliente tenha interesse em prosseguir, é elaborada uma proposta.

A proposta representa a etapa entre a cotação e a contratação efetiva do seguro.

Fluxo

Cotação → Análise do cliente → Aceite → Proposta

Caso o cliente não prossiga, a cotação permanece registrada e não necessariamente resulta em uma apólice.

4.4 Contratação e Apólice

Quando a contratação é efetivada, é gerada uma apólice.

Principais informações
Número da apólice
Data de início da vigência
Data de término da vigência
Status
Fluxo

Proposta → Contratação → Apólice → Controle da vigência

4.5 Controle de Parcelas e Pagamentos

A corretora acompanha os pagamentos e parcelas por meio de Excel e Google Planilhas.

O banco de dados deverá permitir relacionar cada parcela à sua respectiva apólice e registrar a situação do pagamento.

Fluxo

Apólice → Parcelas → Vencimento → Pagamento → Atualização do status

4.6 Atendimento ao Cliente

Os atendimentos são registrados nas planilhas de acompanhamento.

Durante as visitas, os dados podem ser inicialmente registrados em papel e posteriormente transferidos para os controles digitais.

Fluxo

Cliente → Atendimento/Visita → Levantamento de informações → Registro → Atualização

4.7 Sinistros

O processo de sinistros possui tratamento específico dentro da organização.

Uma funcionária é responsável pelo acompanhamento dos sinistros e pelas listagens relacionadas a eles.

O banco de dados deverá permitir relacionar cada sinistro ao cliente e à respectiva apólice.

Fluxo

Cliente → Comunicação do sinistro → Registro → Acompanhamento → Atualização da situação

4.8 Renovação

As renovações são acompanhadas por Excel e Google Planilhas.

A corretora também utiliza informações disponibilizadas pela sucursal para identificar seguros próximos do vencimento.

Quando uma apólice se aproxima do vencimento, a corretora entra em contato com o cliente para tratar da renovação.

Fluxo

Apólice → Verificação do vencimento → Contato com cliente → Renovação ou encerramento

5. Requisitos do Sistema
5.1 Requisitos Funcionais
Código	Requisito
RF01	Permitir cadastrar clientes
RF02	Permitir consultar clientes
RF03	Permitir atualizar dados dos clientes
RF04	Permitir cadastrar tipos de seguros
RF05	Permitir cadastrar seguradoras
RF06	Permitir registrar cotações
RF07	Relacionar uma cotação a um cliente
RF08	Relacionar uma cotação a uma seguradora
RF09	Permitir registrar propostas
RF10	Permitir acompanhar o status das propostas
RF11	Permitir registrar apólices
RF12	Registrar número e vigência da apólice
RF13	Permitir cadastrar parcelas
RF14	Permitir registrar pagamentos
RF15	Consultar parcelas pendentes e pagas
RF16	Permitir registrar atendimentos
RF17	Permitir registrar sinistros
RF18	Permitir acompanhar o status dos sinistros
RF19	Identificar apólices próximas do vencimento
RF20	Permitir registrar renovações
RF21	Manter o histórico do cliente
RF22	Pesquisar informações por cliente, apólice, seguradora ou situação
5.2 Requisitos Não Funcionais
Código	Requisito
RNF01	Possuir interface simples e intuitiva
RNF02	Proteger o acesso às informações por autenticação
RNF03	Restringir o acesso conforme o perfil do usuário
RNF04	Apresentar bom desempenho nas consultas
RNF05	Preservar a integridade dos dados
RNF06	Permitir realização de backups periódicos
RNF07	Evitar duplicidade de clientes
RNF08	Permitir inclusão de novos tipos de seguros
RNF09	Permitir inclusão de novas seguradoras
RNF10	Preservar a confidencialidade dos dados pessoais
6. Regras de Negócio
Código	Regra
RN01	Cada cliente deve possuir CPF, nome e data de nascimento
RN02	O CPF deve identificar unicamente um cliente
RN03	A corretora trabalha com diferentes tipos de seguros
RN04	Uma cotação deve estar associada a um cliente
RN05	Uma cotação deve estar associada a uma seguradora
RN06	A Bradesco Seguros é priorizada nas cotações
RN07	Outras seguradoras podem ser consultadas quando necessário
RN08	Uma proposta pode ser originada a partir de uma cotação
RN09	Nem toda cotação necessariamente resulta em uma proposta
RN10	Uma apólice deve possuir número e período de vigência
RN11	A data inicial da vigência deve ser anterior à data final
RN12	Uma apólice pode possuir várias parcelas
RN13	Uma parcela deve estar vinculada a uma apólice
RN14	Um pagamento deve estar relacionado a uma parcela
RN15	Um sinistro deve estar relacionado a uma apólice
RN16	Os sinistros possuem acompanhamento específico
RN17	Os atendimentos devem estar relacionados aos clientes
RN18	As apólices devem ser acompanhadas quanto ao vencimento
RN19	Uma apólice pode entrar em processo de renovação
RN20	As informações dos clientes devem ser protegidas contra acesso não autorizado
7. Entidades do Banco de Dados

Foram identificadas as seguintes entidades:

Cliente
Seguradora
TipoSeguro
Cotação
Proposta
Apólice
Parcela
Pagamento
Atendimento
Sinistro
Renovação
8. Dicionário de Dados
8.1 Cliente
Atributo	Descrição	Regra
id_cliente	Identificador interno	Único e obrigatório
cpf	CPF do cliente	Obrigatório e único
nome	Nome do cliente	Obrigatório
data_nascimento	Data de nascimento	Obrigatória
8.2 Seguradora
Atributo	Descrição	Regra
id_seguradora	Identificador da seguradora	Único
nome	Nome da seguradora	Obrigatório
prioridade	Indica prioridade comercial	Pode indicar seguradora priorizada
8.3 TipoSeguro
Atributo	Descrição	Regra
id_tipo_seguro	Identificador do tipo	Único
nome	Nome do seguro	Obrigatório
descricao	Descrição do produto	Opcional
8.4 Cotação
Atributo	Descrição	Regra
id_cotacao	Identificador da cotação	Único
data_cotacao	Data da cotação	Obrigatória
valor_cotado	Valor apresentado	Não negativo
status	Situação da cotação	Valores definidos
id_cliente	Cliente relacionado	Obrigatório
id_seguradora	Seguradora consultada	Obrigatório
id_tipo_seguro	Tipo de seguro	Obrigatório
8.5 Proposta
Atributo	Descrição	Regra
id_proposta	Identificador da proposta	Único
data_proposta	Data da proposta	Obrigatória
status	Situação da proposta	Valores definidos
valor_proposta	Valor da proposta	Não negativo
id_cotacao	Cotação de origem	Deve existir
8.6 Apólice
Atributo	Descrição	Regra
id_apolice	Identificador interno	Único
numero_apolice	Número da apólice	Obrigatório
inicio_vigencia	Início da vigência	Obrigatório
fim_vigencia	Fim da vigência	Obrigatório
status	Situação da apólice	Valores definidos
id_proposta	Proposta de origem	Deve existir
8.7 Parcela
Atributo	Descrição	Regra
id_parcela	Identificador da parcela	Único
numero_parcela	Número da parcela	Obrigatório
valor	Valor da parcela	Maior que zero
data_vencimento	Data de vencimento	Obrigatória
status	Situação da parcela	Obrigatório
id_apolice	Apólice relacionada	Obrigatório
8.8 Pagamento
Atributo	Descrição	Regra
id_pagamento	Identificador do pagamento	Único
data_pagamento	Data do pagamento	Obrigatória quando pago
valor_pago	Valor pago	Maior que zero
forma_pagamento	Forma utilizada	Valores definidos
id_parcela	Parcela relacionada	Obrigatório
8.9 Atendimento
Atributo	Descrição	Regra
id_atendimento	Identificador	Único
data_atendimento	Data do atendimento	Obrigatória
tipo_atendimento	Tipo do atendimento	Obrigatório
descricao	Informações do atendimento	Opcional
id_cliente	Cliente atendido	Obrigatório
8.10 Sinistro
Atributo	Descrição	Regra
id_sinistro	Identificador	Único
numero_sinistro	Número do sinistro	Quando fornecido, deve ser registrado
data_sinistro	Data da ocorrência	Obrigatória
descricao	Descrição da ocorrência	Obrigatória
status	Situação do sinistro	Valores definidos
id_apolice	Apólice relacionada	Obrigatório
8.11 Renovação
Atributo	Descrição	Regra
id_renovacao	Identificador	Único
data_contato	Data do contato com cliente	Registrada quando houver contato
data_renovacao	Data da renovação	Obrigatória quando concluída
status	Situação da renovação	Valores definidos
id_apolice	Apólice renovada	Obrigatório
9. Modelagem Conceitual
9.1 Relacionamentos

A estrutura proposta possui os seguintes relacionamentos:

Cliente → Cotação: 1
Seguradora → Cotação: 1
TipoSeguro → Cotação: 1
Cotação → Proposta: 1:0..1
Proposta → Apólice: 1:0..1
Apólice → Parcela: 1
Parcela → Pagamento: 1:0..1
Cliente → Atendimento: 1
Apólice → Sinistro: 1
Apólice → Renovação: 1
10. Diagrama Entidade-Relacionamento
CLIENTE
   │
   │ 1:N
   ▼
COTAÇÃO ───── N:1 ───── SEGURADORA
   │
   │ N:1
   ▼
TIPO_SEGURO

COTAÇÃO
   │
   │ 1:0..1
   ▼
PROPOSTA
   │
   │ 1:0..1
   ▼
APÓLICE
   │
   ├──────────── 1:N ────────────► PARCELA
   │                                  │
   │                                  │ 1:0..1
   │                                  ▼
   │                              PAGAMENTO
   │
   ├──────────── 1:N ────────────► SINISTRO
   │
   └──────────── 1:N ────────────► RENOVAÇÃO

CLIENTE
   │
   │ 1:N
   ▼
ATENDIMENTO

Observação: As cardinalidades apresentadas são uma proposta de modelagem baseada nas informações levantadas durante a pesquisa de campo e devem ser confirmadas com a responsável entrevistada antes da entrega definitiva.

11. Justificativa Técnica

A modelagem foi elaborada considerando os processos identificados durante a pesquisa de campo.

A entidade Cliente foi definida como uma das entidades centrais, pois as atividades de atendimento e contratação estão relacionadas aos clientes da corretora.

As entidades Cotação, Proposta e Apólice foram separadas para representar diferentes etapas do processo comercial.

A entidade Seguradora foi separada de TipoSeguro, pois representam informações diferentes: a seguradora corresponde à companhia responsável pelo produto, enquanto o tipo de seguro representa a modalidade comercializada.

A entidade Parcela foi separada de Apólice, pois uma apólice pode possuir diversas parcelas.

A entidade Pagamento permite registrar a situação financeira de cada parcela.

A entidade Atendimento representa o histórico de contatos realizados com os clientes.

A entidade Sinistro foi incluída devido à existência desse processo dentro da organização.

A entidade Renovação foi incluída devido à necessidade de acompanhar os vencimentos das apólices e manter o histórico das renovações.

12. Evidências da Pesquisa de Campo

A pesquisa de campo foi realizada presencialmente nas instalações da organização.

Foto 1 — Ambiente interno

Registro do ambiente interno da organização, com salas individuais e estrutura destinada à realização das atividades profissionais.

[Inserir Foto 1 aqui]

Foto 2 — Identificação da organização

Registro da identificação visual “Bradesco Empresas e Negócios” presente nas instalações visitadas.

[Inserir Foto 2 aqui]

13. Uso de Inteligência Artificial
Ferramenta utilizada

ChatGPT — OpenAI

Utilização

A ferramenta foi utilizada como apoio nas seguintes etapas:

Organização das informações da entrevista
Estruturação do README
Identificação preliminar das entidades
Elaboração dos requisitos
Organização das regras de negócio
Elaboração do dicionário de dados
Revisão da redação
Organização da proposta de modelagem
Motivação

A IA foi utilizada como ferramenta de apoio para transformar as informações coletadas durante a pesquisa de campo em uma estrutura organizada de documentação e modelagem de banco de dados.

As informações específicas sobre a corretora foram obtidas por meio da pesquisa de campo e entrevista realizada pelo grupo.

As sugestões da IA foram comparadas com as informações fornecidas pela organização para evitar a inclusão de processos inexistentes.

14. Conclusão

O projeto tem como objetivo propor uma estrutura de banco de dados capaz de centralizar, organizar e facilitar o gerenciamento das informações da corretora de seguros.

A modelagem contempla os principais processos identificados durante a pesquisa, incluindo:

Clientes
Seguradoras
Tipos de seguros
Cotações
Propostas
Apólices
Parcelas
Pagamentos
Atendimentos
Sinistros
Renovações
