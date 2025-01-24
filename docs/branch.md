# Branch

Um projeto pode ter diversos colaboradores, entre eles, devs, devops, dbas... para isso precisamos organizar de forma que cada um tenha o sua própria versão de código para poder validar suas modificações e só depois de testadas poderem ser atualizadas para a branch `main` que é a branch principal.

### 1. **Listando as branchs**
Você pode verificar as branchs locais do projeto com o comando:
```bash
git branch
```

ou 

O comando git branch -a mostra todas as branches, tanto as locais quanto as remotas.

```bash
git branch -a
```

### 2. **Criando e mudando de branch**
O Git permite criar ramificações (branches) para trabalhar em novas funcionalidades ou corrigir bugs sem afetar o código principal. O comando para criar uma nova branch é `git branch`, e para mudar de branch, você usa `git checkout`.

Exemplo:
```bash
git branch index
git checkout index
```

Ou, você pode combinar os dois passos em um único comando:
```bash
git checkout -b index
```

### 3. **Merge de branches**
Depois de terminar o trabalho em uma branch, você pode unir suas alterações de volta à branch principal (geralmente chamada de `main` ou `master`) usando o comando `git merge`.

Exemplo:
Primeiro, mude para a branch principal:
```bash
git checkout main
```
Depois, faça o merge da branch com a nova funcionalidade:
```bash
git merge index
```

### 4. **Atualizando o repositório remoto**
Se você estiver trabalhando com um repositório remoto (como no GitHub ou GitLab), você pode fazer o upload das suas alterações com o comando `git push`.

Exemplo:
```bash
git push origin main
```

Isso envia as alterações para a branch `main` do repositório remoto.

### 5. **Obtendo as últimas alterações do repositório remoto**
Para trazer as últimas mudanças do repositório remoto para o seu repositório local, você pode usar o comando `git pull`.

Exemplo:
```bash
git pull origin main
```

Esses são apenas alguns dos comandos básicos do Git, mas ele oferece muito mais funcionalidades, como resolução de conflitos, rebase, stashing, etc.

[Próximo passo... Criar um Pull Request (PR)](/docs/pull-request.md)
