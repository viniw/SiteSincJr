# Site Empresarial SINC com Dashboard Corporativo

Este é o repositório do site institucional da SINC, que agora inclui um **Dashboard Corporativo** integrado para os membros da empresa. O projeto foi construído utilizando tecnologias web nativas (HTML5, Vanilla CSS3 e Javascript) para garantir alta performance, flexibilidade e independência de frameworks pesados.

O design segue um estilo *Premium*, utilizando "Dark Mode" como base e a cor Laranja Escuro para destaques, proporcionando uma experiência moderna e profissional.

## ✨ Funcionalidades

- **Site Institucional**: Landing page completa com seções de Hero, Sobre, Serviços e Contato.
- **Design Responsivo**: Adaptado para dispositivos móveis, tablets e desktops.
- **Dashboard Protegido**: Área exclusiva para membros autenticados.
- **Integração Google Workspace**:
    - **Google Auth**: Login seguro utilizando contas @sincjr.com.br.
    - **Google Calendar**: Visualização da agenda da empresa em tempo real.
    - **Google Tasks**: Gerenciamento de tarefas pendentes diretamente no dashboard.
    - **Google Drive**: Acesso rápido a arquivos e documentos compartilhados.

## 📁 Estrutura do Projeto

Os arquivos principais estão organizados na pasta `Site Sinc`:

- `index.html`: Estrutura principal do site institucional.
- `style.css`: Design system global, animações e responsividade do site.
- `main.js`: Lógica do menu mobile e efeitos de scroll.
- `dashboard.html`: Interface do painel de controle corporativo.
- `dashboard.css`: Estilos específicos e layout do dashboard.
- `dashboard.js`: Lógica de autenticação Google e integração com APIs do Workspace.
- `assets/`: Pasta contendo imagens, ícones e recursos visuais.

## 🚀 Como testar e visualizar o site

Como o projeto é baseado em tecnologias web nativas, você pode visualizá-á-lo de forma simples:

### Opção 1: VS Code (Live Server) - **Recomendado**
Para uma melhor experiência com as integrações:
1. Abra a pasta `Site Sinc` no VS Code.
2. Instale a extensão **Live Server**.
3. Clique com o botão direito no `index.html` e selecione **"Open with Live Server"**.

### Opção 2: Servidor Local com Python
1. Abra o terminal na pasta `Site Sinc`.
2. Execute: `python -m http.server 8000`
3. Acesse `http://localhost:8000` no seu navegador.

### Opção 3: Abrir Diretamente
1. Localize a pasta `Site Sinc` no seu computador.
2. Dê um duplo clique no arquivo `index.html`.

---
**Nota sobre Autenticação:** A integração com o Google requer que o site seja servido através de uma origem autorizada (como `http://localhost`). O dashboard utiliza a API de Clientes do Google para autenticação segura.
