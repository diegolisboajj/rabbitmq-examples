# RabbitMQSpring


Conteúdo
---------

A raiz contem uma arquivo denominado docker-compose.yml. Portanto, este arquivo não faz parte do projeto Java Spring. Mova-o para a uma pasta dedicada 
ao docker-compose. Continuando ... Este arquivo, possui as configurações utilizadas para criar o container com imagem 
RabbitMQ. Dessa formal, foram setados alguns parâmetros como: restart com sistema do host, mapeamento de dados entre host e container, imagem 
utilizada do docker hub.

Caso você ainda não conhece os conceitos de virtualização e as vantagens do docker, 
acesse esse artigo com a descrição toda dessa ferramenta. Link: https://simplificandoredes.com/docker-instalacao/.

Os exemplos estão organizados como segue:

demo - exemplo simplificado de troca de mensagens em sistema de filas "puro";
Work Queue - simulando processamento decorrente de mensagens com payload "pesado" (ex:simulando imagens);
Pub/Sub - comunicação utilizando a intermediação da exchange do tipo fanout;
Routing - defindo labels através da routing key;
Topic - utilizando exchange do tipo topic na comunicação;
PubConfirmation - utilizando confirmação de envio de mensagens do produtor à exchange;
DLX - Criando e utilizando uma Dead Letter Exchange para mensagens com TTL expirado.
