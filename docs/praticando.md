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

Acessar o diretório do repositório:

```bash
cd exercicios-git
```

---

[Próximo passo... Trabalhando com branch](./branch.md)