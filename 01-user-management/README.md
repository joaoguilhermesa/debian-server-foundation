>Laboratório prático desenvolvido durante meus estudos de administração Linux.
# Gereciamento de Usuários

## Cenário
Novo usuário chamado **joao** precisa de acesso a um servidor Debian. O objetivo é criar uma conta, garantir privilégios administrativos e verificar a configurações de identificação.

## Objetivo
- Criar um usuario no sistema;
- Conceder privilegios administrativos ao novo usuario;
- Comfirmar o UID, GID e os grupos associados ao usuário.

## Ambiente
- S.O: Debian 13
- Usuario: debian
## Criar usuário

```bash
sudo adduser joao
```
Cria um novo usuário chamado **joao** e pede por configuração de senha.

## Resultado
![Criacao do usuario](Images/01-add-user.png)

## Adicionar o novo usuario ao grupo sudo

```bash
sudo usermod -aG sudo joao
```
Adiciona o usuário **joao** ao grupo 'sudo' permitindo a este usuário executar comandos administrativos.

## Resultado
![Permissao concedida ao usuario](Images/02-user-sudo.png)

## Verificar o usuário

```bash
id joao
```

## Resultado
![Informacoes do usuario](Images/03-id-user.png)

## Verificar os grupos 

```bash
groups joao
```

## Resultados

![Grupos](Images/04-groups.png)

## O que aprendi
- Criar usuario;
- Adicionar usuario ao grupo sudoers;
- Verificar UID  e GID;
- Confirmar grupos do usuarios;

## Conclusão
Este laborátorio é demonstrado o básico de criação de usuários, atribuição de privilégios administrativos e verificação da conta criada


## Referências
https://manpages.debian.org
https://wiki.debian.org/
https://www.gnu.org/software/coreutils
