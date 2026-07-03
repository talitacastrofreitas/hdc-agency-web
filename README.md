# 🌐 hDC Agency - Landing Page com Bootstrap 5
Um projeto completo de landing page institucional desenvolvido para a agência digital fictícia **hDC Agency - A sua agência web**. O objetivo deste projeto é demonstrar a integração do framework **Bootstrap 5** com bibliotecas JavaScript externas para criar uma experiência rica em interatividade, incluindo efeitos de paralaxe, barras de progresso circulares animadas e filtragem de portfólio em tempo real.

---
## 🎯 Seções da Landing Page
- **Cabeçalho Fixo (Navbar):** Menu de navegação superior responsivo com efeito translúcido que permanece visível durante a rolagem.
- **Destaque (Carousel):** Slider de imagens responsivo ocupando `80vh` da tela, com textos explicativos e botões de chamada para ação (CTA).
- **Sobre a Agência:** Seção informativa com imagem ilustrativa e uma listagem de diferenciais com ícones personalizados.
- **Especialidades (Serviços):** Grid adaptável mostrando as áreas de atuação (Aplicativos Nativos, E-commerces, Design UI/UX, SEO, Suporte e Servidores).
- **Dados Estatísticos:** Contador numérico interativo de projetos entregues, clientes satisfeitos, colaboradores e xícaras de café, animado dinamicamente com base na rolagem da página.
- **Time de Colaboradores:** Exibição da equipe em cards responsivos com fotos e cargos.
- **Trabalhe Conosco:** Chamada para recrutamento com vagas abertas na agência.
- **Portfólio Interativo:** Galeria de projetos com filtro funcional em tempo real para categorias de Desenvolvimento, Design e SEO.
- **Newsletter & Orçamentos:** Captação de e-mails para conteúdo e CTA para solicitação de cotações.
- **Contato:** Informações físicas de atendimento e formulário de mensagem estruturado.
---
## 📂 Estrutura de Arquivos
```bash
Projeto-Bootstrap/
├── css/
│   └── style.css         # Customizações CSS que expandem os estilos padrão do Bootstrap
├── img/
│   ├── agencia.jpg       # Foto para a seção 'Sobre'
│   ├── banner1.png       # Slide 1 (E-commerce)
│   ├── banner2.png       # Slide 2 (Engenharia de Software)
│   ├── banner3.png       # Slide 3 (Manutenção)
│   ├── cidadeparallax.png# Fundo com efeito parallax da seção de dados
│   ├── pattern.png       # Fundo com efeito parallax da seção 'Trabalhe Conosco'
│   ├── profile1-4.jpg    # Fotos do perfil do time
│   ├── proj1-6.jpg       # Capturas de tela para a galeria de portfólio
│   └── hdcagency_logo.svg# Logotipo vetorial da marca
├── js/
│   ├── progressbar.min.js# Biblioteca local ProgressBar.js para animações dos círculos
│   └── scripts.js        # Script customizado (inicialização do parallax, lógica de filtros e barra de progresso)
├── index.html            # Estrutura HTML principal e importação de CDNs
└── README.md             # Documentação do projeto
```
---
## 🛠️ Tecnologias & Bibliotecas Utilizadas
- **Bootstrap 5 (v5.3.0-alpha1):** Utilizado para o grid responsivo, Navbar de navegação móvel, componentes de Carousel, Cards e formulários.
- **jQuery 3.6.3 (via CDN):** Manipulação de elementos no DOM, controle dos filtros de portfólio e detecção de scroll da página.
- **ProgressBar.js:** Biblioteca especializada para renderização dos círculos estatísticos animados (`circleA`, `circleB`, `circleC`, `circleD`).
- **Parallax.js:** Script para efeito de paralaxe na imagem de fundo de seções específicas.
- **FontAwesome (Icons):** Coleção completa de ícones vetoriais corporativos e sociais.
- **Google Fonts (Roboto):** Tipografia padrão integrada.
---
## ⚙️ Funcionamento das Lógicas JavaScript (`js/scripts.js`)
1. **Círculos de Progresso:** A animação dos contadores numéricos (que vão de zero até o valor alvo de cada métrica) só é disparada quando o usuário rola a página e atinge a seção `#data-area` (`dataAreaOffset`).
2. **Efeito Paralaxe:** Aplicado com atraso controlado (`setTimeout` de 250ms) nas imagens `cidadeparallax.png` e `pattern.png` para garantir o carregamento correto do grid.
3. **Filtro de Portfólio:** A função `eachBoxes` oculta de forma suave (`fadeOut`) os elementos que não pertencem à categoria clicada e destaca (`fadeIn`) os correspondentes (`dev`, `dsg` ou `seo`).
---
## 💻 Como Rodar o Projeto
Como este projeto é puramente estático no front-end, basta abri-lo localmente:
1. Clone este repositório ou baixe os arquivos em sua máquina.
2. Dê um duplo clique no arquivo `index.html` para executá-lo diretamente no seu navegador.
3. Certifique-se de estar conectado à internet, pois as bibliotecas Bootstrap, jQuery, FontAwesome e Parallax.js são importadas via CDNs (links externos).
