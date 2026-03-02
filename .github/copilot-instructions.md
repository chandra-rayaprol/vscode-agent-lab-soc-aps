# Copilot Instructions - Soc Ops Bingo Game

## Development Checklist
Before any changes, ensure:
- [ ] `npm run lint` - Code passes ESLint checks
- [ ] `npm run build` - TypeScript compiles successfully
- [ ] `npm test` - All tests pass

## Project Architecture
**Social Bingo game** for in-person mixers: React 19 + TypeScript + Vite + TailwindCSS v4

### Game Flow & State
- **Start Screen** → **Playing** (5x5 grid) → **Bingo** (modal + celebration)
- State managed by `useBingoGame` hook with localStorage persistence
- Center square = FREE SPACE (auto-marked), Win = any row/column/diagonal

### Key Patterns
**State Management**: `useBingoGame` hook centralizes logic with immutable updates via `utils/bingoLogic.ts`

**Components**: Stateless UI receiving props, pattern: `interface ComponentProps` + destructured props
- `App.tsx`: Root with conditional rendering by game state
- `components/`: UI only, `hooks/`: logic, `utils/`: pure functions, `data/`: static content

## Development Conventions

### Testing & Styling
- **Vitest + RTL**: Pure functions fully tested, components via integration
- **TailwindCSS v4**: `@theme` syntax in `index.css`, custom colors (`--color-accent`, `--color-marked`, `--color-bingo`)
- **Layout**: `grid-cols-5 gap-1` for board, mobile-first with `max-w-md mx-auto`, `min-h-[60px]` touch targets

### TypeScript
- Strict typing with domain types in `src/types/index.ts`
- Interface segregation per component
- Re-export pattern: `export type { BingoSquareData } from '../types'`

## Commands & Deployment
- `npm run dev`: Dev server (http://localhost:5173)
- `npm run build`: Production build
- `npm test`: Test runner
- **Auto-deploy**: GitHub Pages on `main` push

## File Modification Patterns
- **Questions**: Update `src/data/questions.ts` (24+ items)
- **Styles**: TailwindCSS classes or `@theme` in `index.css`
- **Logic**: Pure functions in `utils/bingoLogic.ts` + tests
- **UI**: Stateless components from `useBingoGame` props

## Critical Details
- **Board**: Shuffled questions, FREE_SPACE at index 12, 12 win lines (5+5+2)
- **Persistence**: `bingo-game-state` v1 with validation/migration
- **Immutability**: `board.map(sq => sq.id === squareId ? {...sq, isMarked: !sq.isMarked} : sq)`