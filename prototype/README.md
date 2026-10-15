# Protótipo da Academia de Ensino - Comunidade Vitral

Este protótipo responde à pergunta: "Como deveria ser a interface da academia de ensino que agrega as trilhas existentes da Comunidade Vitral?"

## Como executar

Como este é um protótipo estático de HTML/CSS/JS, você pode:

1. **Abrir diretamente no navegador**: Basta dar duplo-clique no arquivo `index.html` ou abri-lo em qualquer navegador moderno.

2. **Servir via HTTP local** (recomendado para melhor experiência):
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Então acesse: http://localhost:8000
   ```

## O que este protótipo demonstra

- **Navegação organizada por trilhas/módulos** com descrições claras (funcionalidade essencial escolhida)
- **Visual padronizado** usando as cores e identidade visual da Comunidade Vitral
- **Integração das 5 trilhas/módulos** dos repositórios existentes:
  - Trilha de Novos (9 passos)
  - Trilha Praticando o Caminho (17 passos)
  - Trilha de Liderança (4 módulos)
  - Dashboard de Estações
  - Panorama Bíblico
- **Layout responsivo** que funciona em desktop e mobile

## Observações importantes

- Este é um **protótipo descartável** criado apenas para validar o conceito visual e de navegação
- O conteúdo real permaneceria nos repositórios existentes, com este portal servindo como interface de navegação
- No MVP inicial, não haveria rastreamento de progresso ou login (conforme decisões tomadas durante o grill-with-docs)
- O foco é proporcionar acesso fácil e organizado ao conteúdo formativo existente