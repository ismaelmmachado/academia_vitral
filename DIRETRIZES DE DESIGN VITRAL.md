# DIRETRIZES DE DESIGN VITRAL — Academia de Ensino

> **Propósito:** Este é o documento único de referência para todas as decisões de design, arquitetura de interface e padrões visuais do portal da Academia de Ensino da Comunidade Vitral. Ele substitui e integra as informações anteriormente dispersas em `SPEC.md` e `REGRA DE OURO.md`.
>
> **Status:** Documento base para implementação. `SPEC.md` descreve o *o que* será criado; este documento define o *como* de design. `REGRA DE OURO.md` define os *porquê* e *para que*. Toda decisão de implementação deve ser conferida aos três documentos.

---

## 1. Visão Geral e Filosofia de UX

A Vitral fundamenta sua presença digital no conceito central de **Igreja em Pessoas**. O portal da Academia de Ensino deve ser um meio de conexão comunitária, acolhimento e crescimento espiritual, mantendo o tom humanizado e sem jargões definido na REGRA DE OURO.

### Princípios Fundamentais de Design

| Princípio | Descrição | Aplicação no Portal da Academia |
|-----------|-----------|--------------------------------|
| **Acolhimento Centrado no Humano** | A interface deve transmitir calor, clareza e transparência. Cada elemento visual visa reduzir atritos e criar um ambiente acolhedor. | Linguagem convidativa em todos os textos; botões e links que se sentem como convites, não exigências; estrutura que faz o usuário se sentir bem-vindo exatamente como está. |
| **Aparência Luz e Translúcida** | Inspirada na estética dos vitrais, a interface utiliza transparências suaves, camadas de luz e bordas sutis para expressar clareza e conexão espiritual. | Fundo de cards com `rgba(255, 255, 255, 0.85)` e `backdrop-filter: blur(10px)`; paleta que reflete luz e renovação. |
| **Simplicidade e Propósito** | Evitamos ruídos visuais. Todo componente interativo possui uma função clara para guiar o usuário com serenidade. | Cada card, link e botão tem propósito definido no checklist da REGRA DE OURO; sem funcionalidades secundárias que desviem do foco no discipulado. |
| **Comunidade e Pertencimento** | A experiência digital facilita a transição orgânica entre o ambiente online e a convivência comunitária presencial. | Cards que mostram conexão com grupos de células/ministérios; linguagem que incentiva participação presencial; links para oportunidades de serviço que conectam o online ao offline. |

---

## 2. Guia de Cores

A paleta de cores reflete estabilidade, renovação, clareza e elegância. **Prioriza-se o contraste acessível** (WCAG 2.1 AA) e o equilíbrio visual.

| Papel da Cor | Nome da Cor | Hexadecimal | Uso Principal | Exemplos no Portal |
|--------------|-------------|-------------|---------------|-------------------|
| **Primária** | Deep Teal | `#005F6B` | Identidade principal, headers, botões primários e destaques | Botão "Começar uma Trilha", headers de seção |
| **Secundária** | Sage Green | `#94A69A` | Elementos de apoio, badges, estados desabilitados e divisores sutis | Badges de nível, divisores entre cards, estado "disabled" |
| **Neutro Escuro** | Charcoal | `#1F2421` | Textos principais, títulos, ícones de alto contraste e superfícies escuras | Texto dos cards, títulos de seção |
| **Neutro Claro** | Pure White | `#FFFFFF` | Fundos de cards, texto sobre fundos escuros e áreas de respiro | Fundo dos cards de trilha, área de hero |
| **Superfície Suave** | Light Sage Tint | `#F2F5F3` | Fundos alternativos de seções e áreas de hover leve | Background alternado de seções, efeito hover em botões |

### Regras de Uso

- **Contraste mínimo:** Texto principal `#1F2421` sobre fundo claro `#FFFFFF` ou `#F2F5F3` cumprem taxa de 4.5:1 (WCAG AA). Texto `#FFFFFF` sobre `#005F6B` cumprem taxa de 7:1.
- **Áreas de toque no mobile:** Todos os elementos interativos possuem área mínima de 48×48dp.
- **Não usar** cores fora da paleta oficial sem justificativa documentada.

---

## 3. Tipografia e Escala Responsiva

Utilizamos a família tipográfica **Inter**, devido à sua alta legibilidade em telas pequenas e versatilidade em interfaces modernas. Essa escolha substitui a anterior menção a Montserrat no SPEC.md (a qual este documento serve como referência unificada).

### Escala Tipográfica (Minor Second)

| Nível | Desktop (pt) | Mobile (pt) | Peso | Aplicação |
|-------|-------------|-------------|------|-----------|
| **Display / Title** | 24 | 20 | **Bold** | Títulos de landing pages e telas principais |
| **Heading 1** | 16 | 15 | **Bold** | Títulos de seções de alto nível |
| **Heading 2** | 13 | 12.5 | **Bold** | Subseções e títulos de cards |
| **Heading 3** | 11 | 11 | **Bold** | Títulos de tabelas, modais e chamadas menores |
| **Body (Normal Text)** | 11 | 11 | **Regular** | Texto corrido, descrições e formulários |
| **Small / Caption** | 9.5 | 9.5 | **Regular / Medium** | Legendas, metadados e notas de rodapé |

### Aplicação no Portal

- Todos os textos da plataforma seguem esta escala.
- Nenhum texto deve ficar abaixo de 9.5pt em mobile ou 11pt em desktop.
- Títulos de cards de trilha usam Heading 2/Heading 3.
- Descrições e textos de apoio usam Body Regular.

---

## 4. Arquitetura de Informação (Academia de Ensino)

A estrutura de conteúdo é organizada para acesso rápido e intuitivo às trilhas de formação, seguindo o fluxo do discipulado.

### Principais Seções

1. **Início (Home):** Apresentação da academia com convite acolhedor para começar a jornada; opções para explorar trilhas; destaque para próxima etapa da jornada do discipulado.
2. **Trilhas:** Grid de cards responsivo apresentando todas as trilhas disponíveis (Trilha de Novos, Trilha Praticando o Caminho, Trilha de Liderança, Panorama Bíblico, Dashboard de Estações). Cada card inclui:
   - Título da trilha
   - Ícone/identificação visual
   - Duração (número de encontros/passos)
   - Público-alvo
   - Descrição focando como ajuda no crescimento espiritual e serviço
   - Chamada para ação ("Começar", "Acessar")
3. **Recursos:** Links diretos para conteúdo original nos repositórios fonte da Comunidade Vitral.
4. **Sobre:** Informações sobre a Academia de Ensino da Comunidade Vitral e o jeito Vitral de criar plataformas.

### Fluxo Lógico

Do primeiro acesso ao término de um módulo, há um fluxo lógico de aprendizado e crescimento, começando no acolhimento e terminando no envio (convite para aplicar o aprendizado).

---

## 5. Abordagem Mobile-First e Navegação

Com mais de 80% dos acessos oriundos de dispositivos móveis, o design prioriza a experiência touch e a navegação ao alcance do polegar (thumb zone).

### Padrões de Navegação

| Padrão | Descrição | Implementação no Portal |
|--------|-----------|------------------------|
| **Bottom Navigation Bar (Mobile)** | Acesso fixo e imediato às seções principais na parte inferior da tela. | 5 itens fixos: Início, Trilhas, Recursos, Sobre, Perfil. Cores: fundo transparente com texto `#1F2421`, estado ativo em `#005F6B`. |
| **Top Bar Enxuta** | Contém o logotipo Vitral, seletor de perfil e ícone de notificações. | Always visible na parte superior; logotipo com altura adequada; ícone de notificações com badge de contagem opcional. |
| **Navegação Desktop** | Header superior fixo com menu horizontal expansível e botão de ação em destaque (CTA). | Header fixo topo da tela; menu com links principais; CTA principal em `#005F6B` com texto `#FFFFFF`. |

### Menu Mobile Details

- Itens da bottom navigation com rótulos de texto + ícone.
- Item ativo: cor `#005F6B` + leve efeito de escala.
- Items inativos: opacidade reduzida 0.6.
- Toque em qualquer item rola para o conteúdo correspondente.

---

## 6. Componentes de Interface (UI Components)

### Botões

| Tipo | Fundo | Texto | Borda | Cantos | Uso |
|------|-------|-------|-------|--------|-----|
| **Primário** | `#005F6B` | `#FFFFFF` | Nenhum (sólido) | 8px | Ações principais: "Começar uma Trilha", "Inscrever-se" |
| **Secundário** | Transparente | `#005F6B` | 1px `#005F6B` | 8px | Ações secundárias: "Saiba mais", "Ver detalhes" |
| **Sutil / Ghost** | Transparente | `#1F2421` ou `#005F6B` | Nenhum | 8px | Links e ações neutras: "Leia também", "Voltar" |

### Efeitos

- **Hover em botões:** Transição suave de cor de fundo em 200ms. Botão primário: `#005F6B` → `#004B54`. Botão secundário: borda mais grossa ou opacidade alterada.
- **Feedback de clique/toque:** Redução leve de escala `scale(0.98)` para indicar pressão tátil no mobile.
- **Estado disabled:** Opacidade 0.4 + cursor `not-allowed`.

### Cards e Contêineres

| Tipo | Fundo | Borda | Sombra | Uso |
|------|-------|-------|--------|-----|
| **Card Elevação Suave** | `#FFFFFF` | 1px `#E5E9E6` | `0px 2px 8px rgba(0,0,0,0.04)` | Cards de trilha, cards de conteúdo |
| **Card Translúcido (Glassmorphism)** | `rgba(255, 255, 255, 0.85)` com `backdrop-filter: blur(10px)` | 1px `#E5E9E6` | — | Seções de destaque, áreas de chamada |
| **Superfície de Foco** | `#F2F5F3` | Nenhum | — | Fundo de hover em botões, estados ativos |

---

## 7. Microinterações e Feedbacks Visuais

As microinterações garantem que a interface responda de maneira fluida e previsível às ações do usuário.

### Hover em Botões

- Transição cor `200ms` facilidade.
- Botão primário: `#005F6B` → `#004B54`.
- Botão secundário: aumento de opacidade da borda ou mudança de cor.
- Manter a proporção e não alterar layout.

### Feedback de Clique/Toque

- Redução de escala `scale(0.98)` por 150ms.
- Confirm visual de que a ação foi registrada.

### Carregamento (Skeletons)

- Uso de blocos animados em `#F2F5F3` durante o carregamento de dados em vez de spinners genéricos.
- Skeletons têm a mesma forma do conteúdo que será carregado (cards, texto, imagens).
- Animação CSS `transition: opacity 1.5s ease-in-out`.

### Transições de Tela

- **Mobile:** Deslizamento suave (`slide-in`) entre seções/grades.
- **Desktop:** Esmaecimento (`fade-in`) para transições entre estados.

---

## 8. Diretrizes de Usabilidade e Acessibilidade (WCAG 2.1 AA)

A inclusão digital é um compromisso da Vitral para garantir que todos tenham acesso irrestrito ao conteúdo.

### Requisitos Técnicos

| Requisito | Especificação | Como atender no portal |
|-----------|--------------|------------------------|
| **Contraste de Cor** | Todos os textos principais `#1F2421` sobre fundos claros `#FFFFFF` e `#F2F5F3` cumprem taxa mínima 4.5:1. Textos `#FFFFFF` sobre `#005F6B` cumprem 7:1. | Sistema de cores acima garante conformidade. Verificar manualmente ferramenta de contraste em todos os estados (normal, hover, ativo, disabled). |
| **Áreas de Toque** | Todos os elementos interativos no mobile possuem área mínima de toque de 48×48dp. | Botões, links e áreas de clique nos cards têm padding mínimo equivalente a 48dp. |
| **Navegação por Teclado** | Foco visível com anel de destaque em `#005F6B` para navegação sem mouse. | Outline CSS `:focus` com `box-shadow: 0 0 0 2px #005F6B` ou `outline: 2px solid #005F6B`. |
| **Leitores de Tela** | Uso rigoroso de marcação semântica HTML (`main`, `nav`, `article`, `header`). Atributos `aria-label` em botões de ícones. Descrições `alt` completas em todas as imagens. | - Estrutura HTML5 semântica em todas as páginas.<br>- `aria-label="Fechar"` em botões de fechamento modais.<br>- `aria-label="Trilha de Novos"` em cards de trilha.<br>- `alt="Capa da Trilha de Novos: identidade em Cristo e pertencimento"` em imagens de capas. |
| **Texto Alternativo** | Todas as imagens têm descrição alt completa e significativa. | Padrão: `alt="[Descrição do conteúdo]: [contexto visual]"` |

### Acessibilidade Adicional

- **Redução de movimento:** Para usuários que ativam a preferência do sistema `prefers-reduced-motion`, microinterações devem ser desativadas ou reduzidas a transições instantâneas.
- **Tamanho de fonte escalável:** O texto deve permanecer legível quando o usuário aumenta o tamanho do texto do navegador até 200%.
- **Ordem de foco:** A ordem tabular segue a ordem visual lógica, começando pelo header, poição para o conteúdo principal, poição para a bottom navigation (no mobile).

---

## 9. Alinhamento com a REGRA DE OURO

Cada diretriz de design abaixo tem um mapeamento explícito aos critérios da REGRA DE OURO, para que decisões visuais sejam sempre justificadas pelos valores espirituais.

| Diretriz de Design | Critério da REGRA DE OURO | Como se conecta |
|--------------------|--------------------------|-----------------|
| **Paleta Deep Teal `#005F6B`** | **ACOLHEDOR** — transmite calor e conexão espiritual. | A cor "Deep Teal" remete à profundidade espiritual e ao "vitral" que deixa a luz passar. |
| **Paleta Sage Green `#94A69A`** | **MISSIONAL** — conecta ao mundo real e serviço. | Verde-sálvia simboliza renovação e crescimento, apontando para aplicação prática. |
| **Bottom Navigation Mobile** | **SIMPLES** — reduz cliques para acessar conteúdo principal. | 5 itens fixos na bottom dão acesso direto às principais seções com um toque. |
| **Tipografia Inter** | **SEM JARGÕES** — alta legibilidade acessível a todos. | Fonte sem serifa moderna, clara, sem ornamentos que dificultem a leitura. |
| **Cards Glassmorphism** | **Aparência Luz e Translúcida** — expressa clareza e conexão. | Efeito de transparência lembra vitral, passando a ideia de que a verdade passa através. |
| **Skeletons em `#F2F5F3`** | **FLUIDEZ** — experiência natural sem atritos. | Blocos animados indicam que algo está acontecendo sem quebrar o fluxo visual. |
| **Contraste WCAG 2.1 AA** | **ACOLHEDOR** — plataforma não cria barreiras. | Garante que pessoas com deficiência visual ou cognitiva possam usar a plataforma. |
| **Microinterações** | **FLUIDEZ** — experiência natural e sem atritos. | Transições suaves tornam a navegação prazerosa, não mecânica. |
| **Foco Visível `#005F6B`** | **ACESSIBILIDADE** — usado criteriosamente. | Anel de foco em Deep Teal cumpre requisito técnico sendo também consistente visualmente. |

> **Nota:** Sempre que houver dúvida sobre uma decisão de design, pergunte-se: *"Isso apoia algum dos critérios da REGRA DE OURO? Simples? Missional? Acolhedor?"*. Se a resposta for não, reavaliar a decisão.

---

## 10. Relacionamento com SPEC.md e REGRA DE OURO.md

### Como este documento se conecta ao ecossistema

| Documento | Função | Relação |
|-----------|--------|---------|
| **DIRETRIZES DE DESIGN VITRAL.md** (este documento) | **Padrões de design** | Define *como* a interface deve parecer e comportar. Fonte Inter, cores oficiais, componentes, microinterações, acessibilidade. |
| **SPEC.md** | **O que será criado** | Descreve a estrutura de páginas, trilhas, componentes lógicos, user stories, requisitos funcionais. Implementa as decisões de design deste documento. |
| **REGRA DE OURO.md** | **Por que e para que** | Define os valores (Simples, Missional, Acolhedor, Reformado, Protestante, Presbiteriano), teologia, linguagem e propósito do discipulado. Todas as decisões de design deste documento devem ser justificadas à luz destes valores. |

### Fluxo de Decisão Recomendado

1. **Definir propósito:** Ler `REGRA DE OURO.md` para entender o "porquê" e "para que".
2. **Definir estrutura:** LER `SPEC.md` para entender o "o quê" (qué features, páginas, fluxos).
3. **Aplicar design:** Consultar **este documento** (DIRETRIZES DE DESIGN VITRAL.md) para decisões de cor, tipografia, componentes, microinterações e acessibilidade.
4. **Verificar consistência:** Garantir que cada escolha de design esteja alinhada aos critérios da REGRA DE OURO (via a Tabela da Seção 9).
5. **Implementar:** Desenvolvedores seguem o SPEC.md, mas dão atenção aos valores visuais e comportamentais definidos neste documento de design.

---

## 11. Histórico de Revisões

| Data | Versão | Autor | Mudanças |
|------|--------|-------|----------|
| Out/2026 | 1.0 | Equipe Academia Vitral | Documento inicial. Consolidou Manual Vitral, adaptou para Academia e adicionou alinhamento com REGRA DE OURO e SPEC.md. |
| — | — | — | — |

---