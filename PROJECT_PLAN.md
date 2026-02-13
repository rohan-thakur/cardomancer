# Cardomancer - Project Plan

## Core User Flow

1. **Upload Photos** - Users upload images of themselves/friends/pets/relatives
2. **Select Theme** - Choose from predefined themes (superhero, anime, pokemon, etc.)
3. **Customize** - Add optional custom prompts for stats, bios, abilities
4. **Preview** - AI generates card design previews
5. **Order** - Place order for physical card packs
6. **Fulfillment** - Cards printed and shipped via QP Market Network

## Themes (Initial Set)

- 🦸 Superhero
- 🎌 Anime
- 🔴 Pokemon
- 🏀 Retro Sports Cards
- ⚔️ Fantasy RPG
- 💼 Corporate Parody
- 🎮 Video Game Character
- 🎭 Movie Poster Style

## Technical Architecture (Draft)

### Frontend
- User interface for photo upload
- Theme selection gallery
- Custom stat/bio editor
- Card preview viewer
- Order/checkout flow

### Backend
- Image storage and processing
- AI integration for card generation
- User management and authentication
- Order management
- Payment processing
- QP Market Network API integration for fulfillment

### AI Components
- Image preprocessing (background removal, face detection, etc.)
- Style transfer / theme application
- Text generation for stats/bios (if user wants AI suggestions)
- Card layout composition

### Fulfillment Integration
- QP Market Network API: https://www.qpmarketnetwork.com/
- Product catalog integration
- Order submission
- Status tracking
- Shipping updates

## Data Models (Preliminary)

### User
- id, email, name, created_at

### CardDesign
- id, user_id, photo_url, theme, custom_stats (JSONB), preview_url, created_at

### Order
- id, user_id, card_designs[], quantity, status, fulfillment_id, created_at

## Monetization
- TBD: Pricing per card pack
- Potential tiers: Standard cards, premium finishes, foil cards, etc.

## Next Steps
1. Choose tech stack (frontend/backend frameworks)
2. Set up development environment
3. Design database schema
4. Create wireframes/mockups
5. Investigate QP Market Network API documentation
6. Research AI models for card generation
7. Build MVP prototype
