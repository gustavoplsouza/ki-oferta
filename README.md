# KiOferta · WebApp de Ofertas (Estudo de Caso & Atividade Bônus)

Este repositório contém o desenvolvimento da **Tela Inicial (Vitrine de Produtos)** do webapp **KiOferta**, estruturado em HTML5 e estilizado com CSS3 puro (Flexbox) e integração investigativa com o framework CSS **Bulma**. 

O projeto foi projetado e testado para responsividade total em telas móveis com largura a partir de **360px** a **420px**, sem geração de barra de rolagem horizontal.

---

## Parte A · Pesquisa sobre o Framework CSS (Bulma)

### A1. O que é o framework e qual abordagem ele segue?
O **Bulma** é um framework CSS moderno, gratuito e open-source, construído inteiramente com base na especificação **Flexbox**. Ele segue uma abordagem baseada em **componentes visuais e classes utilitárias puramente CSS**, o que significa que não inclui nem exige dependências de scripts JavaScript. Sua filosofia de design é orientada ao desenvolvimento *mobile-first*, fornecendo uma sintaxe declarativa e semântica (como `.button`, `.card`, `.columns`) para acelerar a estruturação de interfaces web.

### A2. Como você incluiu o framework na página?
O framework foi incluído na aplicação através da importação da sua folha de estilo oficial via CDN (Content Delivery Network). Adicionamos a seguinte tag `<link>` dentro da seção `<head>` do arquivo `index.html`:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css">
```

### A3. Três benefícios percebidos ao usar
1. Agilidade no alinhamento de layouts complexos usando o sistema de colunas baseado em Flexbox (.columns e .column) permite criar layouts responsivos sem a necessidade de escrever regras manuais de largura.
2. Padronização Rápida de Componentes: Elementos como botões, cards de produtos e formulários já vêm com espaçamentos, tipografia e estados visuais pré-ajustados.
3. Leitura Clara do Código HTML: A nomenclatura das classes é intuitiva (ex.: .button, .is-primary, .has-text-centered), facilitando a manutenção em grupo.

### A4. Duas limitações ou desvantagens
1. Aparência Genérica: Sem customização aprofundada, a aplicação assume o visual padrão compartilhado por diversos outros sites que usam o framework.
2. Atrito para Sobrescrever Estilos: Dificuldade e excesso de código necessários para sobrescrever estilos padrões quando o projeto já possui um guia de estilo próprio (cores, fontes e espaçamentos fixos).

### A5. Uso de Classes vs IDs no CSS do Framework
Ao inspecionar o CSS do Bulma (via DevTools F12), observa-se o uso exclusivo de classes (.card, .title, .button). Os frameworks preferem classes porque elas permitem reutilização em múltiplos elementos da página e possuem menor especificidade no CSS, facilitando a aplicação repetida de estilos sem travar a customização.

### A6. Fontes consultadas
- Documentação Oficial do Bulma: https://bulma.io/documentation/ (Acesso em: 10/09/2026)
- MDN Web Docs - CSS Selectors: https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors (Acesso em: 10/09/2026)