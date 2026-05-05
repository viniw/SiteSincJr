# 🚀 SINC - Portal Corporativo

Plataforma corporativa moderna desenvolvida para a SINC Jr., oferecendo um portal completo com dashboard integrado ao ecossistema Google (Calendar, Tasks e Drive) e área institucional.

## 📋 Índice

- [Visão Geral](#visão-geral)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Funcionalidades](#funcionalidades)
- [Instalação e Configuração](#instalação-e-configuração)
- [Como Usar](#como-usar)
- [Personalização](#personalização)
- [Integrações](#integrações)
- [Compatibilidade](#compatibilidade)
- [Contribuição](#contribuição)
- [Licença](#licença)

## 🎯 Visão Geral

O **SINC - Portal Corporativo** é uma aplicação web completa que combina um site institucional moderno com uma área de trabalho corporativa (dashboard). O sistema oferece:

- Site institucional responsivo com animações fluidas
- Sistema de autenticação simulado com validação de email corporativo
- Dashboard integrado com widgets do Google Workspace
- Interface moderna com design em dark mode
- Formulário de contato funcional

## 💻 Tecnologias Utilizadas

### Frontend
- **HTML5** - Estrutura semântica
- **CSS3** - Estilização avançada com:
  - CSS Grid e Flexbox para layouts responsivos
  - Animações customizadas
  - Glassmorphism effects
  - Variáveis CSS para theming
- **JavaScript (ES6+)** - Interatividade e lógica:
  - Intersection Observer para animações scroll
  - Manipulação dinâmica do DOM
  - Validações de formulário

### Fontes
- **Google Fonts**:
  - Outfit (títulos)
  - Inter (corpo de texto)

### APIs e Integrações
- Google Calendar (embed)
- Google Tasks (iframe)
- Google Drive (embed folder view)

## 📁 Estrutura do Projeto
sinc-portal/
│
├── index.html # Página institucional principal
├── dashboard.html # Dashboard corporativo
├── style.css # Estilos globais
├── dashboard.css # Estilos específicos do dashboard
├── main.js # Lógica da página principal
├── dashboard.js # Lógica do dashboard
│
├── assets/ # Diretório de imagens
│ └── icone.png # Logotipo do SINC
│
└── README.md # Documentação

text

## ✨ Funcionalidades

### Site Institucional (index.html)
- ✅ **Hero Section** com call-to-action
- ✅ **Sobre Nós** com grid de conteúdo e mockup interativo
- ✅ **Serviços** com cards interativos (3D hover effects)
- ✅ **Contato** com formulário funcional
- ✅ **Menu Mobile** responsivo com animação hambúrguer
- ✅ **Scroll Animations** com Intersection Observer
- ✅ **Navbar** com efeito blur ao scroll
- ✅ **Footer** com links e copyright

### Dashboard Corporativo (dashboard.html)
- ✅ **Login Simulado** com validação de email (@sincjr.com.br)
- ✅ **Widget Google Calendar** (visão mensal/semanal)
- ✅ **Widget Google Tasks** (tarefas pendentes)
- ✅ **Widget Google Drive** (arquivos compartilhados)
- ✅ **Sistema de Logout** com transição suave
- ✅ **Layout Responsivo** com grid adaptável
- ✅ **Animações** de entrada dos widgets

## 🔧 Instalação e Configuração

### Pré-requisitos
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Conexão com internet (para Google Fonts e embeds)
- (Opcional) Servidor web local para testes

### Passo 1: Download
```bash
# Clone o repositório (ou baixe os arquivos)
git clone https://github.com/sinc-jr/portal-corporativo.git
cd portal-corporativo
Passo 2: Estrutura de Arquivos
Certifique-se de que a pasta assets/ existe e contém o arquivo icone.png:

text
assets/
└── icone.png
Passo 3: Configuração Local
Você pode usar qualquer servidor local simples:

Opção A - Live Server (VS Code):

Instale a extensão "Live Server"

Clique com botão direito no index.html → "Open with Live Server"

Opção B - Python:

bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
Opção C - Node.js:

bash
npx serve .
Passo 4: Acesso
Acesse no navegador:

Site institucional: http://localhost:8000

Dashboard: http://localhost:8000/dashboard.html

🎮 Como Usar
Site Institucional
Navegue pelas seções usando o menu

Explore os serviços oferecidos

Preencha o formulário de contato (demo funcional)

Clique em "Entrar" para acessar o dashboard

Dashboard
Login: Use qualquer email com domínio @sincjr.com.br (exemplo: joao@sincjr.com.br)

Agenda: Visualize o calendário corporativo (widget Google Calendar)

Tarefas: Gerencie suas tarefas integradas ao Google Tasks

Drive: Acesse arquivos compartilhados (requer login Google)

Logout: Clique em "Sair" para retornar à tela de login

Testando o Sistema
javascript
// Emails válidos para teste:
"membro@sincjr.com.br"
"admin@sincjr.com.br"
"joao.silva@sincjr.com.br"

// Email inválido (não autentica):
"usuario@gmail.com"
🛠️ Personalização
Cores e Temas
Edite as variáveis CSS no style.css:

css
:root {
    --color-primary: #e65b2a;     /* Cor principal */
    --color-bg: #0A0A0A;          /* Fundo principal */
    --color-surface: #141414;     /* Superfícies */
    --color-text: #F0F0F0;        /* Texto principal */
}
Links de Embed (Google Workspace)
No arquivo dashboard.html, substitua os iframes:

Google Calendar:

html
<!-- Substitua src pelo seu calendário corporativo -->
<iframe src="https://calendar.google.com/calendar/embed?src=SEU_CALENDARIO&ctz=America/Sao_Paulo"></iframe>
Google Drive:

html
<!-- Substitua o ID da pasta pelo seu ID real -->
<iframe src="https://drive.google.com/embeddedfolderview?id=SEU_ID_PASTA#list"></iframe>
Integração Real com Google OAuth
Para implementar autenticação real:

Crie um projeto no Google Cloud Console

Habilite a Google Identity Services API

Configure OAuth 2.0 Client ID

Substitua o dashboard.js:

javascript
// Exemplo de integração real (a ser implementado)
const clientId = 'SEU_CLIENT_ID.apps.googleusercontent.com';

function initGoogleLogin() {
    google.accounts.id.initialize({
        client_id: clientId,
        callback: handleCredentialResponse
    });
}
🔌 Integrações
Atuais
Google Calendar: Embed nativo

Google Tasks: Interface via iframe

Google Drive: Folder view embed

Possíveis Expansões
Google OAuth 2.0 (autenticação real)

API do Google Tasks (listagem dinâmica)

Google Drive API (upload/download)

Google Meet (agendamento direto)

Analytics (dashboard personalizado)

Banco de dados para leads

🌐 Compatibilidade
Navegadores Suportados
Navegador	Versão Mínima
Chrome	90+
Firefox	88+
Safari	14+
Edge	90+
Opera	76+
Dispositivos
✅ Desktop (1920x1080 otimizado)

✅ Tablet (768px - 1024px)

✅ Mobile (320px - 768px)

👥 Contribuição
Faça um fork do projeto

Crie sua branch de feature (git checkout -b feature/NovaFuncionalidade)

Commit suas mudanças (git commit -m 'Adiciona nova funcionalidade')

Push para a branch (git push origin feature/NovaFuncionalidade)

Abra um Pull Request

Padrões de Código
HTML: Indentação de 2 espaços

CSS: Seletores em kebab-case

JavaScript: camelCase para variáveis/funções

📄 Licença
Este projeto é de uso exclusivo da SINC Jr. Todos os direitos reservados.

📞 Suporte
Para dúvidas ou sugestões:

Email: contato@sincjr.com.br

Dashboard: Acessar Dashboard

🎨 Demonstração
Site Institucional
Design moderno com efeitos glassmorphism

Animações suaves ao scroll

Experiência mobile-first

Dashboard
Interface profissional para gestão

Visualização centralizada de ferramentas

Transições fluidas entre login/dashboard

🚀 Roadmap
Implementar autenticação real com Google OAuth

Adicionar dashboard analytics (KPIs)

Criar área de administração

Implementar chat interno

Adicionar módulo de relatórios

Integrar com sistemas de CRM

Desenvolvido com 🧡 pela Equipe SINC Jr.

Transformando gestão em inovação

text

Este README fornece:

1. **Documentação completa** do projeto
2. **Instruções claras** de instalação e uso
3. **Guia de personalização** detalhado
4. **Informações de compatibilidade**
5. **Roadmap** para desenvolvimento futuro
6. **Exemplos práticos** de integração

O documento está estruturado profissionalmente, pronto para ser usado em repositórios Git ou documentação interna da empresa.
