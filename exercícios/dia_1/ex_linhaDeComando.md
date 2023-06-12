## Exercício de linha de comando

1. Crie uma pasta chamada "meus_arquivos" no diretório atual.
2. Dentro da pasta "meus_arquivos", crie dois arquivos de texto: "notas.txt" e "tarefas.txt".
3. Verifique o conteúdo da pasta "meus_arquivos".
4. Renomeie o arquivo "notas.txt" para "anotacoes.txt".
5. Crie uma pasta chamada "documentos" dentro da pasta "meus_arquivos".
6. Mova o arquivo "tarefas.txt" para a pasta "documentos".
7. Verifique novamente o conteúdo da pasta "meus_arquivos" para confirmar as alterações.

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

> Solução:

```
$ mkdir meus_arquivos
$ cd meus_arquivos
$ touch notas.txt tarefas.txt
$ ls
notas.txt tarefas.txt
$ mv notas.txt anotacoes.txt
$ mkdir documentos
$ mv tarefas.txt documentos
$ ls
anotacoes.txt documentos
$ ls documentos
tarefas.txt
```
