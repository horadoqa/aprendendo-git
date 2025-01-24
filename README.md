# Guia de Git e GitHub

Bem-vindo ao repositório "Aprendendo Git e GitHub"! 

Este repositório é um recurso abrangente para entender e usar Git e GitHub, ferramentas essenciais para controle de versão e colaboração em projetos de software.

## Índice

- [O que é Git?](#o-que-é-git)
- [O que é GitHub?](#o-que-é-github)
- [Instalação do Git](#instalação-do-git)
- [Comandos Básicos do Git](#comandos-básicos-do-git)
- [Usando o GitHub](#praticando)
- [Commits Semânticos](#commits-semânticos)
- [Contribuições](#contribuições)

## O que é Git?

Git é um sistema de controle de versão distribuído que permite que desenvolvedores gerenciem e acompanhem alterações em projetos de software. Ele ajuda a manter um histórico de versões, permite a colaboração em equipe e facilita a reversão de alterações.

O Git foi criado por Linus Torvalds, o mesmo criador do Linux. Ele desenvolveu o Git em 2005 para gerenciar o código fonte do kernel do Linux de forma mais eficiente. A motivação principal para o desenvolvimento do Git foi a insatisfação com os sistemas de controle de versão existentes na época, especialmente após problemas com o sistema de controle de versão usado pelo projeto do Linux.

[Saiba mais...](git.md)

## O que é GitHub?

GitHub é uma plataforma de hospedagem de código-fonte que utiliza Git. Ela permite que desenvolvedores colaborem em projetos, façam revisões de código e automatizem fluxos de trabalho de desenvolvimento através de funcionalidades como GitHub Actions.

O GitHub pertence à Microsoft. A Microsoft adquiriu o GitHub em 2018, por cerca de 7,5 bilhões de dólares em ações da empresa. Embora o GitHub tenha se tornado parte da Microsoft, ele continua funcionando como uma plataforma independente, com foco em desenvolvimento de software colaborativo e hospedagem de código-fonte usando Git.

[Saiba mais...](github.md)

## Instalação do Git

Para instalar o Git, siga estas etapas:

1. **Windows**: O Git Bash faz parte do pacote Git for Windows.

Baixe o instalador do [site oficial do Git](https://git-scm.com/download/win) e siga as instruções.

2. **macOS**: Você pode instalar usando o Homebrew:
   
   ```bash
   brew install git
   ```

3. **Linux**: Use o gerenciador de pacotes da sua distribuição. Por exemplo, no Ubuntu

    ```bash
    sudo apt-get install git
    ```

## Comandos básicos do git

- git init: Cria um novo repositório Git.
- git clone: Faz uma cópia de um repositório remoto.
- git add: Adiciona arquivos ao índice para preparação para commit.
- git commit: Registra as mudanças no repositório local.
- git push: Envia as alterações locais para um repositório remoto.
- git pull: Atualiza o repositório local com alterações do repositório remoto.
- git checkout: Cria ou deleta branches.
- git branch: Gerencia branches (criação, listagem, exclusão).
- git merge: Mescla alterações de diferentes branches.
- git rm: Utilizado para remover arquivos do seu repositório Git

## Praticando

No github, vamos criar um repositório chamado exercícios-git e dentro dele um index.html, depois de criados vamos seguir todo o processo para enviar este arquivo para o github.

[Saiba mais...](praticando.md)

## Sites para praticar

https://ohmygit.org

https://learngitbranching.js.org


## Contribuições

Contribuições são sempre bem-vindas! 

Se você gostaria de ajudar a melhorar este projeto, siga as etapas abaixo:

1. **Fork o repositório**:
   - Clique no botão **Fork** no canto superior direito da página do repositório no GitHub.
   - Isso criará uma cópia do repositório na sua conta do GitHub.

2. **Clone o repositório**:
   - Clone seu repositório forkado para sua máquina local:
     ```bash
     git clone https://github.com/seu-usuario/nome-do-repositorio.git
     ```
   - Substitua `seu-usuario` pelo seu nome de usuário no GitHub e `nome-do-repositorio` pelo nome do repositório.

3. **Crie uma nova branch**:
   - Navegue até o diretório do projeto:
     ```bash
     cd nome-do-repositorio
     ```
   - Crie uma nova branch para suas alterações:
     ```bash
     git checkout -b minha-nova-feature
     ```

4. **Faça suas alterações**:
   - Realize as alterações necessárias no código ou na documentação.

5. **Adicione e faça commit das suas alterações**:
   - Adicione as alterações ao índice:
     ```bash
     git add .
     ```
   - Faça um commit com uma mensagem descritiva:
     ```bash
     git commit -m "Descrição clara da alteração"
     ```

6. **Envie suas alterações para o GitHub**:
   - Envie sua branch para o repositório forkado:
     ```bash
     git push origin minha-nova-feature
     ```

7. **Crie um Pull Request**:
   - Vá até o repositório original no GitHub.
   - Você verá uma opção para **Comparar & Pull Request**. Clique nela.
   - Adicione uma descrição do que você alterou e clique em **Criar Pull Request**.

8. **Aguarde a revisão**:
   - Seu Pull Request será revisado. Esteja aberto a feedbacks e sugestões!

**Agradecemos suas contribuições!**
