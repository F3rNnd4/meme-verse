# Atividade Avaliativa: Componentização com Props em Next.js


## Objetivo


Desenvolver uma aplicação de compartilhamento de memes utilizando Next.js 15, aplicando conceitos de componentização com props e CSS Modules.


## Contexto


Você foi contratado para trabalhar como desenvolvedor frontend no "MemeVerse", uma plataforma de compartilhamento de memes voltada para adolescentes e jovens adultos. O time de design já criou uma interface completa, e agora você precisa implementar essa interface usando Next.js 15, focando em componentização e reutilização de código.

## Requisitos da Atividade

### Estrutura de Componentes Obrigatória

Você deve criar, no mínimo, os seguintes componentes:

1. `Header` - Componente de cabeçalho com logo, navegação e busca
2. `HeroSection` - Seção principal com o meme do dia
3. `MemeCard` - Card individual de um meme (deve ser reutilizável)
4. `InteractionBar` - Barra de interação com botões de curtir, comentar, etc.
5. `CategoriesSection` - Seção de navegação por categorias
6. `Footer` - Rodapé com links de navegação e informações da empresa
7. `Sidebar` - Barra lateral com conteúdo complementar


## Instruções de instalação e execução - Criação do zero


1. No terminal, realizar o comando `npx create-next-app@latest nome-do-projeto`;
2. Responder à perguntas da criação do projeto como:
    - Ok to proceed? y
    - TypeScript - No
    - ESLint - Yes
    - Tailwind CSS - No
    - `src/` directory - Yes
    - App Router - Yes
    - Turbopack for `next dev` - Yes
    - import alias - No
3. Acessar o diretório do projeto com `cd nome-do-projeto`;
4. Mudar o nome dos arquivos `layout.js e page.js` para `layout.jsx e page.jsx`;
5. Executar o comando `npm run dev` para iniciar o servidor de desenvolvimento;
6. Acessar o projeto no navegador em `http://localhost:3000`.

## Instruções de instalação e execução - Git Clone

1. Clone o repositório e entre na pasta do projeto;
2. Instale as dependências com `npm install`;
3. Execute o comando `npm run dev` para iniciar o servidor de desenvolvimento;
4. Acesse o projeto no navegador em `http://localhost:3000`.


## Descrição dos componentes criados

1. **Header**  
   O componente `Header` contém o logotipo da aplicação, uma barra de navegação com "links" para algumas páginas, um sininho de notificações e a foto de perfil para navegar até a página da conta.

2. **HeroSection**  
   A `HeroSection` exibe o "Meme do Dia" em destaque, com a imagem do meme, título, descrição, quem postou, um botão para ver o meme por completo, os likes e comentários.

3. **MemeCard**  
   O `MemeCard` é um componente reutilizável que exibe informações de um meme, como título, descrição, autor, categoria e imagem. Ele também inclui o componente `InteractionBar` para interações como curtidas, comentários, botão de compartilhamento e de salvar.

4. **InteractionBar**  
   A `InteractionBar` é uma barra de interação que contém botões para curtir, comentar, compartilhar e salvar exibindo o número de curtidas e comentários de cada meme. Este componente foi projetado para ser reutilizado em diferentes contextos.

5. **CategoriesSection**  
   A `CategoriesSection` exibe uma lista de categorias para facilitar a navegação por temas específicos de memes. Cada categoria é apresentada como um botão estilizado.

6. **Footer**  
   O `Footer` contém links de navegações, recursos, informações sobre a empresa e links para redes sociais. Ele foi projetado para ser simples e funcional.

7. **Sidebar**  
   A `Sidebar` exibe informações complementares, como eventos próximos, recursos premium e tags populares. Este componente foi projetado para enriquecer a experiência do usuário com conteúdo adicional.

## Decisões de design tomadas

- **Uso de CSS fornecido pelo professor**  
   Para garantir consistência visual e economizar tempo, optei por utilizar o CSS fornecido pelo professor como base para os estilos do projeto. Isso ajudou a manter a padronização e focar na implementação dos componentes.

## Desafios enfrentados e soluções aplicadas

1. **Desafios Iniciais**
    - Dificuldade em entender a estrutura e como os componentes interagem entre si.
    - Solução: Aula prática com o professor utilizando outro projeto como exemplo, o que ajudou a entender melhor a estrutura e a lógica do Next.js.

2. **Erros pequenos**
    - Tive dificuldades com pequenos erros de sintaxe e lógica, como esquecer de importar componentes ou não passar as props corretamente.
    - Solução: Revisão constante do código, uso de ferramentas de linting (ESLint e Prettier) e Github Copilot para identificar e corrigir esses erros rapidamente.
    - Exemplo: Ao criar o componente `MemeCard` ou o `InteractionBar`, inicialmente não passei as props corretamente, o que resultou em erros de renderização. Após revisar a mensagem do erro, o código e o exemplo da aula, consegui resolver esse problema.