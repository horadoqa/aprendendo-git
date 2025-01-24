# Criando as chaves (Keys)

Para criar as chaves públicas e privadas para o GitHub, você pode usar o **ssh-keygen** no terminal do seu computador. Aqui está um passo a passo para gerar as chaves:

### 1. **Abrir o terminal**:
   - **No Linux ou macOS**, abra o terminal.
   - **No Windows**, você pode usar o Git Bash ou o terminal do PowerShell.

### 2. **Gerar a chave SSH**:
   No terminal, execute o seguinte comando:
   ```bash
   ssh-keygen -t rsa -b 4096 -C "seu_email@example.com"
   ```
   - O `-t rsa` especifica o tipo de chave (RSA).
   - O `-b 4096` define o tamanho da chave (4096 bits é recomendado para segurança).
   - O `-C "seu_email@example.com"` é um comentário que ajuda a identificar a chave, geralmente seu e-mail do GitHub.

### 3. **Escolher o local para salvar a chave**:
   Após executar o comando, ele perguntará onde salvar a chave gerada. Por padrão, a chave será salva no diretório `~/.ssh/id_rsa`. Caso queira usar o local padrão, basta pressionar **Enter**.

### 4. **Definir uma senha (opcional)**:
   O sistema pedirá para você criar uma senha para proteger sua chave privada. Essa etapa é opcional, mas recomendada para segurança adicional.

### 5. **Adicionar a chave pública ao GitHub**:
   Agora você precisa adicionar a chave pública gerada no GitHub:

   - Exiba a chave pública com o comando:
     ```bash
     cat ~/.ssh/id_rsa.pub
     ```
   - Copie todo o conteúdo da chave que aparecerá no terminal.

   - Vá até o GitHub e faça login.
   - No canto superior direito, clique na sua foto de perfil e depois em **Settings**.
   - No menu à esquerda, clique em **SSH and GPG keys**.
   - Clique em **New SSH key**.
   - No campo **Title**, coloque um nome para identificar essa chave, por exemplo, "Meu laptop".
   - No campo **Key**, cole a chave pública que você copiou.
   - Clique em **Add SSH key**.

### 6. **Testar a conexão SSH**:
   Para garantir que tudo está funcionando, você pode testar a conexão SSH com o GitHub:

   ```bash
   ssh -T git@github.com
   ```

   Se tudo estiver configurado corretamente, você verá uma mensagem como:
   ```
   Hi <username>! You've successfully authenticated, but GitHub does not provide shell access.
   ```

E pronto! Agora você tem uma chave SSH configurada para usar com o GitHub. Você pode usar o Git sem precisar inserir sua senha toda vez que fizer operações como `git push` ou `git pull`.


[Próximo passo... Enviar as modificações para o github](/docs/push.md)