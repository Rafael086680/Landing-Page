# VitaPet Veterinária

Portal do tutor para acompanhamento de pets — projeto acadêmico desenvolvido com HTML5 e CSS3 puro.

---

## Sobre o Projeto

O **VitaPet** é uma landing page que simula o portal de um tutor de pets em uma clínica veterinária. O usuário Rafael Rodrigues pode visualizar o próprio perfil, as fichas completas dos seus três animais, consultas agendadas e uma galeria de fotos — tudo em uma interface responsiva e acessível.

Projeto desenvolvido para a disciplina **Ferramentas Web e UX — HTML5 & CSS3** do 1º semestre de 2026 na **Católica SC de Jaraguá do Sul**.

---

## Seções da Página

| Seção | Descrição |
|---|---|
| **Hero / Destaque** | Boas-vindas personalizadas com card de resumo do perfil do tutor |
| **Meu Perfil** | Dados pessoais, endereço e veterinário responsável em cards |
| **Meus Pets** | Fichas completas de Sheik (Bull Terrier), Missinha e Paulinho (SRD) |
| **Agenda** | Próximas consultas com status (confirmado, pendente, urgente) |
| **Galeria** | Grade de fotos em layout assimétrico com efeito de zoom no hover |
| **Contato** | Endereço, telefone e card de agendamento rápido |

---

## Destaques Técnicos

- **CSS Custom Properties** (`--verde`, `--laranja`, `--raio-xl`…) para padronização de cores, sombras e arredondamentos em todo o site
- **Layout com CSS Grid e Flexbox** — grade responsiva que se adapta de desktop a celular sem JavaScript
- **Animações CSS puras** — bolhas flutuantes com `@keyframes`, cards que sobem ao carregar (`subir`), zoom nas fotos da galeria e linha de hover nos links do menu
- **Cabeçalho sticky** com `backdrop-filter: blur` (efeito vidro fosco)
- **Pseudo-elementos** (`::before`, `::after`) para decorações como a faixa de patinhas e as linhas do card de perfil — sem tags extras no HTML
- **Semântica HTML5** — uso correto de `<article>`, `<section>`, `<aside>`, `<address>`, `<dl>/<dt>/<dd>`, `<time>` e atributos `aria-label` / `aria-hidden`
- **Tipografia responsiva** com `clamp()` — títulos crescem e diminuem fluidamente com a tela
- **Design responsivo** com dois breakpoints (`@media max-width: 900px` e `600px`)

---

## Estrutura de Arquivos

```
vitapet/
├── index.html
├── style.css
└── assets/
    ├── pata.jpg              # ícone da patinha no logo
    ├── ediatr.jpg            # ícone do botão de editar foto
    ├── cattt.png             # textura de patinhas (fundo da seção Perfil)
    ├── dadoscat.jpg          # imagem do card Dados Pessoais
    ├── homecat.jpg           # imagem do card Endereço
    ├── doctorcat.jpg         # imagem do card Vet Responsável
    ├── sheikavatar.jpg       # foto do pet Sheik
    ├── missinha.jpg          # foto da pet Missinha
    ├── paulinho.png          # foto do pet Paulinho
    ├── fotomissi.jpg         # galeria — foto grande
    ├── pauli1.jpg            # galeria
    ├── missi2.jpg            # galeria
    ├── missi3.jpg            # galeria
    └── paulinho2.jpg         # galeria
```

---

## Como Rodar Localmente

Não há dependências ou build steps. Basta clonar e abrir:

```bash
git clone https://github.com/seu-usuario/vitapet.git
cd vitapet
```

Abra o arquivo `index.html` diretamente no navegador, ou use a extensão **Live Server** no VS Code para recarregamento automático.

> As imagens da pasta `assets/` são necessárias para a exibição correta do layout. Certifique-se de que a pasta está junto com o `index.html`.

---

## Responsividade

| Breakpoint | Comportamento |
|---|---|
| `> 900px` | Layout completo em duas colunas |
| `≤ 900px` | Cards empilhados, fichas de pets com foto no topo, galeria em 2 colunas |
| `≤ 600px` | Menu oculto, galeria e cards em coluna única |

---

## Tecnologias

- **HTML5** — estrutura semântica
- **CSS3** — Grid, Flexbox, Custom Properties, animações, media queries
- **Google Fonts** — Playfair Display (títulos) + DM Sans (texto)

Sem frameworks, sem JavaScript, sem bibliotecas externas.

---

## Autor

**Rafael Rodrigues Antonio**  
Disciplina: Ferramentas Web e UX — HTML5 & CSS3  
1º Semestre / 2026 · Católica SC — Jaraguá do Sul
