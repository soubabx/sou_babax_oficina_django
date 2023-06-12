# Introdução a linha de comando

**O que é a linha de comando?**
A janela, que normalmente é chamada de linha de comando ou interface de linha de comando, é uma aplicação baseada em texto para visualização, manipulação e manuseio de arquivos em seu computador. Outros nomes para a linha de comando são: cmd, CLI, prompt, console ou terminal.

**Seu primeiro comando (YAY!)**
Vamos começar com algo simples. Digite o seguinte comando:
```
$ whoami
```
Depois tecle Enter. Essa é nossa saída:
```
$ whoami
www-data
```
Como você pode ver, o terminal só apresentou o nome de usuário, no caso www-data.

**O básico**
Cada sistema operacional tem o seu próprio conjunto de instruções para a linha de comando, mas no codespaces usamos um sistema Linux.

**- Pasta atual**
Seria legal saber em que pasta estamos agora, certo? Vamos ver. Digite o seguinte comando seguido de um enter:
```
$ pwd
/mnt/project
```
Provavelmente você vai ver algo parecido na sua máquina.

**- Criando uma pasta**
Que tal criar um diretório (pasta) chamado "minhapasta" no seu projeto chamado afropython? Você pode fazer assim:
```
$ mkdir minhapasta
```
Este comando vai criar uma pasta com o nome "minhapasta" no nosso projeto chamado afropython. Vamos verificar se ela está lá?

**- Listando arquivos e pastas**
Digite o seguinte comando:
```
$ ls
minhapasta
```
Ali está a pasta criada! Vamos entrar nela?

**- Entrando nas pastas**
Para entrar na pasta, digite o seguinte comando:
```
$ cd minhapasta
```
Veja se realmente entramos na pasta:
```
$ pwd
/mnt/project/minhapasta
Aqui está!
```
> Dica de profissional: se você digitar `cd m` e apertar a tecla tab no seu teclado, a linha de comando irá preencher automaticamente o resto do nome para que você possa navegar rapidamente. Se houver mais de uma pasta que comece com "m", aperte a tecla tab duas vezes para obter uma lista de opções. E se você não quiser digitar o mesmo comando várias vezes, tente pressionar seta para cima e seta para baixo no teclado para percorrer comandos usados recentemente.

**- Limpando**
Não queremos deixar uma bagunça, então vamos remover tudo o que fizemos até agora. Primeiro, precisamos voltar para nosso workspace (área de trabalho):
```
$ cd ..
```
Fazendo `cd ..` nós mudaremos do diretório atual para o diretório pai (que significa o diretório que contém o diretório atual). Veja onde você está:
```
$ pwd
/mnt/project
```
Agora é hora de excluir o diretório "minhapasta". Atenção: A exclusão de arquivos usando `del`,

 `rmdir` ou `rm` é irreversível, significando que os arquivos excluídos vão embora para sempre! Então, tenha cuidado com este comando.
```
$ rm -r minhapasta
```
Pronto! Para ter certeza de que a pasta foi excluída, vamos checar:
```
$ ls
```
Por enquanto é isso!
