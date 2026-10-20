# GUIA DE CONTRIBUIÇÃO E GOVERNANÇA — PortfolioHUB

Agradecemos o interesse em contribuir para o **PortfolioHUB**. Este documento estabelece as diretrizes de desenvolvimento, segurança e padronização.

---

## 1. Fluxo de Trabalho e Branches
- **`main`**: Branch de produção vinculada ao GitHub Pages. Alterações diretas são restritas.
- **`feature/*` ou `fix/*`**: Branches para novas funcionalidades ou correções.
- Toda alteração deve ser submetida via **Pull Request (PR)**.

---

## 2. Padronização de Commits (Conventional Commits)
Os commits devem seguir o formato:
`<tipo>(<escopo>): <descrição sucinta>`

Tipos permitidos:
- `feat`: Nova funcionalidade no PortfolioHUB.
- `fix`: Correção de bugs ou ajustes visuais.
- `docs`: Alterações na documentação.
- `chore`: Tarefas de manutenção e infraestrutura.
- `security`: Ajustes de segurança e DevSecOps.

---

## 3. Segurança e Gestão de Segredos
- **Proibição Absoluta**: NUNCA envie tokens de acesso, chaves privadas (`.pem`, `.key`) ou credenciais no histórico do Git.
- Todos os contribuidores devem manter o ficheiro `.gitignore` atualizado.
- Autenticação obrigatória via Personal Access Token (PAT) ou chaves SSH com MFA ativo na conta GitHub.

---

## 4. Revisão de Código e Aceitação
- Todo Pull Request necessita de validação dos critérios de aceitação e testes de regressão antes do *merge*.
