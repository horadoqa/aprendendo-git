# Pull Request (PR)

Como trabalhamos com muitos colaborados e alterações são constantes nos códigos, precisamos analisar essas alterações e aprovar ou não a atualização do `main`, para isso, precisaremos criar o famoso `Pull Request (PR)`.

Para criar um **Pull Request (PR)**, o processo geralmente envolve algumas etapas no GitHub (ou em plataformas similares como GitLab, Bitbucket, etc.), após você ter feito mudanças em um repositório. O Pull Request serve para pedir a revisão de suas alterações antes de mesclá-las com a branch principal do projeto (geralmente a `main` ou `master`). Vou te guiar pelas etapas em um repositório no GitHub.

### 1. **Faça as alterações no código e crie uma branch**
Primeiro, crie uma nova branch para suas alterações, assim você pode trabalhar sem afetar a branch principal (`main` ou `master`).

```bash
# No terminal, crie uma nova branch
git checkout -b minha-nova-funcionalidade

# Adicione suas mudanças (por exemplo, edite um arquivo)
git add .

# Faça o commit das alterações
git commit -m "Adiciona nova funcionalidade X"
```

### 2. **Envie suas alterações para o repositório remoto (GitHub)**
Depois de fazer o commit, você precisa enviar a branch para o repositório remoto.

```bash
# Envie a branch para o repositório remoto
git push origin minha-nova-funcionalidade
```

### 3. **Abra o GitHub e crie o Pull Request**
Agora que você enviou suas alterações para o repositório remoto, siga esses passos:

1. **Vá para o repositório no GitHub** onde você fez o `push` da sua branch.
   
2. Você verá um aviso logo acima da lista de arquivos que diz algo como "Your recently pushed branches: minha-nova-funcionalidade". Clique no botão **"Compare & pull request"**.

3. Na página seguinte, você verá uma comparação entre a sua branch e a branch principal (geralmente `main`). Aqui, você pode adicionar um título e uma descrição detalhada sobre o que foi feito na sua branch e o motivo das alterações.

4. Se tudo estiver correto, clique em **"Create Pull Request"**.

### 4. **Revisão do Pull Request**
Depois de criar o PR, ele ficará disponível para revisão. O time do projeto (ou você mesmo, se for um repositório pessoal) pode revisar suas alterações, discutir melhorias ou correções, e até mesmo sugerir ajustes.

- Se precisar fazer alterações, basta fazer commit na sua branch local e fazer um novo `push`. As mudanças serão automaticamente refletidas no PR.

### 5. **Mesclando o Pull Request**
Se as alterações forem aprovadas, o PR pode ser **mesclado** (merge) com a branch principal do projeto. Você pode fazer isso clicando no botão **"Merge pull request"** no GitHub.

---

### Resumo do Processo:

1. Crie uma nova branch (`git checkout -b minha-nova-funcionalidade`).
2. Faça suas alterações e commit (`git add .` e `git commit -m "mensagem"`).
3. Envie a branch para o repositório remoto (`git push origin minha-nova-funcionalidade`).
4. Vá para o GitHub e crie o Pull Request.
5. Acompanhe a revisão e, após aprovação, faça o merge.

O processo pode variar um pouco dependendo da plataforma (GitLab, Bitbucket, etc.), mas a ideia principal do Pull Request é sempre a mesma: sugerir alterações e permitir que outros revisem antes da fusão com a branch principal.

[Próximo passo... Mergeando as alterações](merge.md)