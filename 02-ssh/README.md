# SSH (secure shell)

## objetivo

Aprender instalar, configurar e utilizar o servico SSH para administracao remota de servidores Debian.

## instalar OpenSSH server
```bash
sudo apt update
sudo apt install openssh-server -y
```
instala servidor SSH

## verificar o status do servico

```bash
sudo systemctl status ssh
```
verifica se o servico esta em execucao

## Iniciar o servico
```bash
sudo systemctl start ssh
```

## Habilitar na inicializacao
```bash
sudo systemctl enable ssh
```
## reiniciar o servico
```bash
sudo sysmtectl restart ssh
```
## conectar a outro computador
```bash
ssh usuario@12.168.1.100
```
## arquivo de configuracao
```text
/etc/ssh/sshd_config
```
Apos alterar esse arquivo

```bash
sudo systemctl restart ssh
```

## verificar se a porta 22 esta aberta
```bash
sudo ss -tlnp | grep ssh
```

## o que aprendi

-instalar openssh server
-gerenciar o servico com systemd
-reaalizar o servico com systemd
-realizar conexoes remotas via SSH
-identificar o arquivo principal de configuracao
-reiniciar o servico apos alteracao