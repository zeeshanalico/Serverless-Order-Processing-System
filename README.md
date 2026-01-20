# Serverless Order Processing System

A clean, minimal React frontend for processing orders with form validation and API integration.

## Features

- ✅ React functional components with hooks
- ✅ Vite for fast development and building
- ✅ Tailwind CSS for modern, professional styling
- ✅ Form validation for all required fields
- ✅ Loading states during API calls
- ✅ Success and error message handling
- ✅ Disabled submit button while loading
- ✅ AWS Amplify compatible

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- pnpm (install with `npm install -g pnpm`)

### Installation

1. Install dependencies:
```bash
pnpm install
```

2. Start the development server:
```bash
pnpm dev
```

3. Open your browser and navigate to `http://localhost:5173`

### Building for Production

```bash
pnpm build
```

The built files will be in the `dist` directory.

### Preview Production Build

```bash
pnpm preview
```

## Project Structure

```
.
├── src/
│   ├── App.jsx          # Main order form component
│   ├── main.jsx         # React entry point
│   └── index.css        # Tailwind CSS imports
├── index.html           # HTML template
├── vite.config.js       # Vite configuration
├── tailwind.config.js   # Tailwind CSS configuration
├── postcss.config.js    # PostCSS configuration
└── package.json         # Dependencies and scripts
```

## API Integration

The form submits to `/api/orders` endpoint. Update the API endpoint in `src/App.jsx` if needed.

Expected request format:
```json
{
  "customerName": "John Doe",
  "email": "john@example.com",
  "productName": "Product Name",
  "quantity": 5
}
```

## AWS Amplify Deployment

This project is configured to work with AWS Amplify. The build settings are compatible with Amplify's default React build configuration.

## Technologies Used

- React 18
- Vite 5
- Tailwind CSS 3
- pnpm

