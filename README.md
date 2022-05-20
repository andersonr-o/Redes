# Principais Protocolos e Portas de Comunicação
 Basicamente, uma porta de comunicação é por onde entrará e sairá dados do computador. Elas que organizam o que entra ou não.
Se não fosse assim, seria uma bagunça. Tudo entraria ao mesmo tempo e a tela ficaria poluída ou não entraria nada em momentos desejados.
As portas são representadas por números, que vão de 0 a 65.535.
## Portas Baixas (well known ports):
São destinadas aos protocolos de serviços, como os servidores e serviços de internet. Vão de 0 a 1023.
## Portas Altas:
São destinadas aos clientes (respostas às requisições dos clientes). Vão de 1024 a 65.535.
## Principais Portas e Protocolos:
Veremos somente as de serviços, que, além de serem as mais conhecidas, são as mais importantes para quem quer entender sobre Redes.
<ul>
 <li>
   20/21 &rightarrow; FTP:<br>
   Serve para a transferência de arquivos de dados. A porta 20 refere-se aos dados e a 21 ao controle desses dados.
   Podemos ver o FTP quando plugamos o nosso celular na USB do computador, lá aparece a opção de tranferirmos FTP, isto é, arquivos;<br><br>
 </li>
 <li>
   22 &rightarrow; SSH:<br>
   É um terminal remoto criptografado. Essa porta é acionada quando acessamos outro computador, que não seja o nosso, remotamente;<br><br>
 </li>
 <li>
   23 &rightarrow; Telnet:<br>
   Trata-se de outro terminal remoto, mas dessa vez descriptografado. Quando ele está descriptografado, significa que todos os usuários da rede podem ginfar a porta;<br><br>
 </li>
 <li>
   25/587 &rightarrow; SMTP:<br>
   É uma porta de envio de e-mails. A porta 25 não é mais utilizada. Ela foi anulada pelo Comitê Gestor de Internet após negociações com os provedores, devido ao alto número de spammers nela. (não confundir com webmail.);<br><br>
 </li>
 <li>
   53 &rightarrow; DNS:<br>
   Associa um IP a um nome e um nome a um IP. É como se fosse a agenda do seu celular. Você não precisa saber o número de toda pessoa que for ligar, mas sim saber o seu nome e procurar na agenda. Isso é útil porque todo site é um IP. Graças ao DNS, não precisamos decorá-los;<br><br>
 </li>
 <li>
   67 &rightarrow; DHCP:<br>
   Distribui as configurações de rede necessárias para a conexão aos dispositivos, tais como IP, gateway, máscara de rede, DNS, etc;<br><br>
 </li>
  <li>
   69 &rightarrow; TFTP:<br>
   Transfere arquivos simples, como a configuração de arquivos da rede;<br><br>
  </li>
  <li>
   79 &rightarrow; Finger:<br>
   Transfere informações dos usuários conectados na rede;<br><br>
  </li>
  <li>
   80 &rightarrow; http:<br>
   Transfere hipertexto (textos com configurações adicionais que o tornam dinâmico);<br><br>
  </li>
  <li>
   110 &rightarrow; pop:<br>
   Ao contrário do SMTP, o pop é responsável pelo recebimento dos e-mails. Os e-mails recebidos na porta pop somem do servidor depois de um tempo;<br><br>
  </li>
  <li>
   123 &rightarrow; NTP:<br>
   Sincroniza data e hora entre os dispositivos da rede;<br><br>
  </li>
  <li>
   143 &rightarrow; imap:<br>
   Igual ao pop, também é responsável pelo recebimento de e-mails, mas o imap guarda-os no servidor.<br>
   Sendo assim, o usuário pode acessar os mesmos e-mails em outros dispositivos através da sincronização com o servidor;<br><br>
  </li>
  <li>
   161/162 &rightarrow; SNMP:<br>
   Gerencia as conexões de rede (quantos e quais IPs estão conectados, há quanto tempo, etc);<br><br>
  </li>
  <li>
   443 &rightarrow; https:<br>
   Faz a mesma coisa que o http, mas o https é criptografado com SSL E TLS.
  </li>
