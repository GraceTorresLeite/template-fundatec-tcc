## Mapeamento das Personas
 - Consumidor: Cliente que irá consumir os serviços
 
 - Prestador de Serviço: Quem irá executar os serviços e que se deslocará ao local indicado pelo cliente.
 
## História de Usuário - _três aspectos críticos ( 3Cs)_

### **História 1: Cliente envia seu horário e serviço desejados ao seu prestador de serviço**

**Como um(a)**  cliente

**Quero** acesso rápido e fácil para o serviço no qual desejo contratar

**Para** garantir meu horário no momento que lembro da necessidade, de forma ágil e em tempo real, independente de um contato direto com o profissional

__


## CENÁRIOS

**Cenário 1: Cliente com conexão na internet**

**Dado que** a agenda utiliza a navegação para executar a marcação em tempo real 

**Quando**   o cliente possui o serviço de dados ou wifi habilitado em seu dispositivo móvel ou desktop/notebook

**Então**    pelo navegador de sua preferência digitará a URL da Schedule Beauty 

**E**        após carregar a página terá acesso ao site com as abas de (HOME, SERVIÇOS E VALORES, AGENDE SEU HORÁRIO)

__

**Cenário 2: Agendamento conectado na internet primeiro acesso do cliente**

**Dado que**  os atendimentos possuem flexibilidade de endereço, o mesmo será informado no momento de cada agendamento

**Quando**   o cliente navegar pelo site não haverá solicitação de cadastro para habilitar formulário de agendamento

**Então**    o cliente terá livre acesso a todas as páginas do site

__

**Cenário 3: Agendamento desconectado da internet**

**Dado que** a agenda utiliza a navegação para executar a marcação em tempo real  

**Quando**   o cliente estiver com os serivços de dados ou wifi desabilitados ou indisponíveis

**Então**   mesmo que a página carregue devido a mémoria cache do navegador, o formulário de agedamento não será completado o envio

**E**       uma tela retornará com a notificação padrão de seu navegador quanto a falta de conexão

__

**Cenário 4: Cliente preenchendo formulário de agendamento com campos nulos**

**Dado que** Todos os campos do formulário contidos na aba "AGENDE SEU HORÁRIO" são obrigatórios. Exceto(Complemento,Mensagem)

**Quando**   um ou mais campos não forem informados

**E**        clicado no botão "ENVIAR"

**Então**    o sistema apontará no campo expecífico uma caixa de diálogo com a seguinte mensagem "Preencha este campo.", e semelhantemente para cada campo subsequente

__

**Cenário 5: Cliente preenchendo formulário de agendamento com o campo e-mail inválido**

**Dado que** o cliente digite no formulário um e-mail sem o "@"

**Quando**   clicar em "ENVIAR" o formulário de agendamento

**Então**    uma caixa de diálogo apontando para o devido campo surgirá informando:"Inclua um "@" no endereço de e-mail. "email_digitado.com" está com um "@" faltando. 

__

**Cenário 6: Cliente preenchendo formulário de agendamento com o campo cep inválido**

**Dado que** o cliente digite números (faltantes, a mais que o esperado ou que não contenha na base de dados da API utilizada) 

**Quando**   clicar em "ENVIAR" o formulário de agendamento

**Então**    um alerta será emitido pelo sistema com a seguinte mensagem "CEP não encontrado. + botão [OK]"

__

**Cenário 7: Agendamento realizado com sucesso**

**Dado que** cliente está com internet e com o acesso do site em seu navegador 

**Quando**   preenchido os dados como: Nome, Telefone, E-mail, Endereço, Serviço, Dia e Horário;

**E**    clicar em "Enviar"

**Então**  Uma mensagem aparecerá para que aguarde a confirmação do prestador de serviço e seu horário ficará temporariamente reservado(cor Amarela). Se o cliente não informou a opção de confirmação, o e-mail será a opção padrão.

__

### **História 2: [Prestador de serviço recebe agendamentos realizados por seus clientes](/doc/historia_usuario/Historia_usuario_prestador_de_servico.md)**
