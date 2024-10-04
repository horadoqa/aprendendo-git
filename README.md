# Guia de Git e GitHub

Bem-vindo ao repositório "Git e GitHub"! 

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

[Saiba mais...](git.md)

## O que é GitHub?

GitHub é uma plataforma de hospedagem de código-fonte que utiliza Git. Ela permite que desenvolvedores colaborem em projetos, façam revisões de código e automatizem fluxos de trabalho de desenvolvimento através de funcionalidades como GitHub Actions.

[Saiba mais...](github.md)

## Instalação do Git

Para instalar o Git, siga estas etapas:

1. **Windows**: Baixe o instalador do [site oficial do Git](https://git-scm.com/download/win) e siga as instruções.

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

Sites pra testes:

- learngitbranching.js.org 
- https://ohmygit.org/

## Commits Semânticos

Commits semânticos, ou convenções de commits semânticos, referem-se a um padrão de nomenclatura para mensagens de commit que visa facilitar a compreensão do histórico de um projeto e melhorar a comunicação entre desenvolvedores. Esse padrão, conhecido como Conventional Commits, utiliza uma estrutura específica que ajuda a descrever claramente as mudanças realizadas no código.

[Saiba mais...](commits-semanticos.md)

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
