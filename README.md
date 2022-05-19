Nesse artigo iremos discorrer sobre alguns tipos de conexões, como:<br>
<ul>
<li>Cliente-Servidor;
<li>Ponta a ponta;
<li>CDN;
<li>Proxy Reverso
</ul>

# Conexão Cliente e Servidor
## O que é
A rede internet é regida por quem usa o serviço da rede e por quem provê, ou seja, cliente e servidor, respectivamente.<br><br>
Um cliente que deseja acessar um site, digita o seu domínio no navegador, este vai até o DNS para procurar o IP do site solicitado para estabelecer o acesso.<br><br>
Um servidor não é necessariamente uma máquina superpotente muito melhor que máquinas domésticas, mas sim uma máquina especialista em realizar uma função específica.<br><br>
A interação cliente - servidor é, então, a troca de informações entre duas máquinas (e não necessariamente máquinas físicas).
Essa interação ocorre em qualquer conexão entre dois dispositivos, onde o cliente quer serviços do servidor e o servidor quer servir o cliente.<br><br>
Outro exemplo: se eu quero conectar o meu celular a um fone bluetooth, uma rede para a troca de informações será construída. Essa rede é chamada PAN (Personal Area Network), mas também pode e ocorre em LAN, MAN, CAN e WAN.<br><br>
A conexão mais popular é a conexão de internet (que pode ter qualquer classificação, como já vimos no artigo sobre [Abragências](https://github.com/andersonr-o/Redes/blob/main/abrangencias-de-rede/README.md)). Na WEB, por exemplo, nosso dispositivo envia solicitações ao servidor destino, que nos retorna o que queremos, caso dê tudo certo na rota de comunicação.<br><br>
Assim se estabelece uma conexão de internet. Obviamente há muitos processos envolvidos em meio a tudo isso, mas essa é a base.<br><br>
Nosso cliente pode enviar solicitações a um servidor de arquivos, servidor de processos, servidor de terminal, ou a todos eles ao mesmo tempo. Isso é feito através da rede e todas as informações trocadas saem do núcleo de uma máquina e chegam ao núcleo da outra.<br><br>
Um servidor pode ser cliente de outro servidor. Por exemplo: um servidor de impressão pode ser cliente de um servidor de banco de dados para tomar uma decisão que um cliente solicitou.<br><br>
Exemplo de uma conexão, de maneira básica, entre um cliente e um servidor:<br><br>
![cliente-servidor-450](https://user-images.githubusercontent.com/97858145/166838654-9c3fc5aa-c27a-43db-9440-b55fa3bf4818.png)<br><br>
## Alguns tipos de servidores:
<ul>
  <li>Servidor Web &rightarrow; É um servidor que transaciona arquivos com o cliente, assim como o servidor de arquivos, mas somente arquivos web como jpeg, png, html, etc.
  <li>Servidor de banco de dados &rightarrow; Sua função é fornecer os dados solicitados para o cliente.
  <li>Servidor de Internet &rightarrow; Gerencia a comunicação das conexões dos usuários conectados na internet. É o servidor de internet que possui proxy para bloquear ou não quem vai acessar o quê.
</ul>

# Conexão Ponta a Ponta
É quando não há um servidor bem definidocomo intermediador; não existe um administrador na rede que gerencia todas as máquinas, ou seja, uma máquina conversa com todas as outras livremente. Essa é a principal diferença entre os dois.<br><br>
Em uma rede ponta a ponta não podemos utilizar serviços complexos como um banco de dados, por exemplo.<br><br>
Isso acontece porque a rede ponta a ponta tem o objetivo de ser simples e ter baixo custo. Um exemplo são as redes domésticas; não temos ninguém administrando todas as outras máquinas, a princípio.<br><br>
Por ser mais simples, a rede ponta a ponta torna-se mais vulnerável frente à conexão clinte e servidor.<br><br>
Se houver conexão entre um dispositivo e outro, temos a conexão ponta a ponta; se houver conexão entre um dispositivo e outros, há a conexão multiponto.<br><br>
Imagem de um exemplo de conexões ponta a ponta e multiponto:<br><br>
![ponta-a-ponta](https://user-images.githubusercontent.com/97858145/166844561-ea2567b0-3c45-4a71-8634-5a6faf4c384f.png)

# CDN (Content Delivery Network)
## Como funciona?
Ou, em português, Rede de Distribuição de Conteúdo, o CDN funciona, basicamente, como um intermediador entre o cliente e o servidor. Mas para que queremos um intermediador? Ele não iria atrasar a conexão?<br><br>
Não. O CDN, na verdade, deixa ela mais rápida.<br><br>
Ele recebe a nossa solicitação ao servidor e o guarda em uma memória temporária. Mas o cliente nem sempre procura o servidor físico mais próximo. O CDN faz isso, diminuindo a latência e aumentando a rapidez da conexão.<br><br>
Isso se já não existir o mesmo arquivo na memória temporária do seu servidor CDN. Se for o caso, a conexão será mais rápida ainda.<br><br>
Alguns serviços de CDN, quando buscam a sua solicitação no servidor físico mais próximo, já os guarda em todos os outros CDNs ao redor do mundo, até que sua memória temporária expire.<br><br>
Essa memória temporária serve enquanto não alteramos a solicitação. Se queremos o conteúdo X do servidor, enviamos a solicitação, e depois querermos mudar para o Y, ele removerá a solicitação do conteúdo X de sua memória temporária e nos dará o Y.<br><br>
O CDN opera sobre arquivos estáticos, como imagens, vídeos, html, css, javascript e até PDFs.
## Como o serviço de CDN sabe a nossa localização?
Ele sabe através do nosso IP, que mostra até o nosso município, aumentando a precisão da localização de um servidor físico próximo.<br><br>
Se quiser saber mais sobre o assunto de rastreamento de IP, recomendo o [Vídeo do Gabriel Pato](https://m.youtube.com/watch?v=6WZox0-Tc3k).
## Como usar o CDN
Trata-se de um serviço pago, com um serviço semelhante a um provedor de internet. Basta comparar e escolher o que melhor te agrada.
<!--Proxy Reverso-->
