# HelioPT

HelioPT e um site interativo para explorar o potencial solar em Portugal. O utilizador pode selecionar uma regiao no mapa, ver estimativas de producao diaria/anual, calcular poupanca aproximada e configurar paineis solares conforme o uso pretendido.

## Funcionalidades

- Mapa solar interativo de Portugal por regioes.
- Painel lateral com resumo, media diaria e media anual.
- Estimativas para paineis de 400W.
- Configurador de paineis em 3 passos.
- Selecao de varios usos de energia solar ao mesmo tempo.
- Filtros por gama de preco dos paineis.
- Calculo de quantidade, producao e total estimado.
- Login e registo ligados ao Supabase.
- Design escuro com animacoes, emojis e cursor solar animado.
- Layout adaptado para desktop e telemovel.

## Paginas

- `index.html` - mapa solar, painel de informacoes e configurador.
- `login.html` - entrada de utilizadores com Supabase.
- `register.html` - criacao de conta com Supabase.
- `style.css` - estilos, responsividade e animacoes.
- `supabase-config.js` - configuracao do Supabase.

## Como Abrir

Abre o ficheiro `index.html` no navegador.

No VS Code, a melhor opcao e usar a extensao **Live Server**:

1. Abre a pasta do projeto no VS Code.
2. Clica com o botao direito em `index.html`.
3. Escolhe `Open with Live Server`.

Tambem podes abrir diretamente:

```text
index.html
```

## Supabase

O projeto usa Supabase para login e registo.

O ficheiro `supabase-config.js` deve conter:

```js
const SUPABASE_URL = "https://ldqknjzefmnmkqqkkpkm.supabase.co";
const SUPABASE_ANON_KEY = "A_TUA_CHAVE_PUBLICA";

const supabaseClient = window.supabase.createClient(SUPABASE_URL, SUPABASE_ANON_KEY);
```

Importante: usa apenas a chave publica/publishable no frontend. Nunca coloques uma `service_role key` no site.

## Estrutura

```text
Heliopt/
  index.html
  login.html
  register.html
  style.css
  supabase-config.js
  README.md
```

## Tecnologias

- HTML
- CSS
- JavaScript
- Leaflet
- TopoJSON
- Supabase Auth

## Estado

Projeto em desenvolvimento. O foco atual e melhorar a experiencia visual, o configurador de paineis e a integracao com autenticacao.
