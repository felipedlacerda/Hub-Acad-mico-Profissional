<div align="center">

# POUPI

### Planejamento e acompanhamento financeiro

**Projeto acadêmico de Engenharia de Software**

Centro Universitário de Brasília — CEUB

Design de Interfaces · Engenharia de Requisitos · Prototipação

**Status: Em desenvolvimento**

</div>

---

## 01 — Apresentação

<p align="justify">
O <strong>Poupi</strong> é um projeto acadêmico de aplicativo voltado à organização financeira pessoal, concebido para permitir o registro de receitas e despesas, o acompanhamento de saldos e a análise da distribuição dos gastos por grupos.
</p>

<p align="justify">
A proposta contempla o desenvolvimento progressivo de uma interface para dispositivos móveis, estruturada a partir de requisitos funcionais, princípios de usabilidade e componentes visuais reutilizáveis. O processo de concepção utiliza o Figma para a elaboração do sistema de design, dos wireframes e do protótipo navegável.
</p>

<p align="justify">
O projeto encontra-se em fase de desenvolvimento. As funcionalidades descritas neste documento constituem o escopo previsto para a primeira etapa, não representando necessariamente recursos implementados em código.
</p>

---

## 02 — Problema e objetivos

### 02.1 — Contextualização

<p align="justify">
O acompanhamento das finanças pessoais exige a organização de diferentes informações, incluindo entradas, saídas, recorrência de transações e distribuição das despesas. A fragmentação desses registros pode dificultar a compreensão do saldo disponível e a identificação dos principais componentes do orçamento.
</p>

<p align="justify">
O Poupi propõe reunir essas informações em uma interface única, com navegação simplificada e representação visual dos dados financeiros.
</p>

### 02.2 — Objetivo geral

Desenvolver o projeto de interface de um aplicativo móvel para registro, organização e acompanhamento de informações financeiras pessoais.

### 02.3 — Objetivos específicos

1. Estruturar o registro de receitas e despesas.
2. Permitir a classificação das transações por grupos.
3. Apresentar o saldo financeiro e o resumo mensal.
4. Organizar informações por meio de relatórios visuais.
5. Desenvolver componentes de interface padronizados e reutilizáveis.

---

## 03 — Escopo funcional

<p align="justify">
O escopo inicial está organizado em seis telas principais, previstas para o primeiro ciclo de desenvolvimento. A estrutura contempla operações de registro financeiro, classificação de despesas e visualização consolidada das informações.
</p>

| Identificação | Tela | Finalidade |
|:---:|:---|:---|
| 01 | Home | Visão geral do saldo e movimentações |
| 02 | Nova Receita | Registro de entradas financeiras |
| 03 | Nova Despesa | Registro de saídas financeiras |
| 04 | Grupos | Organização das despesas por categoria |
| 05 | Editar Grupo | Atualização das informações de um grupo |
| 06 | Relatórios | Apresentação de indicadores financeiros |

### 03.1 — Requisitos funcionais previstos

| Código | Requisito |
|:---:|:---|
| RF01 | Registrar receitas financeiras |
| RF02 | Registrar despesas financeiras |
| RF03 | Identificar transações recorrentes e não recorrentes |
| RF04 | Associar despesas a grupos |
| RF05 | Criar e editar grupos de despesas |
| RF06 | Definir limites financeiros por grupo |
| RF07 | Apresentar o saldo disponível |
| RF08 | Exibir receitas e despesas do período |
| RF09 | Apresentar relatórios e gráficos |
| RF10 | Permitir navegação entre as telas principais |

### 03.2 — Requisitos não funcionais propostos

| Código | Requisito |
|:---:|:---|
| RNF01 | Interface adaptada a dispositivos móveis |
| RNF02 | Consistência tipográfica e cromática |
| RNF03 | Componentes visuais reutilizáveis |
| RNF04 | Organização padronizada dos espaçamentos |
| RNF05 | Hierarquia visual clara |
| RNF06 | Navegação compreensível entre as telas |
| RNF07 | Legibilidade e contraste adequados |
| RNF08 | Facilidade de manutenção do sistema visual |

<p align="justify">
Os requisitos não funcionais apresentados constituem diretrizes de projeto. Sua validação dependerá de critérios mensuráveis e de testes realizados durante o desenvolvimento.
</p>

---

## 04 — Metodologia de desenvolvimento

<p align="justify">
O processo de concepção da interface está dividido em quatro etapas sequenciais, permitindo estabelecer as regras visuais antes da construção das telas definitivas.
</p>

| Etapa | Atividade | Resultado esperado |
|:---:|:---|:---|
| 01 | Design System | Definição de cores, tipografia e componentes |
| 02 | Wireframes | Estruturação das telas e da navegação |
| 03 | Interface final | Aplicação do sistema visual |
| 04 | Prototype | Protótipo navegável no Figma |

### 04.1 — Organização do Figma

O arquivo de design será organizado em três páginas:

```text
POUPI — FIGMA
│
├── Design System
│   ├── 01 — Cores
│   ├── 02 — Tipografia
│   ├── 03 — Spacing
│   └── 04 — Components
│
├── Wireframes
│   ├── 01 — Home
│   ├── 02 — Nova Receita
│   ├── 03 — Nova Despesa
│   ├── 04 — Grupos
│   ├── 05 — Editar Grupo
│   └── 06 — Relatórios
│
└── Poupi App
    ├── Telas finais
    ├── Componentes aplicados
    └── Conexões de prototipação
```

<p align="justify">
Essa divisão separa a definição dos elementos visuais, o planejamento estrutural das telas e a apresentação final da interface. As interações serão configuradas no modo Prototype, utilizando as telas da página Poupi App.
</p>

---

## 05 — Design System

### 05.1 — Identidade cromática

<p align="justify">
A identidade visual utiliza o verde como cor principal, associado a tons neutros para superfícies e textos. A diferenciação cromática entre receitas, despesas e estados de alerta procura facilitar a interpretação das informações financeiras.
</p>

| Token | Código hexadecimal | Aplicação |
|:---|:---:|:---|
| Primary | `#176B52` | Cor principal |
| Secondary | `#35A67A` | Destaques |
| Surface Green | `#EAF6F1` | Superfícies e cards claros |
| Background | `#F7F9F8` | Fundo das telas |
| Text | `#17211D` | Textos principais |
| Expense | `#D94C4C` | Despesas, erros e alertas |

<p align="justify">
A cor destinada às despesas e aos alertas não deverá ser utilizada indiscriminadamente em ações comuns, preservando a associação visual entre tonalidade e significado.
</p>

### 05.2 — Tipografia

A família tipográfica definida para o projeto é **Inter**.

| Elemento | Peso | Tamanho |
|:---|:---|---:|
| Valores financeiros em destaque | Bold | 34 px |
| Títulos e subtítulos principais | Semi Bold | 21 px |
| Informações secundárias | Regular | 13 px |

<p align="justify">
A hierarquia tipográfica busca estabelecer distinção entre valores financeiros, títulos e informações complementares, mantendo consistência entre as telas.
</p>

### 05.3 — Sistema de espaçamento

<p align="justify">
O projeto adota uma escala de espaçamentos inspirada na sequência de Fibonacci. A progressão é utilizada como referência para estabelecer relações proporcionais entre elementos, componentes e seções, sem comprometer requisitos de legibilidade e acessibilidade.
</p>

**Sequência de referência:**

`3 → 5 → 8 → 13 → 21 → 34 → 55 → 89`

| Espaçamento | Aplicação |
|:---:|:---|
| 8 px | Elementos de proximidade imediata |
| 13 px | Elementos relacionados |
| 21 px | Margens e preenchimentos principais |
| 34 px | Separação entre seções |
| 55 px | Separações amplas |
| 89 px | Elementos de destaque, quando aplicável |

### 05.4 — Componentes

<p align="justify">
A construção da interface prevê a utilização de componentes reutilizáveis no Figma, com propriedades padronizadas de cor, tipografia, espaçamento e geometria.
</p>

**Componente inicial: `Button / Primary`**

| Propriedade | Especificação |
|:---|:---|
| Cor de fundo | `#176B52` |
| Cor do texto | `#FFFFFF` |
| Padding horizontal | 21 px |
| Padding vertical | 13 px |
| Raio de borda | 13 px |
| Organização | Auto Layout |
| Tipologia | Componente reutilizável |

<p align="justify">
A utilização de componentes compartilhados busca reduzir divergências entre as telas e facilitar alterações globais durante a evolução do projeto.
</p>

---

## 06 — Wireframes e arquitetura de informação

### 06.1 — Padrão de dispositivo

A primeira versão dos wireframes utilizará uma área de referência de **360 × 800 px**, correspondente a um formato de tela móvel.

### 06.2 — Home

A tela inicial deverá apresentar:

- Identificação do aplicativo e acesso ao perfil.
- Mensagem de apresentação.
- Saldo disponível.
- Total de receitas e despesas.
- Ações para adicionar receita ou despesa.
- Resumo financeiro mensal.
- Gráfico de movimentações.
- Lista de grupos de despesas.
- Navegação inferior.

### 06.3 — Nova Receita

Campos previstos:

- Valor.
- Descrição.
- Tipo de recorrência.
- Data.
- Categoria.
- Ação para salvar.

### 06.4 — Nova Despesa

Campos previstos:

- Valor.
- Descrição.
- Tipo de recorrência.
- Grupo de despesa.
- Data.
- Ação para salvar.

### 06.5 — Grupos

A interface deverá permitir a consulta dos grupos financeiros e disponibilizar acesso à criação e edição de grupos.

### 06.6 — Editar Grupo

Campos previstos:

- Nome.
- Limite financeiro.
- Ícone de identificação.
- Ação para salvar alterações.

### 06.7 — Relatórios

A tela deverá apresentar:

- Receitas do período.
- Despesas do período.
- Saldo resultante.
- Comparação entre entradas e saídas.
- Distribuição percentual das despesas por grupo.

<p align="justify">
Os valores financeiros utilizados nos wireframes e protótipos são ilustrativos e destinam-se exclusivamente à representação visual dos componentes.
</p>

---

## 07 — Prototipação e navegação

<p align="justify">
A prototipação será realizada no Figma por meio de conexões entre elementos interativos e telas de destino, permitindo simular o fluxo de navegação antes da implementação funcional do aplicativo.
</p>

| Origem | Ação | Destino |
|:---|:---|:---|
| Home | Selecionar Receita | Nova Receita |
| Home | Selecionar Despesa | Nova Despesa |
| Home | Selecionar Grupos | Grupos |
| Grupos | Selecionar um grupo | Editar Grupo |
| Navegação inferior | Selecionar Relatórios | Relatórios |
| Telas secundárias | Selecionar Voltar | Tela anterior |

<p align="justify">
A navegação do protótipo não representa, por si só, persistência de dados ou execução de operações financeiras. Essas funcionalidades dependerão de implementação posterior.
</p>

---

## 08 — Planejamento e evolução

### 08.1 — Sprint 1

O escopo inicial compreende:

1. Estruturação do Design System.
2. Elaboração dos seis wireframes.
3. Construção das telas finais.
4. Configuração das conexões de navegação.
5. Revisão da consistência visual.
6. Documentação dos componentes e fluxos.

### 08.2 — Etapas posteriores

<p align="justify">
Após a conclusão e validação do protótipo, o projeto poderá avançar para a implementação das interfaces, definição da arquitetura de software, modelagem de dados, persistência das transações e testes funcionais.
</p>

<p align="justify">
Essas atividades constituem possibilidades de evolução e não devem ser interpretadas como funcionalidades já desenvolvidas.
</p>

---

## 09 — Organização e colaboração

<p align="justify">
O desenvolvimento colaborativo deverá seguir padrões compartilhados de nomenclatura, componentes e documentação. A definição centralizada dos elementos do Design System busca evitar inconsistências decorrentes de decisões visuais individuais.
</p>

**Fluxo de desenvolvimento adotado como referência:**

`Requisito → Wireframe → Design System → Interface → Protótipo → Implementação`

<p align="justify">
A participação dos integrantes poderá ser registrada por atividade, permitindo identificar responsabilidades relacionadas à definição de requisitos, construção de telas, revisão e documentação.
</p>

---

## 10 — Ferramentas

| Ferramenta | Aplicação |
|:---|:---|
| Figma | Design System, wireframes e prototipação |
| Git | Controle de versões dos arquivos versionados |
| GitHub | Organização e documentação do projeto |
| Markdown | Documentação técnica |

<p align="justify">
A plataforma e as tecnologias de implementação do aplicativo ainda deverão ser definidas conforme a evolução do projeto. O uso do Figma nesta etapa está relacionado à concepção e à prototipação da interface.
</p>

---

## 11 — Critérios de validação

<p align="justify">
A primeira etapa poderá ser considerada concluída quando os artefatos de design e prototipação estiverem disponíveis e apresentarem consistência com os requisitos estabelecidos.
</p>

- [ ] Design System estruturado.
- [ ] Paleta cromática documentada.
- [ ] Tipografia e espaçamentos definidos.
- [ ] Componentes reutilizáveis criados.
- [ ] Seis wireframes elaborados.
- [ ] Seis telas finais desenvolvidas.
- [ ] Navegação configurada no Prototype.
- [ ] Fluxos principais revisados.
- [ ] Documentação atualizada.

---

## 12 — Limitações e considerações técnicas

<p align="justify">
O projeto descrito neste documento corresponde à concepção de um aplicativo de organização financeira pessoal. A etapa de prototipação tem por objetivo validar a disposição dos elementos, a consistência da interface e os fluxos de navegação.
</p>

<p align="justify">
A implementação de operações financeiras, armazenamento de informações, autenticação, segurança de dados e geração dinâmica de relatórios dependerá de requisitos adicionais e de decisões arquiteturais específicas.
</p>

---

## 13 — Autoria e documentação

**Projeto:** Poupi  
**Natureza:** Projeto acadêmico  
**Área:** Engenharia de Software  
**Instituição:** Centro Universitário de Brasília — CEUB  
**Participação:** Projeto desenvolvido em contexto acadêmico colaborativo  
**Documentação:** Felipe de Lacerda Pereira

<p align="justify">
Este documento apresenta o delineamento funcional e visual do Poupi, reunindo as decisões iniciais de interface, os requisitos previstos e o planejamento de desenvolvimento. Seu conteúdo deverá ser atualizado à medida que os artefatos forem produzidos e validados.
</p>

---

<div align="center">

**POUPI**

Planejamento financeiro · Design de interfaces · Engenharia de Software

[Repositório principal](https://github.com/felipedlacerda/Hub-Acad-mico-Profissional) · [Projetos acadêmicos](https://github.com/felipedlacerda/Hub-Acad-mico-Profissional/tree/main/Hub-Academico-Profissional/04_Projetos_e_Pesquisa/Engenharia_de_Software)

</div>
