## gerenciammaneto de users
Comandos estudados
## adicona ususario
```bash 
sudo adduser joao
```
## da permissao de admin para o user
```bash 
sudo usermod -aG sudo joao

## ver inforacao do user
id joao
## grupos 
groups joao
## ver a lista de usuarios com acesso a sudo
cat /etc/sudoers
## da permissao ao usuario modificar e executar arquivor
sudo joao chmod a+x joaoguilhermesa.txt 
```
## altera senha de usuario
```bash
sudo passwd joao
````
## remove usuario
```bash
sudo deleuser joao

```
Objetivos
Aprender criacao de usuarios, grupos e permissoes basicas na distro Debian

Aprendi
-diferenca entre usuarios comum e root
-manipular roles de usuarios comums e root
-visualizacao em uid, gid e grupos.