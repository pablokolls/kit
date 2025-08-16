# 5. Building Block View

## 5.1 Level 1 (System Overview – C4 Container Diagram)
- **Kit Customization App**
  - Admin Extension (Polaris UI)
  - Theme Extension (Liquid component)
  - Remix Backend API
  - PostgreSQL Database

## 5.2 Level 2 (Main Components – C4 Component Diagram)
- **Remix Backend**
  - Auth Controller (Shopify OAuth)
  - Admin API Controller (customization config)
  - Storefront API Proxy (fetch product data, stock, pricing)
  - Validation Module (blacklist checks, input sanitization)
  - Persistence Layer (Prisma + PostgreSQL)

- **Admin Extension**
  - Config UI
  - Product Selection
  - Customization Rules Management

- **Theme Extension**
  - UI Renderer (Liquid block)
  - Cart Integration
  - Live Preview

## 5.3 Level 3 (Code/Modules – C4 Code Diagram)
- Prisma schema (models: Product, CustomizationOption, Blacklist, UserRoles)
- Liquid components (CustomizerUI, Preview, CartButton, OptionSelector)
- Node.js services (AuthService, ValidationService, ProductService)
