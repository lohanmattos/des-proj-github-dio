# Os 13 comandos GIT mais usados

![](C:\Users\lohanamendola\Desktop\Estudos na Plataforma da DIO\Bootcamps\Impulso Javascript Evolution\Módulo I - Princípios de Desenvolvimento de Software\desafio-git\des-proj-github-dio\comandos-git.png.webp)

### Git init

Para começar um projeto que ainda não seja um repositório (ou repo), o Git Init costuma ser o comando mais indicado. 

Basicamente, ele cria um repositório vazio ou transforma uma pasta que você já tem e que não está com controle de versão em um repositório:

```
git init
```
Com sua pasta de trabalho devidamente iniciada, é hora de começar a preenchê-la.

### Git clone
O Git clone é um comando para baixar o código-fonte existente de um repositório remoto (como o Github, por exemplo).

Existem algumas maneiras de baixar o código-fonte, mas eu prefiro o clone com o modo https:

```
git clone <https://url-do-link>
```

Quando você clonar um repositório, o código é copiado para a o seu computador e continua linkado ao original, como foi explicado lá na descrição do que é um sistema distribuído.

Se você quiser desvincular a sua cópia do original, rode o comando abaixo:

```
git remote rm origin
```

### Git branch
Com as branches (ou ramificações), vários desenvolvedores podem trabalhar paralelamente no mesmo projeto. Assim, cada um pode codar a sua parte sem que haja confusão! 

Funciona basicamente da seguinte forma: a cada alteração realizada no código, seja para adicionar um novo recurso ou até mesmo corrigir um erro, cria-se um novo ponto de ramificação que consolida essas mudanças, sem interferir nos arquivos originais. 

Considerado um dos comandos Git mais importantes, o branch pode ser usado para três finalidades diferentes: criar, listar e excluir ramificações. Veja, na sequência, como trabalhar com cada uma delas.Para criar uma nova branch local, digite:

```
git branch <nome-da-branch>
```

Este comando criará uma branch local. Para upar a nova branch para o repositório remoto, você precisa usar o seguinte comando:
```
git push -u <remote> <nome-da-branch>
```
Para ver as ramificações, por sua vez, use:
```
git branch
```
ou
```
git branch --list
```
Por último, delete uma branch a partir do comando:
```
git branch -d <nome-da-branch>
```
### Git checkout
Esse é um dos comandos git mais utilizados. Para trabalhar em uma branch, primeiro você precisa mudar para ela. Apesar de parecer algo óbvio, não ir para a branch que você acabou de criar e na qual quer trabalhar é um erro bastante comum no começo.

Neste contexto, o principal objetivo do git checkout é ajudar você a mudar de uma branch para outra ou então verificar arquivos e commits:
```
git checkout <nome-da-ramificação>
```
Há ainda um comando de atalho que te permite criar e ir para um branch de uma vez só:
```
git checkout -b <nome-da-branch>
```

### Git status
Sim, já falamos sobre ele, mas vale retomar: o comando Git status serve para fornecer algumas informações importantes sobre a branch em que você estiver no momento, incluindo se ela está atualizada em relação à master e quais arquivos foram alterados.
```
git status
```


### Referências

[geekhunter](https://blog.geekhunter.com.br/comandos-git-mais-utilizados/)
