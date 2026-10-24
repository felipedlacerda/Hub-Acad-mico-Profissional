# Política de Segurança — PortfolioHUB

## Versões suportadas
| Versão | Suporte |
|:--|:--|
| 1.x (main) | ✅ |

## Como reportar uma vulnerabilidade
Não abra issue pública. Use a aba **Security → Report a vulnerability** do repositório ou contate o mantenedor pelo LinkedIn. Resposta em até 7 dias.

## Práticas adotadas
- Autenticação em dois fatores (2FA) na conta do mantenedor
- Branch `main` protegida (sem force push e sem exclusão)
- Dependabot alerts e Secret Scanning com push protection ativos
- `.gitignore` bloqueando `.env`, `.pem` e `.key`
- Personal Access Tokens com escopo mínimo e prazo de expiração
- Commits assinados e verificados
