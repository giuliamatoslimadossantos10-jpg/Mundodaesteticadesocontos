# Mundo da Estética — Portal de Descontos & Benefícios

Landing page (página de aterrissagem) única e interativa para o **Mundo Estética**, um clube de benefícios que reúne descontos, cupons e vantagens para cursos profissionais de estética e lojas parceiras.

## Visão Geral

O projeto é uma página web única (single-page) construída com **HTML5**, **Tailwind CSS** (via CDN) e **JavaScript vanilla** (sem frameworks). Ele oferece uma experiência gamificada e interativa para o usuário descobrir descontos em cursos de estética.

### Funcionalidades Principais

- **Roda da Sorte (Roleta Interativa):** Uma roleta SVG animada com 5 setores que sorteia um cupom de desconto garantido ao girar. O prêmio é exibido dinamicamente com opção de copiar o código.
- **Simulador de Economia Infinity:** Calculadora interativa que compara o preço de cursos avulsos selecionáveis com a assinatura Infinity (R$ 1.044/ano), mostrando a economia em tempo real.
- **Catálogo de Cursos Promocionais:** Grid de 3 cards de cursos com imagem, descrição, preço antigo (riscado), preço promocional e botão que abre um modal de confirmação de desconto.
- **Cupons de Parceiros:** Cards com códigos de cupom de lojas parceiras (Mundo do Cabeleireiro, Shopee) com botão de copiar para a área de transferência.
- **Sistema de Notificações Toast:** Feedback visual temporário no canto inferior direito ao copiar cupons ou girar a roleta.
- **Modal de Promoção:** Overlay modal ao clicar em "Ver Desconto" nos cursos, com preço promocional e link para matrícula.

## Estrutura do Projeto

```
Mundodaesteticadesocontos/
├── README.md                    # Este arquivo
├── mundoesteticadescontos       # Página HTML única (sem extensão)
└── .github/                     # Configurações do GitHub
```

> **Nota:** O arquivo principal `mundoesteticadescontos` não possui extensão `.html`, mas é um documento HTML5 completo e pode ser aberto diretamente em qualquer navegador.

## Tecnologias Utilizadas

| Tecnologia | Função |
|---|---|
| **HTML5** | Estrutura semântica da página |
| **Tailwind CSS** | Framework de estilização utilitária (via CDN) |
| **JavaScript (Vanilla)** | Interatividade e lógica de negócio |
| **SVG** | Desenho vetorial da roleta de prêmios |
| **Google Fonts (Inter)** | Tipografia principal |
| **FontAwesome 6.4.0** | Biblioteca de ícones |
| **Unsplash** | Imagens dos cards de cursos (com fallback) |

## Seções da Página

1. **Navbar** — Barra de navegação fixa com logo, links internos e CTA
2. **Hero** — Cabeçalho de destaque com título, botões de ação, estatísticas e card promocional da Assinatura Infinity
3. **Roda da Sorte** — Roleta interativa SVG com 5 prêmios e botão de giro
4. **Simulador de Economia** — Calculadora dinâmica de comparação de preços
5. **Catálogo de Cursos** — Grid de 3 cards de cursos com preços promocionais
6. **Cupons de Parceiros** — Grid de 3 cards de cupons com botão de copiar
7. **Footer** — Rodapé com navegação, contato e copyright
8. **Toast** — Notificação flutuante (oculta por padrão, controlada via JS)
9. **Modal** — Overlay de promoção (oculto por padrão, controlado via JS)

## Funções JavaScript

| Função | Descrição |
|---|---|
| `copyToClipboard(text)` | Copia texto para a área de transferência usando `execCommand('copy')` |
| `showToast(title, message)` | Exibe notificação toast por 4 segundos |
| `spinWheel()` | Sorteia prêmio, anima a roleta e exibe o resultado |
| `calculateSavings()` | Calcula economia em tempo real ao marcar/desmarcar cursos |
| `openPromoModal(courseName, price)` | Abre o modal de promoção com dados do curso |
| `closePromoModal()` | Fecha o modal de promoção |
| `window.onload` | Executa cálculo inicial ao carregar a página |

## Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/giuliamatoslimadossantos10-jpg/Mundodaesteticadesocontos.git
   ```
2. Abra o arquivo `mundoesteticadescontos` diretamente em qualquer navegador moderno (Chrome, Firefox, Edge, Safari).
3. Não é necessário servidor local, build ou instalação de dependências — tudo funciona via CDN.

## Paleta de Cores (Tema "Aesthetic")

| Token | HEX | Uso |
|---|---|---|
| `aesthetic-50` | `#FDF8F5` | Fundo suave |
| `aesthetic-100` | `#FBEFEA` | Fundos de seção |
| `aesthetic-200` | `#F7DEC3` | Seleção de texto |
| `aesthetic-300` | `#E9C49A` | Decorativo |
| `aesthetic-400` | `#D49B6A` | Detalhes |
| `aesthetic-500` | `#C17B4B` | Botões |
| `aesthetic-600` | `#A75D35` | Hover states |
| `aesthetic-700` | `#8A4526` | Textos de destaque |
| `aesthetic-gold` | `#C5A880` | Dourado principal |
| `aesthetic-dark` | `#1C1917` | Fundo escuro |

## Prêmios da Roleta

| Setor | Prêmio | Cupom |
|---|---|---|
| 1 | 15% OFF na Assinatura Infinity | `INFINITY15` |
| 2 | 20% OFF Premium de Estética | `PREMIUM20` |
| 3 | Mentoria VIP Exclusiva | `MENTORIAVIP` |
| 4 | 10% de Desconto em Cursos Avulsos | `CURSOS10` |
| 5 | E-Book Oficial Grátis | `EBOOKGRATIS` |

## Licença

© 2026 Mundo Estética — Clube de Benefícios. Todos os direitos reservados.