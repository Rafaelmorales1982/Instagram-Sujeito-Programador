# Projeto Instagram — Clone da Tela de Login

Projeto de estudo que recria a tela de login do Instagram utilizando **HTML5** e **CSS3**, com layout dividido em duas colunas: à esquerda, a imagem ilustrativa de um celular; à direita, o painel de login e o bloco de cadastro.

Desenvolvido durante o curso **[Sujeito Programador](https://sujeitoprogramador.com/)**.

---

## 📋 Sobre o projeto

O objetivo é praticar os fundamentos do desenvolvimento front-end, reproduzindo uma interface real e conhecida. O projeto tem foco em:

- Estruturação semântica do HTML;
- Organização do CSS por blocos comentados;
- Uso de **Flexbox** para centralizar e dividir o layout;
- Estilização de formulários (inputs, placeholder, estados de `:focus` e botão);
- Posicionamento de imagens via `background-image` no CSS.

> ⚠️ O projeto é **apenas visual/front-end**. Não há back-end, autenticação real ou envio de dados — o formulário não possui `action` configurada.

---

## 🖥️ Preview do layout

```
┌───────────────────────────────────────────────┐
│                                               │
│   ┌───────────────┐     ┌───────────────────┐ │
│   │               │     │   [ Logo Instagram]│ │
│   │   Imagem de   │     │                   │ │
│   │   um celular  │     │ [Usuário/E-mail]  │ │
│   │               │     │ [Senha]           │ │
│   │               │     │ [     Entrar    ] │ │
│   └───────────────┘     └───────────────────┘ │
│                         ┌───────────────────┐ │
│                         │ Não possui conta? │ │
│                         │    Cadastre-se    │ │
│                         └───────────────────┘ │
└───────────────────────────────────────────────┘
```

- **Coluna esquerda:** imagem `main-foto.png` aplicada como plano de fundo da `.left`.
- **Coluna direita:** painel branco com a logo, campos de usuário e senha, botão **Entrar** e o bloco "Não possui uma conta? cadastre-se".

---

## 🚀 Tecnologias utilizadas

| Tecnologia | Uso no projeto |
|------------|----------------|
| HTML5 | Estrutura e conteúdo da página |
| CSS3 | Estilos, layout com Flexbox e responsividade básica |
| Git/GitHub | Versionamento e publicação do código |

Nenhuma biblioteca ou framework foi utilizado — o projeto roda direto no navegador.

---

## 📁 Estrutura de arquivos

```
Projeto-instagram/
├── index.html          # Estrutura da página
├── css/
│   └── style.css       # Estilos do layout, formulário e painéis
├── img/
│   ├── logo.png        # Logo exibida no painel de login
│   ├── main-foto.png   # Imagem de fundo da coluna esquerda
│   ├── appstore.png    # Badge da App Store (ainda não utilizada)
│   └── googleplay.png  # Badge do Google Play (ainda não utilizada)
└── README.md
```

---

## ▶️ Como executar

Não é necessário instalar dependências. Basta clonar o repositório e abrir o `index.html` no navegador.

```bash
# Clone o repositório
git clone https://github.com/Rafaelmorales1982/Instagram-Sujeito-Programador.git

# Entre na pasta
cd Instagram-Sujeito-Programador
```

Depois, abra o arquivo `index.html` com dois cliques ou, se preferir, utilize a extensão **Live Server** do VS Code para visualizar com recarregamento automático.

---

## 🧩 Detalhes da implementação

### HTML (`index.html`)

- `#wrapper` → área global que ocupa toda a altura da tela (`100vh`).
- `#container` → limita a largura em `800px`, centraliza o conteúdo com `margin: 0 auto` e usa `display: flex` para colocar as colunas lado a lado.
- `.column.left` → coluna da ilustração.
- `.column.right` → coluna com `.login-painel` (logo + formulário) e `.infobox` (bloco de cadastro).

### CSS (`css/style.css`)

- **Reset básico:** `box-sizing: border-box`, remoção de margens e paddings padrão.
- **Layout:** `.column` recebe `flex: 1` e `width: 50%`, garantindo duas colunas de tamanhos iguais.
- **Formulário:** `display: flex` em coluna, inputs com `320px` de largura, borda arredondada e mudança de borda ao focar.
- **Botão:** fundo azul `#3c96ed`, texto branco em negrito e `cursor: pointer`.
- **Organização:** o arquivo é dividido por comentários (`CONFIGURAÇÃO PADRÃO`, `GLOBAL WRAPPER`, `CONTAINER`, `CADASTRE-SE`), facilitando a leitura e manutenção.

---

## ✅ O que já está pronto

- [x] Estrutura HTML da página de login;
- [x] Layout com duas colunas usando Flexbox;
- [x] Painel de login estilizado (logo, inputs e botão);
- [x] Bloco "Não possui uma conta? Cadastre-se";
- [x] Imagem ilustrativa na coluna esquerda;
- [x] Estilos de foco e placeholder dos campos.

## 🛣️ Próximos passos (roadmap)

- [ ] Adicionar os badges da App Store e Google Play na coluna esquerda (imagens já disponíveis em `img/`);
- [ ] Criar o rodapé com links (Meta, Sobre, Blog, Carreiras, Ajuda, etc.);
- [ ] Tornar o layout responsivo para telas menores (celulares e tablets);
- [ ] Ocultar a coluna da imagem em telas pequenas;
- [ ] Implementar validação básica do formulário;
- [ ] Criar a página de cadastro;
- [ ] Adicionar modo escuro (opcional).

---

## 👨‍💻 Autor

**Rafael Morales**

- GitHub: [@Rafaelmorales1982](https://github.com/Rafaelmorales1982)
- Projeto original: [Instagram-Sujeito-Programador](https://github.com/Rafaelmorales1982/Instagram-Sujeito-Programador)

---

## 📄 Observação

Este projeto foi desenvolvido **exclusivamente para fins de estudo**. A marca, o logotipo e o layout do Instagram pertencem à **Meta Platforms, Inc.** Nenhuma afiliação oficial é sugerida.
