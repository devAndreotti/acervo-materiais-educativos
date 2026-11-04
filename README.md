# 📚 Acervo de Materiais Educativos

<p align="center">
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/devAndreotti/acervo-materiais-educativos?style=flat-square&labelColor=111827&color=22c55e">
  <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/devAndreotti/acervo-materiais-educativos?style=flat-square&labelColor=111827&color=38bdf8">
  <img alt="GitHub stars" src="https://img.shields.io/github/stars/devAndreotti/acervo-materiais-educativos?style=flat-square&labelColor=111827&color=f59e0b">
  <img alt="License MIT" src="https://img.shields.io/badge/license-MIT-eab308?style=flat-square&labelColor=111827">
</p>

<p align="center">
  <img alt="HTML5" src="https://img.shields.io/badge/HTML5-e34f26?style=flat-square&logo=html5&logoColor=white">
  <img alt="CSS3" src="https://img.shields.io/badge/CSS3-1572b6?style=flat-square&logo=css3&logoColor=white">
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-f7df1e?style=flat-square&logo=javascript&logoColor=111827">
  <img alt="GitHub Pages" src="https://img.shields.io/badge/GitHub%20Pages-222222?style=flat-square&logo=github&logoColor=white">
  <img alt="GoatCounter" src="https://img.shields.io/badge/GoatCounter-Analytics-7c3aed?style=flat-square&labelColor=111827">
</p>

<p align="left">
  <strong>Cartilhas, ebooks e infográficos gratuitos, prontos para baixar.</strong><br />
  Um site estático que reúne materiais educativos sobre segurança digital, meio ambiente e IA, com contagem de acessos e downloads.
</p>

![Banner do Acervo de Materiais Educativos](./Banner.png)

> Um acervo simples, sem cadastro e sem anúncios: o material está a um clique e pode ser compartilhado livremente.

---

## 🧭 Visão geral

**Acervo de Materiais Educativos** é um site estático publicado no GitHub Pages. Ele organiza os materiais por tema e permite baixar cada PDF diretamente.

1. **Lista os materiais** por tema, com ODS e status de disponibilidade
2. **Libera os PDFs** de cada atividade (cartilha, ebook ou infográfico)
3. **Conecta cada material** ao formulário de feedback comunitário
4. **Registra acessos e downloads** com o GoatCounter, sem cookies

O foco é publicar materiais de forma clara e sem fricção, mantendo o código simples de manter.

---

## 🎬 Demo

<p align="center">
  <img src="./photo.png" alt="Exemplo visual do Acervo de Materiais Educativos" width="92%" />
</p>

---

## 🔀 Fluxo

```mermaid
flowchart LR
    A["Visitante"] --> B["Página do acervo"]
    B --> C["Filtro por tema"]
    C --> D["Download do PDF"]
    B --> E["Pesquisa de feedback"]
    D --> F["GoatCounter registra o evento"]
    E --> F

    style A fill:#450a0a,color:#fff,stroke:#7f1d1d
    style B fill:#7f1d1d,color:#fff,stroke:#7f1d1d
    style C fill:#b91c1c,color:#fff,stroke:#7f1d1d
    style D fill:#dc2626,color:#fff,stroke:#b91c1c
    style E fill:#dc2626,color:#fff,stroke:#b91c1c
    style F fill:#f97316,color:#111827,stroke:#ea580c
    linkStyle default stroke:#7f1d1d,stroke-width:2px
```

---

## 👥 Para quem é

- Estudantes e professores que querem material pronto para aula ou estudo
- Famílias e responsáveis buscando orientação sobre segurança digital
- Microempreendedores interessados em ferramentas gratuitas de IA
- Qualquer pessoa que queira compartilhar os materiais com outras

---

## 🧰 Stack

- **HTML5 e CSS3** para a estrutura e o layout responsivo, com tema claro e escuro
- **JavaScript** puro para o filtro por tema e a troca de tema
- **GitHub Pages** para publicação, sem servidor
- **GoatCounter** para contagem de visitas e cliques, sem cookies

---

## 📋 Pré-requisitos

*   [x] **Navegador moderno** - para visualizar o site localmente ou online
*   [x] **Git** - para clonar e publicar alterações
*   [x] **Conta no GitHub** - apenas se for publicar sua própria cópia

---

## ⚙️ Configuração

### 1. Clonar o repositório

```bash
git clone https://github.com/devAndreotti/acervo-materiais-educativos.git
cd acervo-materiais-educativos
```

### 2. Contagem de acessos

A contagem usa o GoatCounter. Para usar outra conta, troque o endereço no `index.html`:

```html
<script data-goatcounter="https://SEU-CODIGO.goatcounter.com/count" async src="//gc.zgo.at/count.js"></script>
```

| Variável | Descrição | Exemplo |
|---|---|---|
| `SEU-CODIGO` | Código da sua conta no GoatCounter | `devandreotti` |

### 3. Testar localmente

```bash
python3 -m http.server 8000
```

Depois abra `http://localhost:8000` no navegador.

---

## 🚀 Uso

### Fluxo diário

1. Coloque o PDF novo em `materiais/`
2. Abra o `index.html` e troque o card da atividade: remova a classe `locked`, adicione os links e o botão de pesquisa
3. Confira localmente com o servidor de teste
4. Faça commit e push para a branch `main`

### Exemplo

```bash
git add materiais/novo-material.pdf index.html
git commit -m "feat: libera novo material"
git push origin main
```

### O que fazer depois

- Conferir se o GitHub Pages terminou o build (aba **Actions** ou **Settings → Pages**)
- Verificar os eventos no painel do GoatCounter
- Atualizar o selo de publicação quando um post novo for ao ar

---

## 🗂️ Estrutura do projeto

```text
acervo-materiais-educativos/
├── index.html          # Página do acervo, com filtro e troca de tema
├── favicon.svg         # Ícone da aba do navegador
├── materiais/          # PDFs publicados (cartilhas, ebooks e infográficos)
├── Banner.png          # Imagem de capa do README
├── photo.png           # Captura da página para o README
├── .nojekyll           # Desativa o processamento do Jekyll no GitHub Pages
└── README.md
```

---

## 🤝 Contribuindo

Contribuições são bem-vindas!

1. Faça um fork do repositório
2. Crie uma branch: `git checkout -b feature/sua-feature`
3. Commit suas alterações: `git commit -m "feat: minha contribuição"`
4. Push da branch: `git push origin feature/sua-feature`
5. Abra um Pull Request com um resumo das alterações

Use [Conventional Commits](https://www.conventionalcommits.org/): `feat:`, `fix:`, `docs:`, `style:`, `refactor:`, `test:`, `chore:`.

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](./LICENSE) para detalhes.

---

<p align="center">
  Desenvolvido com ☕ por <a href="https://github.com/devAndreotti">devAndreotti</a>
</p>
