# Como obter mensagens do MQ por um CorrelId ou MsgId

### O IBM MQ permite obter mensagens atráves de um Id de correlação, CorrelId, este parâmetro deve ser definido no Header de uma mensagem e atráves dele deve ser feita a consulta no MQ para obter uma mensagem especifica em uma fila de resposta.

### Para fazer esta consulta, o backend precisa receber uma mensagem e fazer um PUT em uma fila, com isto, o Datapower poderá ir até esta fila e realizar um GET desta mensagem especifica.

### Para fazer este exemplo será utilizado um serviço do tipo Multi-protocol Gateway

## Pré-requisitos

- Criar um serviço MPG
- Ter um IBM Queue Manager configurado
- Ter um MQ como backend

