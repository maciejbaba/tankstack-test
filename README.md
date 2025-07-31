# TanStack Test

A simple counter application built with [TanStack Start](https://tanstack.com/start) (React full-stack framework) that demonstrates server-side state persistence.

## Features

- **Server-side Counter**: Counter state is persisted on the server using a file-based storage
- **Real-time Updates**: Uses TanStack Start's server functions for seamless client-server communication
- **Type-safe**: Built with TypeScript for enhanced developer experience
- **Modern React**: Utilizes React 19 with the latest patterns

## Tech Stack

- **Framework**: [TanStack Start](https://tanstack.com/start) v1.116.1
- **Router**: [TanStack Router](https://tanstack.com/router) v1.116.0
- **Frontend**: React 19 + TypeScript
- **Build Tool**: [Vinxi](https://vinxi.vercel.app/) v0.5.4
- **Development**: Vite with TypeScript support

## Getting Started

### Prerequisites

- Node.js (version 18 or higher recommended)
- npm or yarn package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/maciejbaba/tankstack-test.git
cd tankstack-test
```

2. Install dependencies:
```bash
npm install
```

### Development

Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:3000` (or the next available port).

### Building for Production

Build the application:
```bash
npm run build
```

Start the production server:
```bash
npm run start
```

## How It Works

The application demonstrates a simple yet powerful pattern:

1. **Server Function**: `getCount()` reads the current counter value from `count.txt`
2. **Client Interaction**: Users can click a button to increment the counter
3. **Server Update**: `updateCount()` server function updates the file and persists the new value
4. **State Synchronization**: The router invalidates and refetches the latest count

### File Structure

```
├── app/
│   ├── routes/
│   │   ├── __root.tsx      # Root layout component
│   │   └── index.tsx       # Home page with counter logic
│   ├── client.tsx          # Client-side entry point
│   ├── router.tsx          # Router configuration
│   └── ssr.tsx            # Server-side rendering setup
├── app.config.ts          # TanStack Start configuration
├── package.json
├── tsconfig.json
└── count.txt             # Server-side counter storage
```

## Key Concepts Demonstrated

- **Server Functions**: Type-safe functions that run on the server
- **File-based Routing**: Automatic route generation from file structure
- **SSR**: Server-side rendering with hydration
- **State Management**: Server-side state persistence
- **Type Safety**: End-to-end TypeScript support

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the ISC License.

## Learn More

- [TanStack Start Documentation](https://tanstack.com/start/latest)
- [TanStack Router Documentation](https://tanstack.com/router/latest)
- [React Documentation](https://react.dev/)