# Implementation Plan - AVIVA Mart

AVIVA Mart is a dual-purpose marketplace for products and professional services, specifically tailored for the Nigerian market (with a focus on Ebonyi State). It features a managed inventory model where products are vetted and stocked by admins before being listed.

## User Persona & Features
- **Sellers/Providers**: List products/services. Products go to 'Pending' status.
- **Admins**: Review, accept, and stock products. Manage listings.
- **Buyers/Clients**: Browse products and services, filter by location (Nigerian states).
- **Location Focus**: Ebonyi State (priority), all other Nigerian states, and FCT.

## Proposed Tech Stack
- **Frontend**: React, Tailwind CSS, Lucide React (icons), Radix UI (components).
- **State Management**: React Context or local state for mock demo.
- **Routing**: React Router.
- **Images**: Placeholder images via Unsplash/generated.

## Phase 1: Foundation & Branding
- [ ] Set up project structure and routing (`/`, `/browse`, `/list-item`, `/admin`, `/auth`).
- [ ] Implement global layout with "AVIVA Mart" branding.
- [ ] Create a "catchy" landing page with clear value propositions for relocators and craftsmen.

## Phase 2: Location & Category Data
- [ ] Create a constant for Nigerian states with Ebonyi at the top.
- [ ] Define categories for Products (Furniture, Electronics, etc.) and Services (Painters, Event Managers, Rentals).

## Phase 3: Listing & Submission (Seller Flow)
- [ ] Create a multi-step form for "Selling a Product" (includes condition, relocation details).
- [ ] Create a form for "Registering as a Craftsman".
- [ ] Implement a "My Listings" dashboard showing "Pending" vs "Active" status.

## Phase 4: Admin Control Panel
- [ ] Create an admin view to see all pending products.
- [ ] Action buttons: "Approve & Stock" (marks as active), "Reject".
- [ ] Display the 5% commission calculation on potential sales.

## Phase 5: Marketplace & Discovery
- [ ] Main browse page with tabs for "Products" and "Services".
- [ ] Filtering system by State (Ebonyi, FCT, etc.) and Category.
- [ ] Product/Service detail pages.

## Phase 6: Polish & User Experience
- [ ] Sign-up/Login modals (simplified for demo).
- [ ] Mobile-responsive navigation.
- [ ] Visual cues for "Pending" status and "Verified" craftsmen.

## Execution Handoff

### Phase 1 & 2: Core Infrastructure
- **Agent**: `frontend_engineer`
- **Scope**: Layout, Routing, Landing Page, Nigerian State Constants.
- **Files**: `src/App.tsx`, `src/components/layout/`, `src/pages/Landing.tsx`, `src/constants/locations.ts`.

### Phase 3 & 4: Seller & Admin Workflows
- **Agent**: `frontend_engineer`
- **Scope**: Product listing forms, Service registration, Admin Dashboard UI, Approval logic (mocked).
- **Files**: `src/pages/ListProduct.tsx`, `src/pages/AdminDashboard.tsx`, `src/hooks/useListings.ts`.

### Phase 5: Marketplace & Search
- **Agent**: `frontend_engineer`
- **Scope**: Search/Filter UI, Browse page, Product/Service Cards.
- **Files**: `src/pages/Browse.tsx`, `src/components/marketplace/`.

### Phase 6: Final Polish
- **Agent**: `quick_fix_engineer`
- **Scope**: CSS tweaks, brand consistency, Nigerian state ordering, 5% fee display verification.
