Site Empresarial & Portal SINC
Este repositório contém o site institucional e o Portal Corporativo (SINC Workspace) da SINC. O projeto utiliza tecnologias web nativas para garantir performance, mantendo um design Premium em Dark Mode com destaques em Laranja Escuro.  

📁 Estrutura do Projeto
🌐 Site Institucional (Público)
index.html: Estrutura principal com seções Hero, Sobre, Serviços e Contato.  

style.css: Design system, animações e responsividade do site público.  

main.js: Lógica de navegação e animações de Scroll Reveal.  

🔐 Portal Corporativo (Restrito)
dashboard.html: Interface do portal com integração visual de ferramentas (Agenda, Tarefas e Drive).  

dashboard.css: Estilização específica para a grade de widgets e o overlay de login.  

dashboard.js: Lógica de autenticação simulada e controle de visibilidade dos widgets.  

🛠️ Novas Funcionalidades: SINC Workspace
O portal foi projetado para centralizar as ferramentas da equipe:  

Autenticação Restrita: Simulação de login via Google, permitindo acesso apenas para e-mails com domínio @sincjr.com.br.  

Integração com Google Workspace: Widgets que incorporam Google Calendar, Google Tasks e pastas compartilhadas do Google Drive via iframes.  

Interface Dinâmica: Transição suave entre a tela de login e o dashboard com animações de entrada para os cartões de dados.  

🚀 Como testar e visualizar o site
Opção 1: Abrir diretamente no Navegador
Abra a pasta do projeto e dê um duplo clique em index.html.  

Para acessar o portal, clique no botão "Entrar" no menu de navegação.  

Opção 2: Simulação de Login
No portal corporativo (dashboard.html):

Clique em "Entrar com Google".  

O sistema validará o domínio. Atualmente, está configurado para aceitar o e-mail membro@sincjr.com.br para fins de demonstração.
