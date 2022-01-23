# Escapes
Arquivo: /etc/issue <br>
Fonte: https://manpages.debian.org/bullseye/manpages-pt-br/issue.5.pt_BR.html <br>
Fonte: Manual disponivel no pacote getty

Todo Escape deve ser 'liberado' com a barra invertida no começo \, no exemplo abaixo o sistema subistituira o 4 pelo endereço IPv4
 > Endereço IPV4: \4
 
Lista de scapes:

> **\4** - Exibe o endereço IPv4 da primeira interface listada.
> 
> **\4{interface}** - Exibe o endereço IPV4 da interface selecionada. 
> >EX de uso: \4{eth0} 
>
> **\6** - Exibe o endereço IPV6 da primeira interface listada
> 
> **\6{interface}** - Exibe o endereço IPV6 da interface selecionada. 
> >EX de uso: \6{eth0}
>
> **\S{VARIAVEL}** -Exibe os dados da variavel correspondente de /etc/os-release, se nenhuma for epecificada ele exibira a variavel *PRETTY_NAME* por padrão, lembrando que as variaveis podem mudar de acordo com a distribuição e/ou versão do sistema, considere as informações abaixo apenas como consulta.
>> PRETTY_NAME    = Nome do S.O com versão.
>> 
>> NAME           = Nome do S.O.
>> 
>> VERSION_ID     = Versão do S.O (7,8,9,10 e etc...).
>> 
>> VERSION        = Nome da versão do S.O (wheezy, jessie, stretch, buster e etc).
>> 
>> ID             = Nome do Sistema (Debian, Ubuntu & etc).
>> 
>> HOME_URL       = Home da página do sistema.
>> 
>> SUPPORT_URL    = Pagina de suporte do sistema.
>> 
>> BUG_REPORT_URL = Pagina de report de bugs do sistema.
>> 
> **\b** - Exibe a taxa de baudrate atual do sistema.
>
> **\d** - Exibe a data atual do sistema.
>
> **\l** - Exibe qual o TTY atual.
> 
> **\m** - Exibe a arquitetura do host o mesmo que **uname -m**.
> 
> **\n** - Exibe o hostname do host o mesmo que **uname -n**.
> 
> **\s** - Exibe o nome do Kernel, o mesmo que **uname -s**.
>
> **\r** - Exibe a versão do Kernel, o mesmo que **uname -r**.
>
> **\o** - Exibe o nome de Dominio NIS do host, o mesmo que **hostname -d**.
> 
> **\O** - Exibe o nome DNS do host.
> 
> **\t** - Exibe a hora atual do sistema (não atualiza automaticamente).
> 
> **\u** - Exibe o número de usuários conectados no sistema (1,2,3 e etc).
> 
> **\U** - Exibe o número de usuários conectados no sistema (1 user, 2 user, 3 user e etc).
> 
> **\v** - Exibe o S.O, versão e data de compilação


# Exemplo de aplicação
Código: <br>
![image](https://user-images.githubusercontent.com/52683780/150691565-cc2c14ea-14a2-4b53-be26-e56e322caac5.png)

Resultado: <br>
![image](https://user-images.githubusercontent.com/52683780/150691606-320274ea-7c79-4f76-82eb-1db0376fd593.png)

Outro exemplo um pouco mais personalizado;<br>
Código: <br>
![image](https://user-images.githubusercontent.com/52683780/150692287-23e59659-edf6-40c0-a996-91720ee54af6.png)

Resultado:<br>
![image](https://user-images.githubusercontent.com/52683780/150692091-780d80b7-46df-45a2-a360-c4ec54753037.png)

Para a geração do simbolo do Debian foi usado o pacote **Linux-Logo** 
> http://www.deater.net/weave/vmwprod/linux_logo/

A partir daqui, a imaginação é o limite.
