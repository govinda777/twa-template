# twa-template .

> Template inicial para um novo TWA interagindo com a blockchain TON

# Visão Geral

O projeto é altamente opinativo, e há muitas outras rotas alternativas que poderiam ter sido tomadas. Alguns exemplos:

- Suporta carteiras Ton Connect 2
- Usa vite com react (alternativa ao create-react-app)
- Usa o pacote `ton` do npm

# Visão Geral da Aplicação

Este projeto é um Telegram Web App (TWA) construído com React e Vite, projetado para interagir com a blockchain TON. A aplicação utiliza a biblioteca `@tonconnect/ui-react` para conectar-se a carteiras TON e `@twa-dev/sdk` para interagir com a API do Telegram.

A estrutura do projeto é a seguinte:

- `src/`: Contém o código-fonte da aplicação React.
  - `main.tsx`: O ponto de entrada da aplicação.
  - `App.tsx`: O componente principal da aplicação.
  - `hooks/`: Contém hooks personalizados para interagir com a blockchain TON.
- `public/`: Contém os arquivos estáticos da aplicação.
- `configure.js`: Um script para configurar o bot do Telegram.

# Pré-requisitos

- Node.js v16 (outras versões podem funcionar, precisa de mais testes)
- Uma carteira compatível com TON Connect (ex: [Tonkeeper](https://tonkeeper.com/))

# O que este repositório contém?

- Um aplicativo pronto para TWA baseado em react, interagindo com TON
- Github actions configuradas para implantar o aplicativo no github pages
- Um script para conectar um bot do telegram ao aplicativo implantado

# Como usar

1. Crie um template a partir deste repositório com o botão "Use this template"

   1. Escolha um nome para o seu repositório
   2. `**IMPORTANTE!!**` marque "Include all branches", caso contrário, a implantação do github pages não funcionará.
      ![image](https://user-images.githubusercontent.com/5641469/191731317-14e742fd-accb-47d4-a794-fad01148a377.png)

2. Clone este repositório e execute `yarn`

3. Crie um novo bot com o [botfather](https://t.me/botfather)
   1. Digite `/newbot`
   2. Escolha um nome para o seu bot, ex: `My Ton TWA`
   3. Escolha um nome de usuário para o seu bot, ex: `my_ton_twa_482765_bot`
   4. Anote o token de acesso, ex: `5712441624:AAHmiHvwrrju1F3h29rlVOZLRLnv-B8ZZZ`
   5. Execute `yarn configbot` para vincular seu bot ao aplicativo da web

# Quick Start

## Executando Localmente

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/ton-community/twa-template.git
    cd twa-template
    ```
2.  **Instale as dependências:**
    ```bash
    yarn
    ```
3.  **Configure o bot do Telegram:**
    Crie um novo bot com o [@BotFather](https://t.me/botfather) e obtenha o token de acesso. Em seguida, execute o seguinte comando para vincular seu bot ao aplicativo da web:
    ```bash
    yarn configbot
    ```
4.  **Inicie o servidor de desenvolvimento:**
    ```bash
    npm run dev
    ```
    Abra seu navegador e acesse `http://localhost:3000` para ver a aplicação em execução.

## Deploy

O deploy é feito automaticamente via GitHub Actions. Sempre que um push é feito para a branch `main`, a aplicação é implantada no GitHub Pages.

Para que o deploy funcione corretamente, certifique-se de que a opção "Include all branches" foi marcada ao criar o template a partir deste repositório.

# Desenvolvimento

1. Execute `npm run dev` e edite o código conforme necessário
2. Ao enviar para a branch `main`, o aplicativo será implantado automaticamente via github actions.

# Roadmap

- [ ] Suporte para transferência de Jetton

# Licença

MIT
