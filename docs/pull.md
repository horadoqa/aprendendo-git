# PULL

### 1. **Obtendo as últimas alterações do repositório remoto**
Para trazer as últimas mudanças do repositório remoto para o seu repositório local, você pode usar o comando `git pull`.


Alterar para a branch `main`

```bash
git checkout main
```

Executar o comando:
```bash
git pull

remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 892 bytes | 178.00 KiB/s, done.
From github.com:horadoqa/exercicios-git
   3faa9a7..fe48348  main       -> origin/main
Updating 3faa9a7..fe48348
Fast-forward
 index.html | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html
```

---

[Próximos passos...Criar uma branch chamada css e o arquivo style.css e depois atualizar a branch main](./files.md)