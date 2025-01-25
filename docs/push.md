# PUSH

Enviando as alterações para o repositório (GITHUB)

### 1. **Atualizando o repositório remoto**
Se você estiver trabalhando com um repositório remoto (como no GitHub ou GitLab), você pode fazer o upload das suas alterações com o comando `git push`.

```bash
git push

fatal: The current branch index has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin index
```



```bash
git push --set-upstream origin index

git push --set-upstream origin index
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 292 bytes | 292.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'index' on GitHub by visiting:
remote:      https://github.com/horadoqa/exercicios-git/pull/new/index
remote:
To github.com:horadoqa/exercicios-git.git
 * [new branch]      index -> index
Branch 'index' set up to track remote branch 'index' from 'origin'.
```

Na mensagem acima existe uma orientação:

```bash
Create a pull request for 'index' on GitHub by visiting:
remote:      https://github.com/horadoqa/exercicios-git/pull/new/index
```
Esse link nos permite criar um pull request, mas podemos verificar que na página do nosso repositório aparecerá uma mensagem referente ao nosso push, tipo:

  index had recent pushes on 24 de jan. 

e um botão `Compare & pull request` que veremos mais a seguir...

---

[Próximo passo... Criar um Pull Request (PR)](./pull-request.md)