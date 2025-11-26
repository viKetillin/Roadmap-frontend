# 🚀 Roadmap Frontend — React 2025 do Básico ao Avançado

# ✨ Nota

Este roadmap foi criado com base no material [roadmap.sh](https://roadmap.sh/react),
e recebeu diversas atualizações pessoais para refletir o que considero essencial para a prática moderna de desenvolvimento front-end e preparação para entrevistas internacionais.

Ele combina fundamentos sólidos, conceitos avançados de React 18/19, padrões arquiteturais, performance, acessibilidade e tópicos complementares que eu acredito serem indispensáveis para um desenvolvedor(a) completo(a) em 2025.

# 🧭 Legenda dos ícones
🔺 Alta prioridade – Tópicos essenciais para dominar React moderno e passar em entrevistas internacionais.
🔻 Baixa prioridade – Conteúdos úteis, mas opcionais ou pouco cobrados.
(sem ícone) Prioridade média – Importante, mas não urgente.

# 1. CLI Tools
## Conceitos essenciais 🔺
- Bundler
- Dev Server
- HMR (Hot Module Replacement)
- Transpilation
- Minification
- Tree-shaking
- Code splitting

## Vite
- O que é
- Quando usar
- Como funciona superficialmente (esbuild no dev + rollup no build)

---

# 2. React Fundamentals
## Functional components 🔺
- O que é
- Função pura
- Recebe props
- Idempotência no render
- Porque migramos de classes para funções
- Como o React invoca um componente funcional
- Re-render: quando e por quê?

## JSX 🔺
- JSX não é HTML
- Açúcar sintático para React.createElement
- Cada elemento = Virtual DOM Node
- { } para expressões JS
- Por que `className`

## Props VS State 🔺
- Props são imutáveis
- State é mutável via setState
- Comunicação pai -> filho
- Ambos causam re-render

### Perguntas clássicas de entrevista 🔺
- Por que não posso modificar props?
- Por que React re-renderiza quando o state muda?
- Diferença entre controlled e uncontrolled?

## Conditional Rendering
- &&
- Ternário
- If/else antes do return
- Retornar null
- Guard clauses
- Fallback UI
- Impacto no diff

---

# 3. Components Advanced
## Controlled vs Uncontrolled Components 🔺
- Controlled inputs
- Uncontrolled inputs
- forwardRef em inputs
- Integrando com React Hook Form
- Debounced inputs

## Composition 🔺
- Children
- Render Props
- Compound Components
- Slot Pattern
- Provider Pattern
- Controlled Props Pattern
- State Reducer Pattern
- Composition > Inheritance

---

# 4. Rendering (Modern React 18+) 🔺

## Core Rendering Topics 🔺
- Lifecycle moderno (não classes!)
- Lists & Keys

## Reconciliation (Diff Algorithm) 🔺
- Como React compara árvores
- Por que keys importam
- Quando React recria um componente
- Problemas ao usar index como key

## Rendering Cycle (Render vs Commit Phase) 🔺
- Render phase = pura
- Commit phase = DOM atualizado
- Por que useEffect roda após commit
- Scheduling
- Batching automático

## Concurrent Rendering 🔺
- Pausar renderizações
- Prioridades
- Transitions
- Suspense boundaries

## Server Components (RSC) 🔺
- Client vs Server components
- O que pode ou não pode no server
- Cache
- Streaming
- Server Actions

## Refs Avançado
- DOM refs
- Valores persistentes
- forwardRef
- useImperativeHandle

## Events
- Synthetic events
- Diferenças vs DOM events

## High Order Components (HOCs) 🔻
- (Legado / opcional)

---

# 5. Hooks
## Basic Hooks 🔺
- useState
- useEffect
- useMemo
- useCallback
- useReducer
- useContext
- Custom hooks

## Hooks Best Practices 🔺
- Closures
- Stale closures
- Dependencies corretas

## Performance Optimization 🔺
- Quando usar memo
- Quando NÃO usar memo
- Problemas de closures
- Rerenders desnecessários
- Re-render boundaries

---

# 6. Routing
- React Router
- Tanstack Router
- Next.js Routing (App Router) 🔺

---

# 7. State Management
- Context
- Zustand
- Jotai
- MobX 🔻
- rtk-query (também API layer)

---

# 8. Styling
## CSS Strategies
- Tailwind CSS
- CSS Modules
- Panda CSS 🔻

## Headless UI
- Radix UI
- Ark UI
- React Aria

## Component Libraries
- Shadcn UI
- Chakra UI 🔻
- Material UI 🔻

---

# 9. API Calls
## REST 🔺
- Axios
- swr
- react-query 🔺
- rtk-query

## GraphQL
- Apollo
- Relay
- urql

---

# 10. Testing 🔺
### Unit/Integration
- Jest 🔺
- React Testing Library 🔺

### E2E
- Cypress
- Playwright

---

# 11. Frameworks
## Next.js 🔺
- App Router
- RSC
- Server Actions
- Cache
- Loading/Error states
- Routing avançado

## Outros
- Astro 🔻
- react-router

---

# 12. Forms
- React Hook Form
- Formik 🔻

---

# 13. Types e Validation
- TypeScript 🔺
- Zod 🔺

---

# 14. Animation
- Framer Motion
- React Spring
- GSAP 🔻

---

# 15. Advanced Topics
- Error Boundaries 🔺
- Server APIs
- Suspense 🔺
- Portals 🔺

---

# 16. Accessibility (A11y) 🔺
- Semantic HTML
- Roles
- aria-* attributes
- Keyboard navigation
- Focus management
- Skip links
- A11y testing (axe-core)

---

# 17. Internationalization (i18n)
- next-intl
- react-intl
- i18next
- Message extraction
- Date/number formatting

---

# 18. Web Performance 🔺
- Hydration
- Partial hydration
- Streaming SSR
- Lazy loading
- Bundle analysis
- Route-level code splitting
- Image optimization
- Core Web Vitals
- Lighthouse

---

# 19. Frontend Security 🔺
- XSS
- CSRF
- Sanitização de inputs
- Escape de HTML
- Cookies HttpOnly / SameSite
- OWASP Top 10 (focado em frontend)
