📄 A4 Doc Studio

Descrição curta para o campo "About" do GitHub:
Estúdio web leve para manipulação de documentos A4 em imagem, substituição inteligente de termos mantendo a fonte original, marcação rápida de caixas de seleção ("[X]"), preenchimento de dados em lote com data automática e exportação direta para PDF/Impressão A4.

✨ Sobre o Projeto

O A4 Doc Studio é uma aplicação web 100% client-side (roda direto no navegador, sem necessidade de servidor ou banco de dados externo) desenvolvida para automatizar o preenchimento, a substituição de termos e a preparação para impressão de múltiplos documentos digitalizados ou formulários em formato de imagem A4 (PNG, JPG, WEBP).

Quando um documento existe apenas como imagem, editar palavras específicas ou preencher formulários repetitivos costuma exigir editores pesados. O A4 Doc Studio resolve isso criando máscaras inteligentes que capturam a cor exata do papel ao fundo e aplicam o novo texto calibrando tamanho, cor da tinta e espessura da fonte original.

🚀 Principais Funcionalidades

🎯 Autocalibração de Fonte e Fundo por Pixels: Ao selecionar um termo na imagem, o algoritmo analisa os pixels da região para detectar automaticamente a cor exata do papel (máscara de cobertura), o tom da tinta impressa, a altura real das letras em pixels e a densidade do traço (Normal vs. Negrito).

🔤 Detecção Nativa de Fontes + Upload .TTF / .OTF:

Suporte à API nativa do navegador (queryLocalFonts) para listar fontes instaladas no computador.

Importação direta de arquivos de fonte personalizados (.ttf, .otf, .woff).

☑️ Marcação Rápida de Caixa de Seleção (Marcar "X" em 1 Clique):

Basta clicar dentro de qualquer caixinha vazia [ ] ou ( ) do documento para detectar suas bordas, centralizar automaticamente um X, x ou ✓ na cor da tinta do documento e manter o fundo transparente para não apagar as linhas do formulário.

📊 Dados em Lote Editáveis ({{Variáveis}}):

Crie, edite ou exclua variáveis globais pela interface. Alterando o valor uma única vez na aba Dados em Lote, todas as páginas que utilizam aquela tag são atualizadas em tempo real.

📅 Variável {{Data}} Automática:

Sincroniza automaticamente com a data atual do sistema sempre que o programa é aberto, permitindo alternar entre os formatos DD/MM/AAAA, DD/MM/AA ou data por extenso (com opção de trava manual).

🖱️ Edição Rápida e Intuitiva:

Arraste para mover ou redimensionar caixas mapeadas.

Exclua qualquer caixa instantaneamente clicando com o botão direito do mouse sobre ela ou pressionando as teclas Delete / Backspace.

Botão "Segure p/ Ver Original" para comparar o documento antes e depois das edições.

Replique uma caixa mapeada para a mesma posição em todas as páginas com 1 clique.

💾 Moldes Reutilizáveis (.json):

Exporte e importe o mapeamento das caixas e variáveis em um arquivo .json leve para reutilizar diariamente nos mesmos modelos de documentos.

🖨️ Gerador de PDF Multipágina e Impressão A4 Nativa:

Gera um único arquivo .pdf em alta resolução contendo quantas páginas A4 estiverem na fila.

Impressão direta formatada em 210mm x 297mm sem margens ou cabeçalhos indesejados do navegador.

🛠️ Tecnologias Utilizadas

React 18 (Interface reativa e gerenciamento de estado em tempo real)

Tailwind CSS (Estilização leve e responsiva)

HTML5 Canvas API (Análise de luminância de pixels, detecção de bordas e renderização final em alta resolução)

jsPDF (Geração client-side de documentos PDF multipágina em formato A4)

Local Font Access API & CSS Font Loading API (Detecção de fontes do sistema e carregamento de arquivos .ttf/.otf)

📦 Como Usar ou Publicar (Zero Configuração Local)

O projeto conta com uma versão Standalone (index.html) que não exige instalação de Node.js nem etapa de build:

Opção 1: Hospedar gratuitamente na Vercel / GitHub Pages

Suba o arquivo index.html para este repositório no GitHub.

Importe o repositório na Vercel ou ative o GitHub Pages nas configurações do repositório.

O sistema estará disponível online imediatamente.

Opção 2: Executar direto no computador

Baixe o arquivo index.html.

Dê dois cliques nele para abri-lo em qualquer navegador moderno (Chrome, Edge, Brave, Firefox).

📖 Guia Rápido de Uso

Adicionar Folhas A4: Na coluna esquerda, clique em Adicionar e selecione suas imagens A4 (sem limite de páginas).

Substituir um Termo: Com a ferramenta Mapear Termo ativa, clique e arraste sobre a palavra que deseja substituir na folha. Digite o novo texto ou selecione um Dado em Lote no painel direito.

Marcar Caixas Vazias [ ]: Ative o botão Marcar "X" (1 Clique) no topo e clique dentro do quadradinho vazio do formulário.

Excluir uma Caixa: Clique com o botão direito sobre qualquer caixa mapeada ou selecione-a e aperte Delete.

Salvar ou Imprimir: Clique em Gerar PDF para baixar o documento unificado ou em Imprimir A4 para enviar direto para a impressora.

📄 Licença

Este projeto está sob a licença MIT — sinta-se livre para usar, modificar e distribuir.
