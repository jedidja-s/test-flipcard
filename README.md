# FlipCard Game Demo

This is a [Next.js](https://nextjs.org) project demonstrating the [@jedidja-s/flipcard-game](https://github.com/your-username/flipcard-game) component.

## Getting Started

First, install the dependencies:

```bash
npm install
```

Then, run the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the FlipCard game in action.

## Required Styles

The FlipCard component requires specific CSS classes for the 3D flip animation. These are already included in `app/globals.css`:

```css
.perspective-1000 {
  perspective: 1000px;
}

.preserve-3d {
  transform-style: preserve-3d;
  -webkit-transform-style: preserve-3d;
}

.backface-hidden {
  backface-visibility: hidden;
  -webkit-backface-visibility: hidden;
}

.rotate-y-180 {
  transform: rotateY(180deg);
  -webkit-transform: rotateY(180deg);
}
```

## Features

- Interactive flashcard game with flip animations
- Composer mode for creating and editing cards
- Player mode for learning
- Local storage support
- Progress tracking
- Responsive design

## Component Usage

```tsx
import { FlipCardGame } from "@jedidja-s/flipcard-game";

export default function TestPage() {
  return (
    <FlipCardGame
      adminMode={false}
      storageType="local"
      initialTitle="Programming Flashcards"
      initialCards={[
        {
          id: "1",
          front: "What is a closure?",
          back: "A function that has access to variables in its outer scope",
          learned: false,
        },
      ]}
    />
  );
}
```

## Learn More

To learn more about the technologies used:

- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS](https://tailwindcss.com/docs)
- [@jedidja-s/flipcard-game Documentation](https://github.com/your-username/flipcard-game)

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new).

Check out the [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
# test-flipcard
