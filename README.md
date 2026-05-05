# 🚀 SINC - Site Institucional & Portal Corporativo

Este repositório contém o ecossistema digital da **SINC**, composto por um site institucional de alta performance e um dashboard corporativo integrado ao Google Workspace. 

O projeto foi desenvolvido com tecnologias web nativas para garantir máxima performance, flexibilidade e um design *Premium* focado na experiência do usuário.

---

## ✨ Funcionalidades

### 🌐 Site Institucional (`index.html`)
- **Design Premium**: Interface moderna com Dark Mode e acentos em Laranja SINC.
- **Performance Nativa**: Carregamento ultrarrápido sem dependência de frameworks.
- **Totalmente Responsivo**: Otimizado para smartphones, tablets e desktops.
- **Scroll Reveal**: Animações fluidas ao rolar a página para uma navegação envolvente.

### 📊 Portal Corporativo (`dashboard.html`)
- **Acesso Restrito**: Sistema de login seguro simulado para membros `@sincjr.com.br`.
- **Google Workspace Integration**: Centralização de ferramentas em um só lugar.
- **Widgets em Tempo Real**:
    - 📅 **Agenda SINC**: Visualização completa do Google Calendar.
    - ✅ **Tarefas**: Gerenciamento de pendências via Google Tasks.
    - 📁 **Arquivos (Drive)**: Acesso direto a pastas compartilhadas do Google Drive.
- **Interface Glassmorphism**: Visual moderno utilizando efeitos de transparência e desfoque.

---

## 📁 Estrutura do Projeto

O projeto está organizado na pasta `/Site Sinc`:

- `index.html`: Página principal (Lp, Sobre, Serviços, Contato).
- `dashboard.html`: Portal interno para membros da SINC.
- `style.css`: Design system global e estilos do site principal.
- `dashboard.css`: Estilos específicos do portal (Grid, Widgets, Glassmorphism).
- `main.js`: Lógica de navegação e animações do site principal.
- `dashboard.js`: Lógica de autenticação e controle do portal corporativo.
- `assets/`: Identidade visual, ícones e recursos gráficos.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura semântica e SEO-friendly.
- **Vanilla CSS3**: Design System personalizado, Variáveis CSS e Flexbox/Grid.
- **Javascript (ES6+)**: Lógica funcional e manipulação dinâmica do DOM.
- **Google API Embeds**: Integração direta com serviços Workspace.

---

## 🚀 Como Visualizar o Projeto

Como o projeto é construído sobre tecnologias nativas, você não precisa instalar dependências (npm/yarn).

### Opção 1: VS Code (Live Server) - **Recomendado**
1. Abra a pasta do projeto no VS Code.
2. Clique com o botão direito em `index.html` e selecione **"Open with Live Server"**.
3. Isso habilitará o *Hot Reload*, atualizando o navegador a cada mudança no código.

### Opção 2: Servidor Local Python
No terminal, dentro da pasta `/Site Sinc`, execute:
```bash
python -m http.server 8000
```
Acesse: `http://localhost:8000`

### Opção 3: Acesso Direto
Basta abrir o arquivo `index.html` em qualquer navegador moderno.

---

## 💡 Notas de Implementação
O Dashboard utiliza *iframes* para integrar os serviços do Google. Para que os widgets carreguem corretamente, o usuário deve estar logado em sua conta Google no navegador. Os links de embed no arquivo `dashboard.html` devem ser atualizados com os IDs reais da Agenda e Pastas do Drive da SINC para produção.

---
**SINC - Consultoria Jr.**
*Transformando o futuro através da tecnologia e gestão.*

