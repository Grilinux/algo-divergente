# algo-divergente
Para clonar este repositório foi utilizado o seguinte comando:
```git
git clone https://github.com/FilipeS0usa/algo-divergente.git
```
## Initial commit
Para o primeiro commit foram utilizados os seguintes comandos:

```bash
git add README.md
git commit -m "Initial commit"
git push
```
git add para adicionar o ficheiro
git commit para fazer o commit com a respectiva mensagem
git push para enviar para o repositório remoto

## Filipe Silva

- Foi criado um novo branch chamado FilipeBranch:

```bash
git checkout -b "FilipeBranch"
```

- Foi adicionado o ficheiro main.py, adicionei e fiz commit:

```bash
git add .
git commit -m "Added main.py and updated README.py"
git push
```

- O ficheiro main.py sofreu 3 updates diferentes:

```bash
git add main.py
git commit -m "Updated main.py"
```

- Voltou-se ao branch main, e utilizou-se o cherry-pick para escolher um commit especifico para ser aplicado no main. Neste caso escolheu-se o Update main.py 2:

```bash
git checkout main
git cherry-pick 178d02b
```
Devido ao ficheiro main.py não existir no branch main, houve um conflito. Para resolver este conflito foram efectuados os seguintes comandos:
1. Primeiramente verificou-se se haviam algumas alterações nos ficheiros envolvidos no cherry-pick
```bash
cat main.py
cat README.md
```
2. Como não havia nenhuma alteração nos ficheiros fez-se o seguinte comando para resolver o conflicto:
```bash
git add .
git cherry-pick --continue
```
- De seguida fez-se o merge do branch FilipeBranch com o main:
```bash
git merge FilipeBranch
```

Houve conflictos ao fazer o merge.

1. Para ver quais eram os conflictos fez-se os seguintes comandos

```bash 
cat main.py
cat README.py
```
2. Para resolver os conflictos então editou-se o que era suposto editar e fez-se os seguintes comandos:
```bash
git add .
git commit -m "Solved merge conflict"
```
- Agora esta versão será a versão 1.0 do projecto. Ficando assim mais fácil de acompanhar as versões do projecto, para isso fez-se o seguinte comando:
```bash
git tag v1.0 5541754
```
- Por fim falta ainda usar o rebase, para isso vamos criar um novo branch thisIsRebase, fazer mais uns commits e fazer o respectivo rebase:
```bash
git checkout -b thisIsRebase
git add README.md
git commit -m "Updated README.md"
git add main.py
git commit -m "Added new feature to main.py"
git rebase main
git rebase thisIsRebase
```


## Hugo Almeida

## João Correia
