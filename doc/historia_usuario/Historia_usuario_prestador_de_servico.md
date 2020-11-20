### **História: Prestador de serviço recebe agendamentos realizados por seus clientes**

**Como um(a)**  prestador de serviço

**Quero** receber os agendamentos realizados por meus clientes sem que eu perca tempo na mediação do processo

**Para** que eu não perca serviço por falta de retorno aos mesmos, assim como garantir um bom atendimento no momento da visita sem interrupções para intermediar novos agendamentos.

__


## CENÁRIOS

**Cenário 1: Prestador de serviço recebe e-mail para confirmar agendamento**

**Dado que** a agenda utiliza a navegação para executar a marcação em tempo real 

**Quando**   o cliente conclui e envia a solicitação de agendamento

**Então**    o prestador recebe um e-mail para confirmar o agendamento

__

**Cenário 2: Prestador de serviço responde confirmação de agendamento "ACEITAR"**

**Dado que**  o prestador de serviço visualiza seu email com a notificação para confirmar o agendamento, assim como os dados do mesmo

**Quando**   clicar na opção "Aceitar"

**Então**    o horário na agenda altera de status de reservado (cor amarela) para ocupado (cor vermelha).

**E**       o cliente recebe um e-mail atualizando o status, assim como na opção desejada para confirmação escolhida no momento do agendamento.

__

**Cenário 3: Prestador de serviço responde confirmação de agendamento "RECUSAR"**

**Dado que**  o prestador de serviço visualiza seu email com a notificação para confirmar o agendamento, assim como os dados do mesmo

**Quando**   clicar na opção "Recusar"

**Então**   o horário na agenda altera de status de reservado (cor amarela) para disponível (cor branca).

**E**       o cliente recebe um e-mail atualizando o status, assim como na opção desejada para confirmação escolhida no momento do agendamento.

__

**Cenário 4: Prestador de serviço responde confirmação de agendamento mas precisa realizar ajustes antes de definir status"**

**Dado que** o prestador de serviço visualiza seu email com a notificação para confirmar o agendamento, assim como os dados do mesmo

**Quando**   confere os dados 

**E**        percebe que precisa de ajustes ou mais informações

**Então**    o profissional terá de recusar para que seu cliente possa realizar novo agendamento.

__

**Cenário 5: Mensagem de atualização de status "ACEITAR"**

**Dado que** o prestador de serviço responde a confirmação de agendamento

**Quando**   clicar em "ACEITAR"

**Então**    uma mesagem padrão será enviada ao seu cliente por e-mail "Seu horário foi confirmado "data e horário", obrigado!"

__

**Cenário 6: Mensagem de atualização de status "RECUSAR"**

**Dado que** o prestador de serviço responde a confirmação de agendamento

**Quando**   clicar em "RECUSAR"

**Então**    uma mesagem padrão será enviada ao seu cliente por e-mail "Seu horário foi resusado "data e horário". Motivo: "mensagem dada pelo prestador"

__

**Cenário 7: Agendamento realizado com opção de confirmação por "TELEFONE"**

**Dado que** o sistema envia a confirmação por padrão via e-mail

**Quando**  o prestador visualiza a opção de confirmação por "TELEFONE" 

**E**    clicar nas opções disponíveis de retorno

**Então**  o prestador de serviço deverá incluir essa tarefa manualmente

___

**Cenário 8: Agendamento realizado com opção de confirmação por "WHATSAPP"**

**Dado que** o sistema envia a confirmação por padrão via e-mail

**Quando**  o prestador visualiza a opção de confirmação por "WHATSAPP" 

**E**    clicar nas opções disponíveis de retorno

**Então**  o prestador de serviço deverá incluir essa tarefa manualmente

__
