# Merge

O merge é realizado após o Pull Request (PR) ser revisado e aprovado.

O **merge** no Git é o processo de combinar duas branches (ou mais) em uma única. Quando você realiza um merge, você está pegando as alterações feitas em uma branch e as integrando com outra. Isso é frequentemente usado para juntar uma branch de desenvolvimento com a branch principal (geralmente chamada de `main` ou `master`), após a conclusão de uma funcionalidade ou correção de bug.

### Como funciona o **merge**?

1. **Você tem duas branches**: uma com alterações (por exemplo, uma branch de funcionalidade) e outra, a branch principal (`main`), que contém o código estável.
   
2. **Fazendo o merge**: Quando você faz um merge, o Git tenta combinar as alterações feitas nas duas branches. Se as alterações não se sobrepuserem, o merge é feito automaticamente, e as mudanças de ambas as branches são combinadas na branch de destino.

### Exemplo de Merge

Suponha que você tenha duas branches:

- `main`: a branch principal com o código estável.
- `nova-funcionalidade`: uma branch onde você está trabalhando em uma nova funcionalidade.

O fluxo de trabalho seria:

1. Primeiro, você muda para a branch onde você quer integrar as alterações. Normalmente, você faz o merge na branch `main`:
   ```bash
   git checkout main
   ```

2. Agora, você faz o merge da branch `nova-funcionalidade` na branch `main`:
   ```bash
   git merge nova-funcionalidade
   ```

Neste ponto, o Git tentará combinar as mudanças da `nova-funcionalidade` com a `main`. Se não houver conflitos (ou seja, se as alterações não afetarem as mesmas linhas de código), o merge será feito automaticamente, criando um novo commit na branch `main` que contém as mudanças combinadas.

### Quando ocorre um **conflito de merge**?

Se as alterações nas duas branches forem conflitantes (por exemplo, se você modificou a mesma linha de código em ambas as branches), o Git não consegue fazer o merge automaticamente e marcará esse conflito para que você resolva manualmente.

Nesses casos, o Git vai:
1. Identificar o conflito nos arquivos afetados.
2. Marcar essas partes no código com indicadores de conflito (`<<<<<<<`, `=======`, `>>>>>>>`).
   
Você precisa então editar os arquivos, escolher quais alterações manter, e depois fazer um novo commit para finalizar o merge.

### Como resolver um conflito de merge?

1. **Identificar o conflito**: O Git marca o local do conflito no arquivo.
2. **Editar o arquivo**: Você precisa abrir o arquivo e decidir qual código manter. Por exemplo:
   ```plaintext
   <<<<<<< HEAD
   Código da branch principal (main)
   =======
   Código da branch que você está tentando mesclar (nova-funcionalidade)
   >>>>>>> nova-funcionalidade
   ```
3. **Remover os marcadores de conflito** e escolher a versão correta do código.
4. **Adicionar e fazer commit** das alterações para resolver o conflito:
   ```bash
   git add arquivo_com_conflito
   git commit -m "Resolve conflito de merge"
   ```

### Benefícios do Merge

- **Colaboração**: Ele permite que múltiplos desenvolvedores trabalhem em diferentes partes de um projeto sem interferir diretamente no trabalho um do outro.
- **Histórico claro**: O merge mantém o histórico de commits intacto, o que é útil para rastrear o progresso e as alterações feitas ao longo do tempo.

### Resumo:
- **Merge** é o processo de integrar alterações de uma branch em outra.
- É usado para combinar alterações feitas em diferentes branches, sendo fundamental em projetos colaborativos.
- Pode ocorrer automaticamente ou exigir resolução de conflitos quando as alterações se sobrepõem.

Se precisar de mais detalhes sobre como realizar merges ou lidar com conflitos, só me avisar!