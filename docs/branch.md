# Branch

Um projeto pode ter diversos colaboradores, entre eles, devs, devops, dbas... para isso precisamos organizar de forma que cada um tenha o sua própria versão de código para poder validar suas modificações e só depois de testadas poderem ser atualizadas para a branch `main` que é a branch principal.

### 1. **Listando as branchs**
Você pode verificar as branchs locais do projeto com o comando:
```bash
git branch
```

Pressione a letra `q` para sair da visualização das branchs.

ou 

O comando git branch -a mostra todas as branches, tanto as locais quanto as remotas.

```bash
git branch -a
```

Pressione a letra `q` para sair da visualização das branchs.

### 2. **Criando e mudando de branch**
O Git permite criar ramificações (branches) para trabalhar em novas funcionalidades ou corrigir bugs sem afetar o código principal. O comando para criar uma nova branch é `git branch`

Exemplo:
```bash
git branch index
```

Para mudar de branch, você usa `git checkout`.

Exemplo:
```bash
git checkout index

Switched to branch 'index'
Your branch is up to date with 'origin/index'.
```

Ou, você pode combinar os dois passos em um único comando:
```bash
git checkout -b index
```

Verifique que o prompt muda:

de: `git:(main)`

para: `git:(index)`

Essa mudandça indica que agora estamos trabalhando dentro da branch `index`.

Você pode verificar a mudança utilizando o comando `git branch`

```bash
git branch

* index
  main
```

O (*) indica a branch atual.

**OBS.:** Estamos usando o [Oh My ZSH](https://ohmyz.sh/), para instalação siga os procedimentos no site.

Você também pode apagar uma branch localmente
```bash
git branch -d index

ou 

git branch -D index
```

A opção -d é a forma segura de deletar, ou seja, ela só exclui a branch se todas as alterações já tiverem sido integradas (comitadas) em outra branch.

Se você tem certeza de que deseja excluir a branch, mesmo que ela não tenha sido mesclada (merged), use a opção -D (com D maiúsculo), que forçará a remoção:

Remotamente

```bash
git push origin --delete index

To github.com:horadoqa/exercicios-git.git
 - [deleted]         index
```

---

[Próximo passo... Adicionar arquivos ao repositório](./files.md)