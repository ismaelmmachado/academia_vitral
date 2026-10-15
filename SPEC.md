## Problem Statement

A Comunidade Vitral possui diversos recursos de formação cristã distribuídos em repositórios GitHub separados (Trilha de Novos, Trilha Praticando o Caminho, Trilha de Liderança, Panorama Bíblico e um dashboard de estações), mas não há um ponto centralizado onde os membros da comunidade possam facilmente descobrir, navegar e acessar todo esse conteúdo formativo de forma organizada. Os membros enfrentam dificuldade para encontrar o conteúdo adequado ao seu estágio de jornada espiritual e perderiam tempo procurando pelos materiais em diferentes locais, o que pode dificultar seu crescimento como discípulos de Jesus que são chamados não apenas a conhecer a verdade, mas a vivê-la no serviço a Deus e ao próximo.

## Solution

Criar um portal web responsivo que sirva como academia de ensino centralizada da Comunidade Vitral, organizando e apresentando as trilhas de formação existentes em uma estrutura de navegação clara, permitindo que membros da comunidade explorem e acessem os recursos de formação de acordo com suas necessidades e estágio de crescimento espiritual, mantendo o conteúdo original intacto nos repositórios fonte. Esta plataforma não será apenas um repositório de informações, mas um instrumento para formar discípulos que conhecem Jesus, são transformados por Sua graça e são enviados para servir ao mundo com amor, ajudando cada pessoa a descobrir seu próximo passo obediente na jornada de discipulado.

## User Stories

1. Como um visitante novo na comunidade, quero ver uma visão geral do que a academia de ensino oferece, para que eu possa entender rapidamente as opções de formação disponíveis e começar minha jornada de descobrir quem sou em Cristo.
2. Como um membro da comunidade interessado em crescimento espiritual, quero navegar facilmente entre as diferentes trilhas de formação (Trilha de Novos, Trilha Praticando o Caminho, Trilha de Liderança), para que eu possa encontrar o conteúdo adequado ao meu estágio de fé e dar os próximos passos obedientes em minha caminhada com Jesus.
3. Como um líder ou aspirante a líder na comunidade, quero acessar rapidamente a Trilha de Liderança e recursos relacionados, para que eu possa desenvolver minhas habilidades de liderança servicial que edificam a comunidade, seguindo o exemplo de Jesus que veio para servir, não para ser servido.
4. Como alguém interessado em entender melhor as Escrituras, quero acessar o Panorama Bíblico de forma destacada no portal, para que eu possa estudar a Bíblia de forma sistemática e conhecer melhor a Jesus, o centro de toda a revelação de Deus.
5. Como um facilitador ou líder de grupo, quero acessar o Dashboard de Estaçõe para ver todas as trilhas disponíveis em um único lugar, para que eu possa orientar outros membros sobre quais trilhas fazer e ajudar cada pessoa a discernir onde Deus está trabalhando em sua vida.
6. Como um usuário em dispositivo móvel, quero que o portal seja responsivo e fácil de usar em meu smartphone ou tablet, para que eu possa acessar os conteúdos em qualquer lugar e continuar minha jornada de discipulado onde quer que eu esteja.
7. Como um membro da comunidade, quero identificar visualmente que este portal pertence à Comunidade Vitral através do uso da identidade visual existente, para que eu sinta confiança e pertencimento ao acessar os recursos que me ajudarão a crescer na graça e no conhecimento de Deus.
8. Como um visitante, quero ver descrições claras de cada trilha incluindo o número de encontros/módulos e o público-alvo, bem como como cada trilha me ajuda a crescer em minha relação com Jesus e em meu serviço ao próximo, para que eu possa escolher a trilha mais adequada às minhas necessidades espirituais atuais.
9. Como um usuário, quero acessar diretamente o conteúdo original nos repositórios fonte através de links claros no portal, para que eu tenha certeza de que estou acessando o material mais atualizado e autêntico que me apontará para a verdade de Deus em Cristo.
10. Como um membro menos experiente com tecnologia, quero uma interface simples e intuitiva que não requer login ou configuração complexa, para que eu possa começar a aprender imediatamente sem barreiras técnicas, sentindo-me bem-vindo exatamente como estou, confiando na graça de Deus que me capacita para crescer.
11. Como alguém que deseja aplicar o que aprende, quero encontrar sugestões práticas de como viver o conteúdo das trilhas no meu dia a dia, em meu serviço à comunidade e em meu relacionamento com os outros, para que meu conhecimento se transforme em obedência amorosa.
12. Como um líder de grupo pequeno, quero acessar recursos que me ajudem a facilitar discussões que levam à aplicação prática do aprendizado, para que o grupo inteiro possa crescer junto em discipulado frutífero.

## Scenarios

Given que o usuário acessa o portal da academia de ensino
Quando ele visita a página inicial
Então ele deve ver uma apresentação clara da academia com opções para explorar as trilhas de formação e um convite acolhedor para começar sua jornada de descoberta em Cristo

Given que o usuário está na página inicial
Quando ele clica no botão para explorar as trilhas
Então ele deve ser rolado para a seção que apresenta todas as trilhas disponíveis com descrições que destacam como cada uma ajuda no crescimento espiritual e no serviço

Given que o usuário está vendo a seção de trilhas
Quando ele observa o card da "Trilha de Novos"
Então ele deve ver que é para iniciantes, tem 9 encontros, uma descrição sobre identidade em Cristo e pertencimento à comunidade, e sugestões de como aplicar esse conhecimento no relacionamento com Deus e com os outros

Given que o usuário está vendo a seção de trilhas
Quando ele observa o card da "Trilha Praticando o Caminho"
Então ele deve ver que tem 17 passos divididos em 2 etapas, foca em práticas espirituais e serviço comunitário, e inclui exemplos práticos de como viver esses princípios no dia a dia

Given que o usuário está vendo a seção de trilhas
Quando ele observa o card da "Trilha de Liderança"
Então ele deve ver que tem 4 módulos e foca em desenvolvimento de liderança cristã com ênfase em serviço e gestão de pessoas que edifica, seguido por desafios de aplicação prática dessas habilidades

Given que o usuário está vendo a seção de trilhas
Quando ele observa o card do "Dashboard de Estações"
Então ele deve ver que é um portal integrado para navegar entre todas as trilhas e ajudar cada pessoa a discernir onde Deus está trabalhando em sua vida e quais próximos passos obedientes dar

Given que o usuário está vendo a seção de trilhas
Quando ele observa o card do "Panorama Bíblico"
Então ele deve ver que é uma série de vídeos para entender as Escrituras do Antigo ao Novo Testamento, centrada em Jesus Cristo, com sugestões de como essa compreensão transforma nossa vida e serviço

Given que o usuário está em um dispositivo móvel
Quando ele acessa o portal
Então o layout deve adaptar-se para tela menor com menu de navegação colapsável e cards ocupando toda a largura, mantendo a legibilidade e facilidade de uso para todas as idades e níveis de habilidade tecnológica

Given que o usuário clica em qualquer botão de "Começar", "Acessar" ou "Assistir" em um card de trilha
Então ele deve ser redirecionado para o conteúdo original desse recurso nos repositórios fonte da Comunidade Vitral, onde encontrará materiais bíblicos na Nova Versão Transformadora (NVT) e aplicações práticas do ensinamento

Given que o usuário completa um módulo ou trilha
Quando ele acessa o portal novamente
Então ele deve ver sugestões de próximos passos em sua jornada de discipulado, incluindo oportunidades de serviço e desafios de aplicação prática do que aprendeu

## Implementation Decisions

- **Abordagem Técnica**: Criar um portal web estático usando HTML/CSS/JS que serve como interface de navegação e agregação visual, com links diretos para o conteúdo existente nos repositórios GitHub da Comunidade Vitral
- **Arquitetura**: Aplicação de página única (SPA) simples ou múltiplas páginas estáticas vinculadas, dependendo da complexidade desejada para o MVP
- **Integração de Conteúdo**: Manter todo o conteúdo formativo nos repositórios existentes (trilha_de_novos, trilha_praticando_o_caminho, trilha_lideranca, panorama_biblico, trilhas_discipulado-v2) e criar links a partir do portal para esses recursos
- **Identidade Visual**: Usar as cores existentes da Comunidade Vitral (verde petróleo #005f6b, sálvia #94a69a). Seguir as Diretrizes de Design Vitral (`DIRETRIZES DE DESIGN VITRAL.md`) para tipografia (Inter), componentes, microinterações e acessibilidade, garantindo consistência com o ecossistema Vitral.
- **Responsividade**: Implementar layout responsivo usando CSS Flexbox/Grid que funcione em dispositivos móveis e desktop
- **Navegação**: 
  - **Mobile**: Bottom Navigation Bar com 5 itens fixos (Início, Trilhas, Recursos, Sobre, Perfil), cores Deep Teal `#005F6B` para ativo e Sage Green `#94A69A` para itens inativos. Área mínima de toque 48×48dp.
  - **Desktop**: Header superior fixo com menu horizontal expansível e botão de ação em destaque (CTA) em `#005F6B` com texto `#FFFFFF`.
  - **Padrão consistente**: Segue as Diretrizes de Design Vitral (`DIRETRIZES DE DESIGN VITRAL.md`) Seção 5, garantindo experiência touch e navegação ao alcance do polegar.
- **Apresentação de Trilhas**: Usar um grid de cards responsivo onde cada card representa uma trilha/módulo com ícone, título, descrição que inclui tanto o conteúdo quanto sugestões de aplicação prática, detalhes (duração, nível) e chamada para ação
- **Hospedagem**: Utilizar GitHub Pages para hospedar o portal, similarmente aos sites existentes da comunidade
- **Manutenção**: Implementar como um sistema híbrido onde a estrutura e navegação estão no portal, mas o conteúdo permanece nos repositórios fonte, permitindo atualizações independentes
- **Elementos Missionais**: Incluir nas descrições das trilhas e nas páginas de conteúdo links ou sugestões para oportunidades de serviço, desafios de aplicação prática e recursos para crescimento em relacionamento com Deus e com o próximo
- **Acolhimento**: Garantir que a linguagem usada em toda a plataforma seja acolhedora, convidativa e livre de jargões desnecessários, comunicando graça e aceitação

## Testing Decisions

- **Escopo dos Testes**: Testar o comportamento externo do portal através de testes de interface que verifiquem:
  - Renderização correta dos elementos principais (header, hero section, cards de trilhas, footer)
  - Funcionalidade do menu de navegação responsivo
  - Correção dos links para os repositórios fonte
  - Adaptação do layout em diferentes tamanhos de tela (mobile, tablet, desktop)
  - Presença de linguagem acolhedora e convidativa em todo conteúdo da plataforma
  - Inclusão de sugestões de aplicação prática ou elementos missionais nas descrições das trilhas
- **Abordagem de Testes**: Para o MVP inicial, testes manuais serão suficientes dada a natureza estática e simples do portal. Testes automatizados podem ser adicionados em fases posteriores se o projeto crescer em complexidade.
- **Qualidade de Testes**: Os testes devem focar no comportamento do usuário final (o que ele vê e pode fazer) e não em detalhes de implementação interna, incluindo a experiência emocional e espiritual de uso da plataforma.

## Out of Scope

- Sistema de autenticação de usuários ou login
- Rastreamento de progresso individual ou conquistas (para evitar transformar a fé em desempenho ou competição)
- Funcionalidade de busca por tópicos ou palavras-chave dentro do conteúdo
- Área de comentários, discussão ou interação social entre usuários (para manter o foco no conteúdo formativo e evitar distrações)
- Criação ou modificação do conteúdo formativo existente (todo o conteúdo permanecerá nos repositórios fonte)
- Funcionalidade de e-commerce, pagamentos ou doações online
- Integração com sistemas externos de gestão de igreja ou CRM
- Suporte a múltiplos idiomas inicialmente (portal em português brasileiro)
- Funcionalidades avançadas como recomendação personalizada de trilhas baseadas no histórico do usuário

## Further Notes

Este spec descreve o MVP inicial da Academia de Ensino da Comunidade Vitral, focando em proporcionar acesso organizado e atraente ao conteúdo formativo já existente, mas sempre com o propósito maior de formar discípulos que conhecem Jesus, são transformados por Sua graça e são enviados para servir ao mundo com amor. Futuras iterações podem incluir:

- Sistema de login com rastreamento de progresso (se considerado útil e não prejudicial ao espírito de graça)
- Certificados de conclusão para cada trilha (se forem apresentados como reconhecimento de crescimento, não como mérito próprio)
- Funcionalidade de busca avançada
- Área de recursos complementares (livros, podcasts, materiais de apoio) que apontem para Jesus e para o serviço
- Integração com calendário de eventos da comunidade para facilitar o envolvimento em oportunidades de serviço
- Suporte a múltiplos idiomas
- Plataforma de conteúdo próprio além dos repositórios existentes, sempre mantendo o foco em formar discípulos para a glória de Deus

O sucesso deste MVP será medido não apenas pela adoção pelos membros da comunidade e facilidade de acesso aos recursos formativos, mas também pelo feedback positivo sobre como a plataforma ajudou as pessoas a crescerem em seu relacionamento com Jesus, em seu caráter cristão e em seu serviço amoroso ao próximo, sempre reconhecendo que qualquer crescimento é dom da graça de Deus, não fruto do próprio esforço.