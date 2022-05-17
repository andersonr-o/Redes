# Endereçamento IP
## O que é?
Endereços IPs servem, basicamente, para que as informações do usuário sejam enviados para o servidor, e vice-versa.<br>
Através desse endereço, o sevidor identifica o usuário e o usuário identifica o servidor. Sem isso, nenhuma conexão se torna possível (teoricamente IP 127).<br><br>
Os endereços IPs estão em quase todos os lugares da web, entender o seu funcionamento é primordial para quem deseja seguir na área. Além de ser bem comentado no meio hacking.
## Classes de IPs
Eles são divididos, pois cada classe atende a uma quantidade de IPs possíveis para o consumidor.
Há cinco classes de IPs existentes, sendo elas A, B, C, D e E.
### Classe A
Vai de 0 a 127, sendo capaz de suportar até 16.777.216 endereços IPs.
### Classe B
Vai de 128 a 191 e é capaz de suportar até 65.536 endereços IPs.
### Classe C
Vai de 192 a 223, sendo capaz de suportar até 256 endereços IPs. Geralmente é essa classe de IP que está na maioria dos domicílios, pois muitas vezes não há a necessidade de mais de 256 endereços IPs.
### Classe D
Vai de 224 a 239, é não é capaz de suportar endereços IPs.<br>
Como assim?<br>
Isso mesmo, a sua utilidade está em outro lugar. A classe D é reservada para serviços de Multicast.
### Classe E
Vai de 240 a 255 e também não suporta endereços IPs, mas é reservada para o teste de novas tecnologias. Atualmente, por exemplo, temos o 5G.
## Por que esses números?
Basicamente, um endereço IP como o vemos não é o verdadeiro endereço IP. Aquele número está compilado, pois ele estendido é formado por quatro octetos binários.<br>
Um endereço IP provável da sua casa: 192.168.0.1<br>
O mesmo endereço IP descompilado: 1100 0000 // 1010 1000 // 0000 0000 // 0000 0001<br>
## Como saber a classe do meu IP?
Basta olhar para os três primeiros números do seu endereço IP e ver a qual classe ele pertence.

## Endereços de rede e endereços de host
Cada número dentro dos octetos de um endereço IP significa 1 bit. 4 octetos x 8 espaços = 32 espaços.<br><br>
Cada espaço pode ser ocupado por dois números (0 e 1), e ao menos um octeto será reservado para a rede, dependendo de sua classe. Portanto:
Se o IP for de classe A, o primeiro octeto será reservado para a rede. Se for de classe B, os dois primeiros octetos serão reservados para a rede. Se for de classe C, os três primeiros octetos serão reservados para a rede. O restante fica para os hosts.<br><br>
Quanto mais endereços de hosts e menos endereços de redes, mais dispositivos poderão se conectar.

Classe A - 2^24 = 16.777.216
Ou
10.255.255.255, isto é, 256<sup>3</sup> possiblidades = 16.777.216<br>
*256 porque o 0 conta também. De 0 a 255, temos 256 números.*<br><br>

Classe B - 2^16 = 65.536
Ou
172.16.255.255 &rightarrow; 256<sup>2</sup><br><br>

Classe C - 2^8 = 256
Ou
192.168.0.255, ou seja, 256<sup>1</sup> possibilidades (o que significa 256 mesmo).<br><br>
Exemplo de endereço classe A: 10.xxx.xxx.xxx<br><br>
Exemplo de endereço classe B: 172.16.xxx.xxx<br><br>
Exemplo de endereço classe C: 192.168.0.xxx<br><br>
Aonde os números representam os endereços de rede e os "x" representam os endereços de hosts.

<!--## Como calcular um endereço IP?-->
