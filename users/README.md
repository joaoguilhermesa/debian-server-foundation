# Gerenciamento de usuarios

## Objetivos 
Aprender criacao de usuarios, grupos e permissoes basicas na distro Debian

## Adicionar um usuario
```bash 
sudo adduser joao
```
Cria um novo usuario e solicita senha e informacoes adicionais.

## Adiciona o usuario ao grupo sudoers
```bash 
sudo usermod -aG sudo joao

Concede privilegios adiministratrivos ao usuarios por meio do grupo sudo

## ver inforacao do usuario
```bash
id joao
```
Exibe UID, GID e os grupos aos quais o usuario pertence.

## Ver usuarios com privilegios sudo\
```bash 
groups joao
```
Mostra todos os grupos que o ususario pertence

## Ver usuarios co privilegios sudo
```bash
cat /etc/sudoers
```
## Alterar permissao de um arquivo
```bash
chmod a+x joaoguilhermesa.txt 
```
Adiciona permissao de execucao para todos os usuarios
>> se o arquivo pertence a outro ususario
```bash
sudo bash chmod a+x joaoguilhermesa.txt
```
## Altera senha do usuario
```bash
sudo passwd joao
```

## remove usuario
```bash
sudo deluser joao
```
Aprendi malinupalcao com usuarios, permissoes, grupos, UID, GID, 
Diferenca entre usuario comum e root
Como adicionar usuarios ao grupo sudo
Commo alterar permisao basica de arquivos