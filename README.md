# Netstat analise e monitoramento de rede

O **netstat** é um recursos que mostra conexões de rede, tabelas de roteador, estatiscas de interfaces e conexões mascaradas.

É um recurso que pode nos ajudar na analise de informações e saber como podemos descobrir alguma conexão maliciosa e se possivel mascarada em nossa maquina ou tentando se conectar!

Exemplo 1: netstat -n

Mostra todas as conexões referente ao que está acontecendo agora!

Temos varias informações (ips, conexões estabelecidas, protocolo, tipo da conexão, porta, caminha que está fazendo...)

![image](https://user-images.githubusercontent.com/33209944/210158517-c8ee4a6a-92ca-4c51-b0ee-74b9abac4761.png)

O **netstat** nos mostra muitas conexões que nós permmite ter condições de analisar nosso trafego de rede.

Vamos analisar algumas flags:

netstat -a: Nós mostra conexões ativas e estabelecidas em nossa maquina, principalmente conexões TCP, UDP ou RAW!

![image](https://user-images.githubusercontent.com/33209944/210158624-e60acac4-11a5-4c3a-9256-298bfba7fd04.png)

netstat -at: Mostra todas as conexões TCP

![image](https://user-images.githubusercontent.com/33209944/210158647-acb72fa9-c781-470e-b473-698d50e9110f.png)

netstat -au: Mostra todas a conexões UDP

![image](https://user-images.githubusercontent.com/33209944/210158655-36232806-968c-4fb2-8383-059d8726b5bf.png)

netstat -aw: Mostra algumas conexão RAW. 

![image](https://user-images.githubusercontent.com/33209944/210158709-781c5fd0-4545-4e60-8f39-8466dc7baae3.png)

netstat -ax: Mostra todas as conexões sockets estabelecidas.

![image](https://user-images.githubusercontent.com/33209944/210158743-4403148f-9a2c-47e8-819a-03b75c7be532.png)

netstat -aut: Podemos mesclar as flags...

![image](https://user-images.githubusercontent.com/33209944/210158756-6e4d7cb3-99fa-4111-aeec-a1b10c1f6376.png)

netstat -an: A flag **n** não resolve consulta DNS.

