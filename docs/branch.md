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
O Git permite criar ramificações (branches) para trabalhar em novas funcionalidades ou corrigir bugs sem afetar o código principal. O comando para criar uma nova branch é `git branch`

Exemplo:
```bash
git branch index
```

Para mudar de branch, você usa `git checkout`.

Exemplo:
```bash
git checkout index
```

Ou, você pode combinar os dois passos em um único comando:
```bash
git checkout -b index
```

Você também pode apagar uma branch
```bash
git checkout -d index
```

[Próximo passo... Criar as chaves pública e privada](/docs/keys.md)
