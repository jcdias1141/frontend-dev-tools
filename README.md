# Frontend Dev Tools

Repositório de ferramentas e dicas para desenvolvimento frontend baseado em 6 anos de experiência.

## 📋 Índice

- [CSS](#css)
- [Animações](#animações)
- [Mídia](#mídia)
- [Ferramentas de IA](#ferramentas-de-ia)
- [Editores de Código](#editores-de-código)
- [Workflows & Produtividade](#workflows--produtividade)

## CSS

### Flexbox & Grid

```css
/* Flexbox básico */
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

/* Grid básico */
.grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 20px;
}
```

**Recursos:** [Flexbox Froggy](https://flexboxfroggy.com/), [Grid Garden](https://cssgridgarden.com/)

### BEM CSS

```css
/* Bloco */
.card {}
/* Elemento */
.card__title {}
/* Modificador */
.card--featured {}
```

### SASS/SCSS

```scss
// Mixin para breakpoints
@mixin respond-to($breakpoint) {
  @if $breakpoint == "small" {
    @media (max-width: 576px) { @content; }
  } @else if $breakpoint == "medium" {
    @media (max-width: 768px) { @content; }
  }
}

.element {
  width: 50%;
  @include respond-to(small) { width: 100%; }
}
```

## Animações

### GSAP

```javascript
// Animação básica
gsap.to(".element", {
  duration: 1,
  x: 100,
  rotation: 360,
  ease: "power2.inOut"
});

// ScrollTrigger
gsap.to(".parallax-element", {
  y: 100,
  scrollTrigger: {
    trigger: ".section",
    scrub: true
  }
});
```

### AOS Animate

```html
<div data-aos="fade-up">Anima de baixo para cima</div>
<div data-aos="fade-down" data-aos-delay="300">Com delay</div>
```

## Mídia

### Video.js

```javascript
const player = videojs('my-video', {
  controls: true,
  autoplay: false,
  fluid: true,
  responsive: true
});
```

## Ferramentas de IA

### Claude
- **Uso:** Geração de código, debugging, refatoração, documentação
- **Prompts:** Forneça contexto detalhado e exemplos do resultado desejado

### Mindsurf
- **Uso:** Sugestões de código em tempo real, assistência no debugging

### V0 (Vercel)
- **Uso:** Transformação de designs em código, geração de componentes

### ChatGPT
- **Uso:** Revisões de código, implementações de algoritmos, brainstorming

## Editores de Código

### Cursor
- **Foco:** Integração com IA, autocompletar avançado

### VSCode

**Extensões essenciais:**
- ESLint, Prettier, Auto Rename Tag, Live Server, GitLens

**Atalhos úteis:**
- `Ctrl+P` - Navegação rápida
- `Alt+↑/↓` - Mover linha
- `Ctrl+D` - Selecionar próxima ocorrência
- `Ctrl+/` - Comentar/descomentar

## Workflows & Produtividade

- **Git:** Branches por feature, commits semânticos
- **Performance:** Lazy loading, otimização de imagens, code splitting
- **CI/CD:** GitHub Actions, Vercel, Netlify

---

## Licença
MIT
