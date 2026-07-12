# File permissions and ownership

##objetivo 
aprender a visualizar e modificar permissoes de arquivos e diretorios, alterar propriedades e compreender como o sistema de permissao funciona no Linux


## visualizar permissoes

```bash
ls -l
```
Exibe as permissoes, proprietario, grupo e outras  informacoes dos arquivos.

exemplo:
```text
-rwxr-xr-- 1 joao users 1024 jul 24 arquivo.txt
```

## alterar permissoes

adicionar permissao de execucao para o proprietario:

```bash
chmod u+x arquivo.sh
```

adicionar permissao de leitura para todos:

```bash
chmod a+r arquivo.txt
```

remover permissao de escrita do grupo:

```bash
chmod g-w arquivo.txt
```
permissao numerica:

```bash
chmod 775 script.sh
```


## alterar proprietario

```bash
sudo chown joao arquivo.txt
```

alterar proprietario e grupo:

```bash
sudo chown joao:users arquivo.txt
```

## alterar grupo
```bash
sudo chgrp users arquivo.txt
```

## o que aprendi
-interpretar permissao de arquivo
-modificar permissao de arquivos para usuarios e grupos
-utilizar chmod em modo simbolico e numerico
-relacao entre usuario grupo e permissoes
