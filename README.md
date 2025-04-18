# 🛠️ Frontend Dev Tools

Minha coleção de ferramentas essenciais.  

## 📋 Índice
- [Layout & CSS](#layout--css)
- [Animações](#animações)
- [Frameworks](#frameworks)
- [Mídia](#mídia)
- [IA & Assistência](#ia--assistência)
- [Ambiente Dev](#ambiente-dev)

## Layout & CSS

### Flexboxgrid
```html
<div class="row">
  <div class="col-xs-12 col-sm-6 col-md-4">Responsivo</div>
</div>
```
Sistema de grid baseado em flexbox para layouts responsivos. [Documentação](http://flexboxgrid.com/)

### BEM CSS
```css
.card {} /* Bloco */
.card__title {} /* Elemento */
.card--featured {} /* Modificador */
```
Metodologia para nomes de classes organizados e escaláveis.

### SASS/SCSS
```scss
@mixin respond-to($breakpoint) {
  @if $breakpoint == "small" { @media (max-width: 576px) { @content; } }
}
```
Pré-processador com variáveis, mixins e aninhamento.

### Tailwind CSS
```html
<div class="max-w-sm rounded shadow-lg bg-white p-4">
  <h2 class="text-xl font-bold mb-2">Título</h2>
  <p class="text-gray-700">Conteúdo</p>
</div>
```
Framework de classes utilitárias para desenvolvimento rápido.

## Animações

### GSAP
```javascript
gsap.to(".elemento", {
  duration: 1,
  x: 100,
  opacity: 0.5,
  scrollTrigger: { trigger: ".section", scrub: true }
});
```
Engine de animação profissional com controle refinado.

### AOS Animate
```html
<div data-aos="fade-up" data-aos-delay="300">Anima ao entrar no viewport</div>
```
Biblioteca simples para animar elementos durante o scroll.

### Goo Motion Library
```html
<div goo-motion="fade-up" goo-duration="1">Animação baseada em GSAP para Webflow</div>
```
Animações sem código para Webflow usando atributos personalizados.

## Frameworks

### Next.js
```javascript
// App Router (moderno)
// app/page.js
export default function Home() {
  return <h1>Hello Next.js</h1>
}
```
Framework React com roteamento, SSR e otimizações de performance.

## Mídia

### Video.js
```javascript
const player = videojs('my-video', {
  controls: true,
  fluid: true,
  sources: [{ src: '/video.mp4', type: 'video/mp4' }]
});
```
Player de vídeo personalizável e responsivo.

## IA & Assistência

### Claude
Assistente de IA para geração de código, refatoração e ideação.

### Mindsurf
Sugestões de código em tempo real integradas ao editor.

### V0 (Vercel)
Transformação de designs em código React/Vue/HTML.

### ChatGPT
Assistente para revisões de código e soluções técnicas.

## Ambiente Dev

### Cursor
Editor com recursos de IA para autocompletar e sugestões.

### VSCode
```json
{
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode"
}
```
Extensões essenciais: ESLint, Prettier, GitLens, Live Server

---

## Licença
MIT
