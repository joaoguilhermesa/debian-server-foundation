#user management

## Cenario
novo usuario chamado **joao** ingressou no sistema e precisa de uma conta no servidor debian para acessar

## Objetivo
Criar um usuario;
Conceder privilegios administrativos ao novo usuario;
Comfirmar que o usuario pertence ao grupo "sudo".

## Ambiente
PC Debian 13 i3wm
Usuario: root
## Criar usuario

```bash
sudo adduser joao
```
## Resultado
![Criacao do usuario](Images/01-add-user.png)

## Adicionar o novo usuario ao grupo sudo

```bash
sudo usermod -aG sudo joao
```
## Resultado
![Permissao concedida ao usuario](Images/02-user-sudo.png)

## Verificar usuario

```bash
id joao
```

## Resultado
![Informacoes do usuario](Images/03-id-user.png)

## Verificando grupos 

```bash
groups joao
```

## Resultado

![Grupos](Images/04-groups.png)

## O que aprendi
Criar usuario;
Adicionar usuario ao grupo sudoers;
Verificar UID  e GID;
Comfirmar grupos do usuarios;

