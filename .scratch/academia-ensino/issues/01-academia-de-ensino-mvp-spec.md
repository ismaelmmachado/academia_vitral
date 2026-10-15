Status: ready-for-agent

# Academia de Ensino - MVP Spec

This issue contains the specification for the MVP of the Academia de Ensino da Comunidade Vitral.

## Problem Statement

A Comunidade Vitral possui diversos recursos de formação cristã distribuídos em repositórios GitHub separados (Trilha de Novos, Trilha Praticando o Caminho, Trilha de Liderança, Panorama Bíblico e um dashboard de estações), mas não há um ponto centralizado onde os membros da comunidade possam facilmente descobrir, navegar e acessar todo esse conteúdo formativo de forma organizada. Os membros enfrentam dificuldade para encontrar o conteúdo adequado ao seu estágio de jornada espiritual e perderiam tempo procurando pelos materiais em diferentes locais.

## Solution

Criar um portal web responsivo que sirva como academia de ensino centralizada da Comunidade Vitral, organizando e apresentando as trilhas de formação existentes em uma estrutura de navegação clara, permitindo que membros da comunidade explorem e acessem os recursos de formação de acordo com suas necessidades e estágio de crescimento espiritual, mantendo o conteúdo original intacto nos repositórios fonte.

## User Stories

1. Como um visitante novo na comunidade, quero ver uma visão geral do que a academia de ensino oferece, para que eu possa entender rapidamente as opções de formação disponíveis.
2. Como um membro da comunidade interessado em crescimento espiritual, quero navegar facilmente entre as diferentes trilhas de formação (Trilha de Novos, Trilha Praticando o Caminho, Trilha de Liderança), para que eu possa encontrar o conteúdo adequado ao meu estágio de fé.
3. Como um líder ou aspirante a líder na comunidade, quero acessar rapidamente a Trilha de Liderança e recursos relacionados, para que eu possa desenvolver minhas habilidades de serviço e gestão.
4. Como alguém interessado em entender melhor as Escrituras, quero acessar o Panorama Bíblico de forma destacada no portal, para que eu possa estudar a Bíblia de forma sistemática.
5. Como um facilitador ou líder de grupo, quero acessar o Dashboard de Estaçõe para ver todas as trilhas disponíveis em um único lugar, para que eu possa orientar outros membros sobre quais trilhas fazer.
6. Como um usuário em dispositivo móvel, quero que o portal seja responsivo e fácil de usar em meu smartphone ou tablet, para que eu possa acessar os conteúdos em qualquer lugar.
7. Como um membro da comunidade, quero identificar visualmente que este portal pertence à Comunidade Vitral através do uso da identidade visual existente, para que eu sinta confiança e pertencimento ao acessar os recursos.
8. Como um visitante, quero ver descrições claras de cada trilha incluindo o número de encontros/módulos e o público-alvo, para que eu possa escolher a trilha mais adequada às minhas necessidades atuais.
9. Como um usuário, quero acessar diretamente o conteúdo original nos repositórios fonte através de links claros no portal, para que eu tenha certeza de que estou acessando o material mais atualizado e autêntico.
10. Como um membro menos experiente com tecnologia, quero uma interface simples e intuitiva que não requer login ou configuração complexa, para que eu possa começar a aprender imediatamente sem barreiras técnicas.

## Scenarios

Given que o usuário acessa o portal da academia de ensino
Quando ele visita a página inicial
Então ele deve ver uma apresentação clara da academia com opções para explorar as trilhas de formação

Given que o usuário está na página inicial
Quando ele clica no botão para explorar as trilhas
Então ele deve ser rolado para a seção que apresenta todas as trilhas disponíveis

Given que o usuário está vendo a seção de trilhas
Quando ele observa o card da "Trilha de Novos"
Então ele deve ver que é para iniciantes, tem 9 encontros e uma descrição sobre identidade em Cristo e pertencimento à comunidade

Given que o usuário está vendo a seção de trilhas
Quando ele observa o card da "Trilha Praticando o Caminho"
Então ele deve ver que tem 17 passos divididos em 2 etapas e foca em práticas espirituais e serviço comunitário

Given que o usuário está vendo a seção de trilhas
Quando ele observa o card da "Trilha de Liderança"
Então ele deve ver que tem 4 módulos e foca em desenvolvimento de liderança cristã com ênfase em serviço

Given que o usuário está vendo a seção de trilhas
Quando ele observa o card do "Dashboard de Estações"
Então ele deve ver que é um portal integrado para navegar entre todas as trilhas

Given que o usuário está vendo a seção de trilhas
Quando ele observa o card do "Panorama Bíblico"
Então ele deve ver que é uma série de vídeos para entender as Escrituras do Antigo ao Novo Testamento

Given que o usuário está em um dispositivo móvel
Quando ele acessa o portal
Então o layout deve adaptar-se para tela menor com menu de navegação colapsável e cards ocupando toda a largura

Given que o usuário clica em qualquer botão de "Começar", "Acessar" ou "Assistir" em um card de trilha
Então ele deve ser redirecionado para o conteúdo original desse recurso nos repositórios fonte da Comunidade Vitral

## Implementation Decisions

- **Abordagem Técnica**: Criar um portal web estático usando HTML/CSS/JS que serve como interface de navegação e agregação visual, com links diretos para o conteúdo existente nos repositórios GitHub da Comunidade Vitral
- **Arquitetura**: Aplicação de página única (SPA) simples ou múltiplas páginas estáticas vinculadas, dependendo da complexidade desejada para o MVP
- **Integração de Conteúdo**: Manter todo o conteúdo formativo nos repositórios existentes (trilha_de_novos, trilha_praticando_o_caminho, trilha_lideranca, panorama_biblico, trilhas_discipulado-v2) e criar links a partir do portal para esses recursos
- **Identidade Visual**: Usar as cores existentes da Comunidade Vitral (verde petróleo #005f6b, sálvia #94a69a) e fonte Montserrat conforme definido na trilha de liderança
- **Responsividade**: Implementar layout responsivo usando CSS Flexbox/Grid que funcione em dispositivos móveis e desktop
- **Navegação**: Menu deheader fixo com links para as principais seções do portal (Inicio, Trilhas, Recursos, Sobre)
- **Apresentação de Trilhas**: Usar um grid de cards responsivo onde cada card representa uma trilha/módulo com ícone, título, descrição, detalhes (duração, nível) e chamada para ação
- **Hospedagem**: Utilizar GitHub Pages para hospedar o portal, similarmente aos sites existentes da comunidade
- **Manutenção**: Implementar como um sistema híbrido onde a estrutura e navegação estão no portal, mas o conteúdo permanece nos repositórios fonte, permitindo atualizações independentes

## Testing Decisions

- **Escopo dos Testes**: Testar o comportamento externo do portal através de testes de interface que verifiquem:
  - Renderização correta dos elementos principais (header, hero section, cards de trilhas, footer)
  - Funcionalidade do menu de navegação responsivo
  - Correção dos links para os repositórios fonte
  - Adaptação do layout em diferentes tamanhos de tela (mobile, tablet, desktop)
- **Abordagem de Testes**: Para o MVP inicial, testes manuais serão suficientes dada a natureza estática e simples do portal. Testes automatizados podem ser adicionados em fases posteriores se o projeto crescer em complexidade.
- **Qualidade de Testes**: Os testes devem focar no comportamento do usuário final (o que ele vê e pode fazer) e não em detalhes de implementação interna.

## Out of Scope

- Sistema de autenticação de usuários ou login
- Rastreamento de progresso individual ou conquistas
- Funcionalidade de busca por tópicos ou palavras-chave dentro do conteúdo
- Área de comentários, discussão ou interação social entre usuários
- Criação ou modificação do conteúdo formativo existente (todo o conteúdo permanecerá nos repositórios fonte)
- Funcionalidade de e-commerce, pagamentos ou doações online
- Integração com sistemas externos de gestão de igreja ou CRM
- Suporte a múltiplos idiomas inicialmente (portal em português brasileiro)
- Funcionalidades avançadas como recomendação personalizada de trilhas baseadas no histórico do usuário

## Further Notes

Este spec descreve o MVP inicial da Academia de Ensino da Comunidade Vitral, focando em proporcionar acesso organizado e atraente ao conteúdo formativo já existente. Futuras iterações podem incluir:

- Sistema de login com rastreamento de progresso
- Certificados de conclusão para cada trilha
- Funcionalidade de busca avançada
- Área de recursos complementares (livros, podcasts, materiais de apoio)
- Integração com calendário de eventos da comunidade
- Suporte a múltiplos idiomas
- Plataforma de conteúdo próprio além dos repositórios existentes

O sucesso deste MVP será medido pela adoção pelos membros da comunidade, facilidade de acesso aos recursos formativos e feedback positivo sobre a experiência de navegação e descoberta de conteúdo.

## Relacionado a
- CONTEXT.md (termos do domínio)
- SPEC.md (especificação completa)
- prototype/ (protótipo visual de referência)