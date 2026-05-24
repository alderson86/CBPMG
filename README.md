# Sistema de Auditoria e Inspeção Predial - CBMMG 🚒

Este é um sistema web móvel (Web App) leve, moderno e responsivo, desenvolvido especificamente para a realização de vistorias e auditorias de segurança contra incêndio e pânico, baseado nas diretrizes do Corpo de Bombeiros Militar de Minas Gerais (CBMMG).

O foco principal da aplicação é a **usabilidade no terreno (Mobile-First)**, permitindo que o vistoriador realize o preenchimento de forma rápida através do telemóvel/celular, mesmo sem internet estável.

---

## 🚀 Principais Funcionalidades

- **Design Mobile-First:** Interface inspirada nos padrões modernos de UI (estilo *Shadcn/UI*), com barra de navegação inferior nativa e botões táteis otimizados para o polegar.
- **Persistência de Dados (LocalStorage):** - **Rascunho Automático:** Cada alteração ou resposta é guardada instantaneamente no navegador. Se a aplicação for fechada ou a bateria acabar, o progresso não se perde.
  - **Histórico Local:** Os relatórios finalizados ficam arquivados localmente no dispositivo para consultas futuras.
- **Compressão Avançada de Imagens:** Suporta a captura de fotos diretamente da câmara do telemóvel. O sistema reduz e comprime a imagem automaticamente (JPEG 40%, máx. 300px de largura) para poupar memória no dispositivo e otimizar o tamanho do PDF.
- **Barra de Progresso:** Indicador fixo no topo que mostra a percentagem de conclusão do checklist em tempo real.
- **Dashboard de Conformidade:** Estatísticas rápidas que resumem o estado atual da inspeção (Itens Conformes, Inconformes, N/A e Pendentes).
- **Impressão/PDF Ultra-Otimizado:** Sistema inteligente de exportação que remove os elementos visuais da aplicação e gera um relatório técnico condensado, desenhado para ocupar o menor número de páginas possível.

---

## 📊 Estrutura do Checklist

O sistema conta com **71 itens de verificação técnicos**, abrangendo:
1. Documentação Técnica e Laudos (PSCIP, AVCB, SPDA, Gás, etc.)
2. Sistemas de Extintores (Validade, sinalização, distribuição e fixação)
3. Sinalização de Emergência e Rotas de Fuga (Placas fotoluminescentes, saídas e escadas)
4. Iluminação de Emergência (Autonomia, blocos autónomos e baterias)
5. Hidrantes, Mangueiras e Reservatórios técnicos
6. Alarmes, Detetores de Incêndio e Instalações de GLP
7. Brigada de Incêndio e Conformidade de Uso Geral

---

## 🛠️ Tecnologias Utilizadas

O projeto foi construído utilizando tecnologias puras da Web (Vanilla Architecture) para garantir velocidade máxima e zero dependências externas:

- **HTML5:** Estruturação semântica da aplicação e inputs nativos de câmara (`capture="environment"`).
- **CSS3:** Estilização moderna utilizando variáveis nativas (`:root`), flexbox, posicionamento pegajoso (`sticky`) e regras específicas de impressão (`@media print`).
- **JavaScript (ES6):** Manipulação de estado, processamento de imagem em fila com `HTML5 Canvas` + `FileReader` e gestão de armazenamento com a API `LocalStorage`.

---

## 💻 Como Utilizar

Por ser um ficheiro único estático, o sistema não requer qualquer tipo de instalação ou servidor:

1. Descarregue o ficheiro `sistema_auditoria_cbmmg.html`.
2. Abra o ficheiro em qualquer navegador web (Google Chrome, Safari, Microsoft Edge) no seu computador ou telemóvel.
3. **Na Auditoria:** Responda aos itens selecionando o estado (*Conforme, Inconforme, N/A*). Adicione quantidades, observações ou fotos se necessário.
4. **No Dashboard / Histórico:** Alterne entre as abas na barra inferior para acompanhar as métricas ou ver relatórios passados.
5. **Para Exportar:** Clique em **"Finalizar e Emitir Relatório"** para abrir a janela de impressão nativa do sistema. Pode imprimir diretamente em papel ou escolher a opção "Guardar como PDF".

---

## 📄 Licença e Uso

Este projeto foi desenvolvido para fins de facilitação operacional em auditorias internas e inspeções prediais. Pode ser livremente modificado, expandido ou integrado com bases de dados na nuvem (como Firebase ou APIs REST).
