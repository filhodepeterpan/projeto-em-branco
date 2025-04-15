# 🧱 Projeto em Branco - Template Padrão com SCSS

Este é um projeto base feito para iniciar uma aplicação web com uma estrutura de pastas e arquivos pronta. Ele já vem estruturado com:

- Organização de arquivos por responsabilidade
- Suporte a SCSS
- Uso de variáveis com `:root`
- Estrutura pronta para deploy no Vercel

---

## 📁 Estrutura de pastas

```
📁 projeto-em-branco/
├── 📁 assets/
│   └── 📁 audio/
│   └── 📁 fonts/          
│   └── 📁 img/
│   └── 📁 video/ 
├── 📁 pages/
├── 📁 public/
│   ├── 🎨 style.css           # Arquivo gerado após a compilação do SASS
│   ├── 🎨 style.css.map       # Arquivo gerado após a compilação do SASS
├── 📁 scripts/
│   └── 📜 script.js            # Arquivo JavaScript
├── 📁 styles/
│   └── 🎨 _media.query.scss     # Estilos responsivos
│   ├── 🎨 _root.scss            # Variáveis e configurações globais
│   ├── 🎨 style.scss           # Estilos em geral
├── 🚫 .gitignore
├── 📄 index.html               # Página inicial
├── ⚙️ package.lock.json       # Mantém a versão estável
├── ⚙️ package.json            # Dependências
└── 📑 README.md
```

---

## ⚙️ Requisitos

- [Node.js e NPM](https://nodejs.org/)
- [Sass](https://sass-lang.com/)
- Live Server (recomendado no VSCode)
- [Live Sass Compiler](https://marketplace.visualstudio.com/items?itemName=glenn2223.live-sass) (extensão do VSCode)

---

## 🚀 Como usar o projeto

### 1. Faça o clone

```bash
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo
```

### 2. Instale as dependências (se houver `package.json`)

```bash
npm install
```

e

```bash
npm install -D sass
```

### 3. Compile o SCSS

Para compilar os arquivos `.scss` e gerar o arquivo `.css`, você pode usar o comando de build no terminal. No seu VS Code, basta rodar:

```bash
npm run build
```

Isso irá compilar os arquivos SCSS uma vez e gerar o arquivo style.css na pasta styles.

> 💡 O Live Sass Compiler também cria um arquivo `style.css.map` para ajudar no desenvolvimento com o DevTools do navegador.

> 💡 A compilação com o comando npm run build também evita que arquivos indesejados, como o style.css.map, sejam incluídos no seu repositório, já que estão no .gitignore.


### 4. Inicie com Live Server

Abra o projeto com o Live Server para ver as alterações em tempo real.

---
### 5. Mantenha o SASS no modo "Watching"

Rode uma única vez este comando:

```bash
npm run sass
```

E pronto! Agora é só construir seu site e seus estilos.

---

## 📝 Observações

- **NÃO edite diretamente o `style.css`** — ele é gerado automaticamente pelo Sass.
- **NÃO retire o `_ (underline)` dos arquivos `.scss`** — isso garante que somente o `style.css` será gerado, recebendo imports do `_media.query.scss` e do `_root.scss`, sem a necessidade de compilá-los individualmente.
- Estilos devem ser escritos apenas nos arquivos `.scss`.
- O `style.css` e o `style.css.map` estão no `.gitignore` para evitar conflitos e forçar o uso correto do Sass.

## 🌐 Deploy no Vercel

1. Crie uma conta e importe o projeto do GitHub.
2. Configure o comando de build:
   - **Build Command**: `npm run build`
   - **Output Directory**: `./`

Pronto! A Vercel cuidará de compilar o SCSS antes de servir os arquivos.

### OBS:
- Essa é a linha do `package.json` responsável por essa configuração de build:    
> "build": "sass ./styles/style.scss ./public/style.css --no-source-map"


---

## 🤝 Contribuindo

Sinta-se livre para copiar, melhorar ou adaptar esse template do seu jeito. E se quiser, me adiciona lá no [Linkedin](https://www.linkedin.com/in/douglassoaressantos/) ou no [BlueSky](https://bsky.app/profile/filhodepeterpan.bsky.social) =)



