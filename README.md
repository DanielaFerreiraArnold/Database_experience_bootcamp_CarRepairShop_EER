# database_experience_bootcamp_CarRepairShop


Digital Innovation One Bootcamp: DATABASE EXPERIENCE

## Objetivo:
Criar o esquema conceitual para o contexto de oficina com base na narrativa fornecida

## Narrativa
* Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica
* Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões  periódicas
* Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma OS com data de entrega.
* A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra
* O valor de cada peça também irá compor a OSO cliente autoriza a execução dos serviços
* A mesma equipe avalia e executa os serviços
* Os mecânicos possuem código, nome, endereço e especialidade
* Cada OS possui: n°, data de emissão, um valor, status e uma data para conclusão dos trabalhos.
* Os mecânicos possuem código, nome, endereço e especialidade
* Cada OS possui: n°, data de emissão, um valor, status e uma data para conclusão dos trabalhos.

## Objective:

To create a coneptual schema for management and control of a car repair shop following the narrative bellow.

## Narrative:
Note: the version in English contains extra information I added to make it more clear for ther readers to understand the EER.

* Clients take their cars in for repair or maintnance.

* A client has a name, an address, an identification number, a telephone number, an email address, a work phone number, and the place of work.

* A car inherits the clientformation..

* One client can have one or more cars.

* Each car is designated to a team of mechanics. 

* Each team has more than one mechanic.

* Each mechanic has a name, a specialty, a code and an address.

* One team can receive one or more cars.

* The team will analyse and fill out a service order, so the team has a service order.

* The service order contains a numer, a date, the designated price for the repair, status, and a deadline. 

* One team also has information about servece prices and car part prices, which they will use to feed the service order.
Many teams will have access to the same one database.

* There is only one database.

* One team can be responsible for more than one service order, but one service order can only come from one team.

* The client has access to the service order and the payment methods, which he/she will aprove or not.
If he/she aproves, one or more payment methods can be chosen by one client.

* Different payment methodos can be used by different clients.

* Payment methods can be payment by cash, debid card, credit card, or bank transfer.

Side note:

Client is stated as a strong entity, but it could be a weak one too, once if there is no car, there is no client.
