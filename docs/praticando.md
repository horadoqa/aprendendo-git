# Praticando

Aqui estão alguns conceitos e exemplos de como usar o Git:

### 1. **Criando um repositório**

Dentro do site: https://github.com/horadoqa, acessamos a aba `Repositories` e depois clicamos em `New`.

Será solicitado:

O `Repository name*`, nome do repositório, para este exercício, usaremos:
    
    exercicios-git

O `Description (optional)`, um descrição sobre o repositório.
    Exercícios de git e github

Selecionar se o repositório vai ser `Public` ou `Private`.

Selecionar `Add a README file`, o repositório vai ser inicializado com o arquivo README.md, arquivo que tem as observações do projeto
    
    # Página WEB, com html, css e javascript

Após esta configuração, clicar em: `Criar repositório`.

O repositório será criado com o nome `exercicios-git`.

### 2. **Clonando um repositório**
Podemos fazer uma cópia do projeto para a nossa máquina e trabahar no código usando o comando `git clone`.

Para isso, precisamos acessar o repositório que criamos anteriormente e fazer uma cópia, usando o comando `git clone`.

Exemplo:
```bash
git clone <url do repositório>
```

Em nosso terminal, pode ser direto via CLI ou no Visual Studio Code.
```bash
git clone git@github.com:horadoqa/exercicios-git.git
```

### 3. **Adicionando arquivos ao repositório**
Após criar o arquivo `index.html`, você pode começar a criar o código e logo após adicionar a alteração com o comando `git add`.

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
```

### 5. **Verificando o status do repositório**
Você pode verificar o status do repositório para ver quais arquivos foram modificados, quais estão preparados para o commit, e quais ainda precisam ser adicionados.

Exemplo:
```bash
git status
```

### 6. **Visualizando o histórico de commits**
Para ver o histórico de commits, use o comando `git log`. Ele exibe uma lista de todos os commits feitos, com detalhes como ID do commit, autor, data e a mensagem de commit.

Exemplo:
```bash
git log
```

[Próximo passo... Trabalhando com branch](/docs/branch.md)