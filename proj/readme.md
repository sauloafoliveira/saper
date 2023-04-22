# Projetos 

Aqui, vocês encontrarão o calendário de entregas. As entregas pelo calendário comporão muitas das notas de vocês. Abaixo, existe

## Calendário de entregas

> ``24/04`` Kick-off projeto final;
> - [ ] Criar um repositório **privado** da equipe;
> - [ ] Adicionar a mim ```@sauloafoliveira``` como membro do projeto;
> - [ ] Buscar formar equipes entre 04-05 colegas;
> - [ ] Commitar um readme.me com a escolha dos membros do projeto.

> ``03/05`` Seleção dos projetos;
> - [ ] Escolha do tema do projeto.

> ``18/05`` Definições da camada de Modelos;
> - [ ] Diagrama de Classes;
> - [ ] Diagrama de Entidade-Relacional;
> - [ ] Script SQL de criação do banco de dados do projeto.

> ``05/06`` Definições da camada de Visão;
> - [ ]  Protótipo de telas com base nos requisitos;
> - [ ]  Definição da identidade visual.

> ``14/06`` Definições da camada de Controle;
> - [ ]  Integração com Banco de dados;
> - [ ] (CRUD básico das entidades;

> ``29/06`` Definições da camada de Visão & Controle;
> - [ ] Integração front & back;

> ``30/06`` à ``04/07``Acompanhamento de projeto;

> ``05/07`` Ensaio Pitch;

> ``06/07`` Apresentação final.


# Lista de Projetos

## Sistema de Almoxarifado Hospitalar

O sistema para hospitais permite que sua equipe tenha total controle dos recursos e materiais utilizados em procedimentos médicos. A ideia é   digitalizar um processo comumente manual, cujo controle se dá por planilhas dispersas no sistema de uma operadora de saúde.

O Almoxarifado pode ser conceituado como sendo o local destinado à guarda e conservação de materiais, em recinto coberto ou não, adequado à sua natureza, tendo a função de destinar espaços onde permanecerá cada item aguardando a necessidade do seu uso, ficando sua localização e disposição interna acondicionados à política geral de estoques. O responsável pelo Almoxarifado deve possuir alto grau de honestidade, lealdade, confiança e disciplina.

### Requisitos

- [ ] O sistema deverá manter (cadastrar, alterar, buscar) as informações de materiais;
- [ ] O sistema deverá manter (entrada, saída e consulta de materiais) o almoxarifado;
- [ ] O sistema deverá gerar relatórios de vendas realizadas, materiais com baixo estoque (até 05 unidades) e materiais em falta;
- [ ] O sistema deverá manter (cadastrar, alterar, buscar) informações de funcionários;
- [ ] O sistema deverá manter (cadastrar, alterar, buscar) informações de fornecedores.

### Informações adicionais

Em relação aos materiais, devem ser guardadas as seguintes informações:  ``nome``, ``código de barras``, ``valor de compra``,  ``fornecedor``,  ``mínima``, ``fabricante`` e ``descrição`` como obrigatórias. Já em relação aos funcionários devem ser guardadas as seguintes informações: ``matrícula``, ``nome``, ``endereço``, ``telefone``, ``CPF``, ``data de nascimento``,  a ``situação`` (``ativo`` ou ``inativo``), ``e- mail``, ``cargo``, ``login`` e ``senha``. Sendo todas elas obrigatórias. Por fim, em relação aos fornecedores, devem ser guardadas as seguintes informações: ``matrícula``, ``nome fantasia``, ``endereço``, ``telefone``, ``CNPJ``, ``tempo de entrega`` e ``e-mail``. Sendo todas elas obrigatórias.

Ambos relatórios de entrada e de saída deverão ser gerados a partir da indicação de uma data inicial a uma data final. 

No estoque, deverão ser mostradas as seguintes  informações: o nome do material, sua quantidade em estoque, seu fabricante e seu fornecedor. 

Em relação às novas compras de materiais, deverão ser guardadas as seguintes informações: um código de identificação dessa demanda, o funcionário que a realizou, o(s) produto(s) solicitados(s), data da demanda, o valor total da compra, sua forma de pagamento e sua situação (ativa ou cancelada).

Os funcionário poderam realizar baixas no Almoxarido, isto é, demandar materiais para serem utilizados pelo hospital. Uma vez que essa demanda for atendida, atualiza-se a quantidade de elementos no almoxarifado.

## Sistema de Marcação de Consultas

Trata-se de um sistema web para auxiliar médicos e recepcionistas de uma clínica médica no processo de atendimento e gerenciamento de filas de espera. As agendas dos médicos seriam configuradas de acordo com os dias e horários de atendimentos de cada um, bem como a quantidade máxima de consultas permitidas. Já na recepção o sistema auxiliaria os atendentes a identificar a consulta de um paciente marcada previamente e na inserção de novos pacientes na fila de atendimento sem marcação prévia de uma consulta.


O sistema deve ser capaz de exibir para os médicos a sua lista de atendimento do dia, mostrando, de forma clara, quantos pacientes constam em sua lista e se sua chegada a clinica já foi confirmada, ou não. Os médicos poderiam visualizar, de qualquer lugar, como esta sua agenda de atendimentos para o dia. Para iniciar um atendimento, podem chamar o próximo paciente através do clique em um botão do sistema. Para registrar o atendimento os médicos informaram qual o diagnostico da consulta e o receituário informado. Apos a confirmação do registro da consulta, estas informações serão enviadas para o email do paciente.

### Requisitos 

- [ ] Cadastro de médico;
- [ ] Cadastro de pacientes;
- [ ] Configurar agenda de atendimento de médico;
- [ ] Marcar consulta;
- [ ] Confirmar presença;
- [ ] Confirmar autorização do plano de saúde;
- [ ] Registrar consulta;
- [ ] Visualizar protuário;
- [ ] Gerenciar fila de atendimento.

## Sistema de Controle e reserva de leitos

A gestão de leitos é um assunto muito importante para um hospital ou clínica,  pois através da visualização e monitoramento constante do uso das camas, ou seja, os leitos ocupados, disponíveis, reservados, em limpeza, dentre outros, pode-se combater a ociosidade dos leitos ao aprimorar o planejamento para o seu uso.


### Requisitos

- [ ] Cadastro de pacientes;
- [ ] Cadastro de leitos;
- [ ] Visão geral dos leitos;
- [ ] Dar alta a um paciente;

Ao se cadastrar um paciente e informar dados pesssoais (``número do prontuário``, ``nome do paciente,`` ``idade``, ``especiliadade``, ``data de internação``), os dados acerca da sua permanência, classificação Fugulin e Origem precisam ser informados. Estes dados estão listados conforme categorias abaixo:

| Motivo da permanência          | Classificaçnao de Fugulin    | Origem             |
| :----------------------------- | :--------------------------- | :----------------- |
| Leito de enfermaria            | Cuidados mínimos             | SAMU               |
| Leito de terapia intensiva     | Cuidados intermediários      | Demanda Espontânea |
| Parecer de outra especialidade | Cuidados de alta dependência |                    |
| Transferência externa          | Cuidados semi-intensivos     |                    |
| Social                         | Cuidados intensivos          |                    |
| Hemodiálise                    |                              |                    |
| Outros (descrever)             |                              |                    |

Na visualização dos leitos, cores de acordo com o tempo de perman6encia do paciente devem seguir as seguintes características:

| Verde                                   | Amarela                              | Vermelha   |
| --------------------------------------- | ------------------------------------ | ---------- |
| Se tempo de permanência for ≤ 24 horas. | Permanência > 24 horas e ≤ 72 horas. | ≥ 72 horas |

