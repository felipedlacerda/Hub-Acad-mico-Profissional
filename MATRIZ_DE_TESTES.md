# MATRIZ DE TESTES E QUALIDADE — PortfolioHUB

Este documento regista a bateria de testes funcionais, de navegação, responsividade e segurança executados no projeto.

---

## Matriz de Validação

| ID | Requisito / Funcionalidade | Procedimento de Teste | Resultado Esperado | Resultado Observado | Status | Evidência |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **TF-01** | Acesso ao GitHub Pages | Aceder ao link público do site | Página carrega sem erros 404 | Em validação | Pendente | Print screen do browser |
| **TF-02** | Responsividade Mobile | Abrir o site em dispositivos móveis / Termux | Layout adapta-se corretamente | Em validação | Pendente | Print screen mobile |
| **TF-03** | Validação de Links e Seções | Clicar em cada secção (Perfil, Projetos, Contato) | Navegação fluida pelas âncoras | Em validação | Pendente | Registo de navegação |
| **TS-01** | Segurança de Repositório | Verificar ausência de segredos no GitHub | Histórico limpo sem tokens expostos | Aprovado | Concluído | `.gitignore` ativo |
| **TS-02** | Controlo de Acessos | Validar restrições de branches e commits | Push restrito a colaboradores autorizados | Aprovado | Concluído | Registo de commits |
