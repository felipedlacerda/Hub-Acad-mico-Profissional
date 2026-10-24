# MATRIZ DE TESTES E QUALIDADE — PortfolioHUB

Este documento registra a bateria de testes funcionais, de navegação, responsividade e segurança executados no projeto.

---

## Matriz de Validação

| ID | Requisito / Funcionalidade | Procedimento de Teste | Resultado Esperado | Resultado Observado | Status | Evidência |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **TF-01** | Acesso ao GitHub Pages | Acessar ao link público do site | Página carrega sem erros 404 | Aprovado | Concluído | Print screen do browser |
| **TF-02** | Responsividade Mobile | Abrir o site em dispositivos móveis / Termux | Layout adapta-se corretamente | Aprovado | Concluído | Print screen mobile |
| **TF-03** | Validação de Links e Seções | Clicar em cada seção (Perfil, Projetos, Contato) | Navegação fluida pelas âncoras | Aprovado | Concluído | Registro de navegação |
| **TS-01** | Segurança de Repositório | Verificar ausência de segredos no GitHub | Histórico limpo sem tokens expostos | Aprovado | Concluído | `.gitignore` ativo |
| **TS-02** | Controle de Acessos | Validar restrições de branches e commits | Push restrito a colaboradores autorizados | Aprovado | Concluído | Registro de commits |
