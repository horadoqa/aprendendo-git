Se a ideia é **converter o texto para explicar o GitHub**, mantendo a mesma estrutura:

# `github`

site: [https://github.com/](https://github.com/)

O **GitHub** é uma plataforma de hospedagem e colaboração para projetos de software.

Ele utiliza o **Git** para controle de versão e oferece recursos como:

* Repositórios Git
* Branches
* Commits
* Pull Requests
* Revisão de código
* Issues
* GitHub Actions
* Pipelines de automação
* Controle de permissões

### GitHub

```text
flowchart TD
    A["feature/login"] --> B["Pull Request"]
    B --> C["main"]
```

O **Pull Request** permite solicitar a revisão e a integração das alterações de uma branch em outra.

Os comandos Git continuam sendo:

```bash
git add .
git commit -m "Adiciona login"
git push
```

O Git é a ferramenta de controle de versão; o **GitHub é uma plataforma que hospeda repositórios Git e adiciona recursos de colaboração, revisão de código e automação**.

### Principais recursos

| Recurso           | GitHub              |
| ----------------- | ------------------- |
| Repositórios Git  | GitHub Repositories |
| Branches          | Branches            |
| Commits           | Commits             |
| Pull Request      | Pull Request        |
| GitHub Actions    | CI/CD e automação   |
| Issues            | Issues              |
| GitHub Projects   | Projects            |
| GitHub Codespaces | Codespaces          |

Uma diferença importante na terminologia é que, no GitHub, utilizamos **Pull Request (PR)** para propor a integração das alterações:

```text
flowchart TD
    A["feature/login"] --> B["Pull Request"]
    B --> C["main"]
```

Apesar de o GitHub possuir seus próprios recursos, os comandos básicos do Git permanecem os mesmos.

```bash
git add .
git commit -m "Adiciona login"
git push
```

**Git e GitHub não são a mesma coisa:** o Git é o sistema de controle de versão, enquanto o GitHub é uma plataforma que hospeda repositórios Git e oferece ferramentas para colaboração e desenvolvimento de software.
