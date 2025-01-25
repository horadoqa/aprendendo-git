# Trabalhando com arquivos

### 1. **Adicionando arquivos ao repositório**

Podemos criar o arquivo via CLI mesmo com o comando `touch`
```bash
touch index.html
```

### 2. **Verificando o status do repositório**
Você pode verificar o status do repositório para ver quais arquivos foram modificados, quais estão preparados para o commit, e quais ainda precisam ser adicionados.

Exemplo:
```bash
git status
On branch index
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)
```
### 3. **Adicionando as modificações para serem commitadas**
você pode adicionar a alteração com o comando `git add`.

Exemplo:
```bash
git add index.html
```
Ou para adicionar todos os arquivos no diretório:
```bash
git add .
```

### 4. **Fazendo um commit**
O commit é usado para registrar as alterações feitas nos arquivos. Para fazer um commit, você precisa escrever uma mensagem que descreva o que foi alterado.

Exemplo:
```bash
git commit -m "Criando o arquivo index.html"

[main 27d018d] Criando o arquivo index.html
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html
```

### 5. **Visualizando o histórico de commits**
Para ver o histórico de commits, use o comando `git log`. Ele exibe uma lista de todos os commits feitos, com detalhes como ID do commit, autor, data e a mensagem de commit.

Exemplo:
```bash
git log

commit f118ef7002bbae06bbcaf58c414fcfa58f1c9d83 (HEAD -> index)
Author: Ricardo Fahham <rfahham@hotmail.com>
Date:   Fri Jan 24 14:26:58 2025 -0300

    Criando o arquivo index.html

commit 3faa9a7a746e9953941fdadac6b8aa813c2ed9e4 (origin/main, origin/HEAD, main)
Author: Hora do QA <horadoqa@gmail.com>
Date:   Fri Jan 24 14:26:04 2025 -0300

    Initial commit
```

Pressione a letra `q` para sair da visualização do log.

---

[Próximo passo... Criar as chaves pública e privada](./keys.md)