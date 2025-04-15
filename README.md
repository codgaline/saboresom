---

```md
# Sabor & Som

Sabor & Som é um projeto que oferece sugestões personalizadas de músicas, drinks e snacks com base no humor do usuário. Utilizando APIs públicas (TheCocktailDB, TheMealDB e Last.fm), o sistema retorna uma playlist e sugestões culinárias de forma dinâmica e divertida.

## Funcionalidades

- **Playlist Musical:** Sugestão de uma música baseada no humor informado.
- **Drinks:** Sugestão de um drink popular relacionado ao humor.
- **Snacks:** Sugestão de uma sobremesa ou lanche para complementar o momento.

## Tecnologias Utilizadas

- **Front-end:** HTML, CSS e JavaScript
- **Back-end:** Node.js com Express
- **APIs:** TheCocktailDB, TheMealDB e Last.fm
- **Controle de Versão:** Git

## Instalação

1. **Clone o repositório:**

   ```bash
   git clone <URL_DO_REPOSITÓRIO>
   cd saboresom
   ```

2. **Instale as dependências:**

   ```bash
   npm install
   ```

3. **Configure as variáveis de ambiente:**

   Crie um arquivo `.env` na raiz do projeto com a seguinte estrutura:

   ```env
   PORT=3001
   LASTFM_API_KEY=SUA_CHAVE_LASTFM_AQUI
   ```

4. **Inicie o servidor:**

   ```bash
   npm start
   ```

5. **Acesse o projeto:**

   Abra o navegador e vá para [http://localhost:3001](http://localhost:3001)

## Estrutura do Projeto

```
saboresom/
├── backend/
│   ├── server.js            # Servidor Express
│   └── services/
│       ├── drinkService.js  # Funções para buscar drinks
│       ├── snackService.js  # Funções para buscar snacks
│       └── playlistService.js  # Funções para buscar músicas
├── frontend/
│   ├── index.html           # Página principal
│   ├── style.css            # Estilos
│   └── app.js               # Lógica do front-end
├── .env                     # Variáveis de ambiente
├── package.json             # Configurações do projeto
└── README.md                # Este arquivo
```

## Uso

1. Abra a página principal e escolha seu "mood" no formulário.
2. Clique em "Ver Sugestões" para carregar a playlist, o drink e o snack correspondentes.
3. Se algum serviço não retornar resultados, serão exibidas sugestões padrão.
