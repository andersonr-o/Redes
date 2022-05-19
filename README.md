# Endereçamento IP
## O que é?
Endereços IPs servem, basicamente, para que as informações do usuário sejam enviados para o servidor, e vice-versa.<br><br>
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
Como assim? <br>
Isso mesmo, a sua utilidade está em outro lugar. A classe D é reservada para serviços de Multicast.
### Classe E
Vai de 240 a 255 e também não suporta endereços IPs, mas é reservada para o teste de novas tecnologias. Atualmente, por exemplo, temos o 5G.
## Como saber a classe do meu IP?
Basta olhar para os três primeiros números do seu endereço IP e ver a qual classe ele pertence.

## Endereços de rede e endereços de host
Cada número dentro dos octetos de um endereço IP significa 1 bit. 4 octetos x 8 espaços = 32 espaços.<br><br>
Cada espaço pode ser ocupado por dois números (0 e 1), e ao menos um octeto será reservado para a rede, dependendo de sua classe.<br><br>
Portanto, se o IP for de classe A, o primeiro octeto será reservado para a rede. Se for de classe B, os dois primeiros octetos serão reservados para a rede. Se for de classe C, os três primeiros octetos serão reservados para a rede.<br>
O restante fica para os hosts.<br><br>
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

## Por que esses números?
Basicamente, um endereço IP como o vemos não é o verdadeiro endereço IP. Aquele número está compilado, pois ele estendido é formado por quatro octetos binários.<br><br>
Um endereço IP provável da sua casa: 192.168.0.1<br>
O mesmo endereço IP descompilado: 1100 0000 // 1010 1000 // 0000 0000 // 0000 0001<br>

## Como calcular um endereço IP?
É algo simples até, basta seguir uma tabela.<br>
Temos 8 números dentro de um octeto, onde o primeiro é 1 e o último é 128.<br>
O primeiro é 128, o segundo é 64, o terceiro é 32, o quarto é 16, o quinto é 8, o sexto é 4, o sétimo é 2 e o último é 1.
### Foto demonstrativa:<br>
![tabela-dos-ips-600](https://user-images.githubusercontent.com/97858145/161392982-0db4aec2-b5f6-4cb1-b319-a517bbf88046.jpg)<br>
**Desafio:**<br>
Tente calcular o número dessa tabela acima.

### Exemplo:
Peguemos o 192.168.0.1 da seção "Por que esses números?".<br>
192 &rightarrow; 1100 0000. Ou seja, o primeiro (128) + o segundo (64) = 192.<br>
Como os outros estão com 0, não tem como contá-los.

#### Exemplo em foto:
![tabela-ip](https://user-images.githubusercontent.com/97858145/161392851-e508bd51-132c-4a54-93a2-87133d130509.png)

## Blacklist IPs
Na realidade, os IPs que constam em blacklists são fonte provável de spam. Mas isso também pode ocorrer com emails e domínios.<br>
Para um IP, email ou domínio entrar em uma blacklist, ele precisa se tornar uma fonte provável de spam. Enviar uma quantidade muito grande de emails, ou emails com conteúdo preconceituoso, pornográfico ou com qualquer outro elemento em grande quantidade que seja contrário às regras do provedor como enviar muitos links, mesmo que não sejam maliciosos, podem levá-lo a uma blacklist.<br><br>
### Tipos
Há diversos tipos de blacklists, por isso é sempre bom saber em qual se está para que possa sair dela.<br>
As principais são:<br>
* ZEN Spamhauss
* SURBL
* URIBL
* Barracuda Central
* SpamCop
* Senderscore
* SORBS
* AHBL
* Abuse.ch
* RATS-NoPtr
### Como descobrir a sua
Há diversos sites que podem fazer essa verificação. O analista de suporte da empresa aonde eu estou estagiando utiliza o ![]()

### O que um IP tem a ver com uma blacklist que envolve, majoritariamente, emails?
Muito se fala de emails, mas o que esse tópico está fazendo em um artigo de IPs então?<br><br>
Oras, se um usuário não estiver recebendo e enviando emails por causa de seu IP, ele pode simplesmente trocá-lo e seguir a sua vida distribuindo ou não spams.<br>
Isso é verdade, mas se estivermos falando de um usuário da área empresarial, ele não conseguirá fazer isso, pois deve passar pelo servidor antes.<br>

### Como sair?
Para isso, deverá ser utilizado um site auxiliar para descobrir o responsável por colocar o seu IP na blacklist e, assim, enviar uma solicitação a ele, pedindo a sua retirada enquanto explica o motivo de estar lá.<br>
Um que pode ajudar é o [BlackListAlert](https://www.blacklistalert.org/).<br><br>
Além de verificar as blacklists, ainda mostra os seus responsáveis. Depois disso, basta anotar e contatá-los.
Em alguns casos, a retirada só é possível mediante pagamento, mas só acontece em situações mais raras e incomuns.<br><br>
<!-- IP no DOS e no Bash -->
