# Site Empresarial SINC

Este é o repositório do site institucional da SINC. O projeto foi construído utilizando tecnologias web nativas (HTML5, Vanilla CSS3 e Javascript) para garantir alta performance, flexibilidade e independência de frameworks pesados.

O design segue um estilo *Premium*, utilizando "Dark Mode" como base e a cor Laranja Escuro para destaques.

## 📁 Estrutura do Projeto

- `index.html`: A estrutura principal do site, contendo todas as seções (Hero, Sobre, Serviços, Contato).
- `style.css`: Todo o design system, animações e regras de responsividade.
- `main.js`: Lógica do menu mobile e animações de aparecimento ao rolar a página (Scroll Reveal).
- `assets/`: Pasta contendo as imagens geradas (Logo e Hero Background).

## 🚀 Como testar e visualizar o site

Existem três maneiras simples de visualizar o site localmente na sua máquina:

### Opção 1: Abrir diretamente no Navegador (Mais Rápido)
Como o projeto não utiliza ferramentas de compilação ou frameworks, você pode simplesmente:
1. Abrir a pasta `Site Sinc` no seu gerenciador de arquivos.
2. Dar um duplo clique no arquivo `index.html`.
3. Ele abrirá automaticamente no seu navegador padrão (Chrome, Firefox, Edge, etc).

### Opção 2: Usar um Servidor Local com Python (Recomendado)
Se você estiver no terminal (Linux/Mac) ou se tiver o Python instalado:
1. Abra o terminal na pasta do projeto (`/home/vini/Documents/SINC/Site Sinc/`).
2. Execute o comando:
   ```bash
   python3 -m http.server 8000
   ```
3. Abra o seu navegador e acesse a URL: `http://localhost:8000`

### Opção 3: Usar o VS Code (Live Server)
Se você estiver utilizando o editor Visual Studio Code:
1. Instale a extensão chamada **Live Server** (por Ritwick Dey).
2. Abra a pasta do projeto no VS Code.
3. Clique com o botão direito no arquivo `index.html` e selecione **"Open with Live Server"**.
4. O navegador abrirá automaticamente e qualquer alteração salva no código será atualizada instantaneamente na tela.

---
**Dica de visualização:** Ao testar no navegador, você pode usar a tecla `F12` (Ferramentas de Desenvolvedor) e clicar no ícone de "Dispositivos" (ou pressionar `Ctrl + Shift + M`) para simular como o site se comporta nas telas de diversos smartphones.
