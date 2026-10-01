# React Redux App

A counter app built with React, TypeScript and Vite, using Redux for state management **without Redux Toolkit**.

The full activity instructions are in [instructions.md](instructions.md).

## Features

- Redux store created with `createStore` and the `redux-logger` middleware
- Counter actions and action creators (`increment`, `decrement`, `reset`)
- Counter reducer combined with `combineReducers`
- App wrapped in the React-Redux `<Provider>`
- `Counter` component that reads state with `useSelector` and updates it with `useDispatch`

## Getting Started

```bash
npm install
npm run dev
```

Open http://localhost:5173 and use the +, - and Reset buttons. Open the browser console to see each action logged by `redux-logger`.

## Project Structure

```
src/
├── components/
│   ├── Counter.tsx
│   └── Counter.module.css
├── store/
│   ├── actions/
│   │   └── counterActions.ts
│   ├── reducers/
│   │   ├── counterReducer.ts
│   │   └── index.ts
│   └── store.ts
├── App.tsx
├── index.css
└── main.tsx
```

## Scripts

| Command           | Description                      |
| ----------------- | -------------------------------- |
| `npm run dev`     | Start the development server     |
| `npm run build`   | Type-check and build for production |
| `npm run lint`    | Run ESLint                       |
| `npm run preview` | Preview the production build     |
