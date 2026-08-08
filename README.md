# PHP Master Hub — Interactive Learning Platform

A comprehensive, interactive PHP 8.x learning ecosystem built as a static site with 22 specialized modules covering the entire modern PHP development landscape.

## 🌟 Overview

PHP Master Hub is a self-contained, client-side interactive documentation and learning platform featuring:
- **22 Interactive Modules** across 7 knowledge domains
- **Slide-based presentations** with D3.js visualizations, Mermaid diagrams, and live code simulators
- **Dark/Light theme** with persistent preferences
- **Full-text search** across all content
- **Progress tracking** with localStorage persistence
- **Offline-capable** — no backend required

## 📚 Module Catalog

### 1. Core Language & Modern Syntax (`core-language-modern-features/`)
| Module | File | Key Topics |
|--------|------|------------|
| Modern PHP Syntax | `modern-php-syntax-presentation.html` | `match` expressions, named arguments, nullsafe operator `?->`, `readonly` properties, arrow functions |
| Type System & Strict Types | `type-system.html` | Union/Intersection/DNF types, `strict_types`, variance, type juggling, live type checker simulator |
| Advanced Control Flow | `advanced-control-flow.html` | Generators (`yield`), iterators, optimized conditionals, loop control |
| PHP 8 Attributes | `attributes.html` | `#[Attribute]` metadata, reflection, replacement for DocBlocks |

### 2. Programming Paradigms (`programming-paradigms/`)
| Module | File | Key Topics |
|--------|------|------------|
| Advanced OOP | `advanced-oop.html` | Backed enums, traits, readonly classes, interfaces, polymorphism |
| Functional Programming | `functional-programming.html` | `fn()` arrow functions, immutability, `array_map/filter/reduce`, currying, `Closure::bind` |
| Metaprogramming & Reflection | `metaprogramming.html` | Reflection API, dynamic proxies, runtime code inspection |

### 3. Architecture & Design Patterns (`architecture-design-patterns/`)
| Module | File | Key Topics |
|--------|------|------------|
| MVC & Separation of Concerns | `mvc-separation-concerns.html` | Layered architecture, controller/service/repository pattern |
| SOLID Principles | `solid-principles.html` | All 5 principles with PHP 8.x code, interactive architecture analyzer, UML diagrams |
| Dependency Injection | `dependency-injection.html` | Constructor injection, PSR-11 containers, service locator vs DI |

### 4. Security & Data Integrity (`security-data-integrity/`)
| Module | File | Key Topics |
|--------|------|------------|
| Web Security Essentials | `security.html` | XSS, CSRF, SQL injection prevention, CSP, secure headers |
| Defensive Coding | `defensive-coding.html` | Input validation, fail-safe defaults, error handling without leakage |
| Cryptography & Hashing | `cryptography.html` | `password_hash`, `sodium_*`, encryption, signing, key derivation |

### 5. Infrastructure, Tooling & Performance (`infraestructure-tooling-performance/`)
| Module | File | Key Topics |
|--------|------|------------|
| Dependency Management | `dependency-management.html` | Composer, version constraints, autoload optimization, scripts |
| Performance Optimization | `performance-optimization.html` | OPcache, JIT, profiling (Blackfire/Xdebug), caching strategies |
| Observability & Logging | `observability.html` | PSR-3, Monolog, structured logging, metrics, tracing |
| Deployment Environments | `deployment-environments.html` | CI/CD, Docker, Kubernetes, serverless, zero-downtime deployments |

### 6. Testing & Quality Standards (`testing-quality-standards/`)
| Module | File | Key Topics |
|--------|------|------------|
| PHP-FIG Standards (PSR) | `phpfig-standards.html` | PSR-1,4,7,11,12,14,17,18 — coding style, containers, HTTP messages |
| Static Analysis Tools | `static-analysis.html` | PHPStan, Psalm, Rector, type coverage, baseline management |
| Automated Testing | `automated-testing.html` | PHPUnit, Pest, mocking, test doubles, TDD/BDD, mutation testing |

### 7. Documentation & Community (`documentation-community/`)
| Module | File | Key Topics |
|--------|------|------------|
| PHPDoc & Standard Documentation | `phpdoc.html` | DocBlock syntax, `@param`/`@return`/`@var`, IDE integration, phpDocumentor |
| PHP Lifecycle & Versioning | `lifecycle-management.html` | Release cycle, RFC process, upgrade guides, deprecation policy |

## 🚀 Quick Start

```bash
# No build step required — open directly in browser
open index.html

# Or serve locally for best experience (handles ES modules/CORS)
npx serve .
# or
php -S localhost:8000
```

## ✨ Features

### Interactive Elements
- **Live Type Checker Simulator** — Test PHP type coercion vs strict mode in real time
- **D3.js Type Hierarchy Tree** — Clickable visualization of PHP's type system
- **Mermaid Architecture Diagrams** — Dynamic class/sequence diagrams
- **SOLID Architecture Analyzer** — Toggle traits to compute compliance scores
- **Code Playgrounds** — Edit and simulate PHP snippets client-side
- **Knowledge Quizzes** — Per-module assessments with explanations

### UX & Accessibility
- **Keyboard Navigation** — `Ctrl+K` search, arrow keys for slides, `Esc` to close modals
- **Theme Persistence** — Remembers dark/light preference
- **Progress Tracking** — Marks topics as "visited" in localStorage
- **Responsive Design** — Mobile-first with collapsible navigation drawer
- **Copy-to-Clipboard** — One-click code copying on all snippets

### Technical Stack
- **Vanilla ES6+ JavaScript** — No framework dependencies
- **Tailwind CSS (CDN)** — Utility-first styling with custom design tokens
- **Prism.js** — Syntax highlighting for PHP
- **D3.js** — Data-driven SVG visualizations
- **Mermaid.js** — Markdown-style diagrams
- **Font Awesome 6** — Iconography
- **Google Fonts (Inter, JetBrains Mono)** — Typography

## 📁 Project Structure

```
php-learning/
├── index.html                                    # Main hub / dashboard
├── core-language-modern-features/                # Module 1 (4 topics)
│   ├── modern-php-syntax-presentation.html
│   ├── type-system.html
│   ├── advanced-control-flow.html
│   └── attributes.html
├── programming-paradigms/                        # Module 2 (3 topics)
│   ├── advanced-oop.html
│   ├── functional-programming.html
│   └── metaprogramming.html
├── architecture-design-patterns/                 # Module 3 (3 topics)
│   ├── mvc-separation-concerns.html
│   ├── solid-principles.html
│   └── dependency-injection.html
├── security-data-integrity/                      # Module 4 (3 topics)
│   ├── security.html
│   ├── defensive-coding.html
│   └── cryptography.html
├── infraestructure-tooling-performance/          # Module 5 (4 topics)
│   ├── dependency-management.html
│   ├── performance-optimization.html
│   ├── observability.html
│   └── deployment-environments.html
├── testing-quality-standards/                    # Module 6 (3 topics)
│   ├── phpfig-standards.html
│   ├── static-analysis.html
│   └── automated-testing.html
└── documentation-community/                      # Module 7 (2 topics)
    ├── phpdoc.html
    └── lifecycle-management.html
```

## 🎯 Learning Path Recommendations

### Beginner → Intermediate
1. **Core Language** (4 topics) — Master PHP 8.x syntax & type system
2. **Programming Paradigms** (3 topics) — OOP, Functional, Metaprogramming
3. **Testing & Quality** (3 topics) — PSR standards, static analysis, automated testing

### Intermediate → Advanced
4. **Architecture & Patterns** (3 topics) — SOLID, MVC, Dependency Injection
5. **Security & Data** (3 topics) — Web security, defensive coding, cryptography
6. **Infrastructure & Performance** (4 topics) — Composer, optimization, observability, deployment

### Reference & Maintenance
7. **Documentation & Community** (2 topics) — PHPDoc, PHP lifecycle management

## 🔧 Customization

### Adding a New Topic
1. Create new `.html` file in appropriate module directory
2. Follow existing slide-wrapper pattern with `data-category` and `data-doc` attributes
3. Add entry to `index.html`:
   - Grid card in `#topicsGrid`
   - Navigation dropdown item
   - Mobile drawer link
4. Update topic count badges (22 → 23)

### Theming
Edit `tailwind.config` in any HTML file to customize:
- Color palette (`colors.php.*`, `colors.neon.*`)
- Font families
- Animations

## 📖 Source Attribution

All technical content is grounded in official PHP documentation:
- [php.net/manual](https://www.php.net/manual) — Language specification
- [PHP-FIG PSRs](https://www.php-fig.org/psr/) — Standards
- [PHP RFCs](https://wiki.php.net/rfc) — Feature proposals

Each module includes a "Grounded in Official Manual" chip linking to the authoritative source.

## 🤝 Contributing

This is a personal learning project, but improvements are welcome:
1. Fork the repository
2. Add/correct content following existing patterns
3. Ensure vanilla JS compatibility (no build step)
4. Test in both light/dark modes and mobile/desktop
5. Submit PR with description of changes

## 📄 License

MIT License — Free for personal and educational use.

---

**Built with ❤️ by Freen Jimenez** • Last updated: 2026