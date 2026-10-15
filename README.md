# 🧳 PackKeep

Uma aplicação web minimalista e progressiva (PWA) projetada para gerenciar checklists de viagens inspirada no fluxo prático do Google Keep: separação entre **Template Mestre**, **Viagens Modulares** com cálculo automático de itens, **Modo Poda rápida** e o **"Modo Volta"** (desmarcar tudo com 1 clique).

Tudo roda diretamente no navegador de forma totalmente estática, com persistência local e sincronização opcional na nuvem via GitHub Gist.

---

## ✨ Principais Funcionalidades

- **Matriz de Template Mestre (`viagem base`):** Sua lista base intocável com todos os seus itens essenciais organizados por categorias (Bolsas, Tech, Care, Remédios, Violeta, Roupas, etc.).
- **Duplicação Inteligente:** Crie novas viagens clonando o template ou qualquer viagem anterior do seu histórico.
- **Cálculo Automático de Itens:** Na criação da viagem, informe a quantidade de dias e o app calcula automaticamente as quantidades dinâmicas (ex: `cuecas = dias + 1`).
- **Modo Poda em 1 Clique:** Remova categorias inteiras ou itens avulsos instantaneamente antes de começar a arrumar a mala para viagens mais curtas.
- **Mala de Volta (Uncheck All):** Um botão de destaque para desmarcar todos os itens de uma só vez quando estiver arrumando a mala para retornar para casa.
- **Sincronização via GitHub Gist:** Mantenha seu histórico sincronizado entre o Mac e o iPhone de graça usando um Gist secreto pessoal, sem precisar de banco de dados externo.
- **PWA Nativo para iOS:** Instale direto na Tela de Início do iPhone para rodar em tela cheia, com suporte a *Safe Area* (Dynamic Island/Notch) e ícone dinâmico gerado em tempo real.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5 & Vanilla JavaScript (Single-File):** Sem frameworks pesados, sem etapas de *build* ou dependências de compiladores.
- **Tailwind CSS:** Estilização moderna e responsiva baseada em utilitários via CDN.
- **Font Awesome 6:** Ícones intuitivos.
- **GitHub Gists API:** Armazenamento em nuvem em formato JSON utilizando o ecossistema do próprio GitHub.

---

## 🚀 Como Usar e Rodar Localmente

Como a aplicação é contida em um único arquivo `index.html`, você pode executá-la de duas formas:

1. **Direto no Navegador:** Basta clonar o repositório e dar dois cliques no arquivo `index.html`.
2. **Via Servidor Local (se preferir):**
   ```bash
   npx serve .

---

## ☁️ Configurando a Sincronização (GitHub Gist)

Para manter seus dados sincronizados entre múltiplos dispositivos:
1. Vá nas configurações do seu GitHub e gere um **Personal Access Token (Classic)** com permissão exclusiva no escopo **`gist`**.
2. No aplicativo PackKeep, clique no botão de status **Gist Local** no topo da tela.
3. Cole o seu token e clique em **Salvar & Conectar** (o app criará e gerenciará um Gist privado chamado `packkeep_db.json` automaticamente).
4. No seu outro dispositivo (ex: iPhone), cole o mesmo token e clique em **Buscar meu Gist existente**.

---

## 📱 Instalação como App no iOS

1. Acesse a URL do projeto hospedada no seu **GitHub Pages** através do navegador **Safari** no iPhone.
2. Toque no botão **Compartilhar** ($\uparrow$) na barra inferior.
3. Selecione **"Adicionar à Tela de Início"**.
4. Abra o aplicativo diretamente pelo novo ícone na sua home screen para usá-lo em tela cheia.

---

## 📄 Licença

Este projeto é de uso pessoal e aberto sob a licença **MIT**.
