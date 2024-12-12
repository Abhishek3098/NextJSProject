This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.

# Storybook Setup Guide

This guide explains how to install and run Storybook for your project. Follow the steps below to get started.

## Prerequisites

Ensure you have the following installed on your system:

- **Node.js** (v14 or higher recommended)
- **npm** (v6 or higher) or **yarn**

## Installation

1. **Add Storybook to your project:**

   Run the following command in the root directory of your project:

   ```bash
   npx storybook init
   ```

   This command installs the necessary dependencies and sets up the Storybook configuration files.

2. **Install additional dependencies (if required):**

   If your project uses specific libraries (e.g., React, Vue, Angular), ensure their respective Storybook addons are installed. For example, for React projects:

   ```bash
   npm install --save-dev @storybook/react
   ```

## Running Storybook

To start the Storybook development server, run the following command:

```bash
npm run storybook
```

or, if you use yarn:

```bash
yarn storybook
```

This will launch Storybook at [http://localhost:6006](http://localhost:6006) in your default web browser.

## Building Storybook for Production

To create a static build of your Storybook for production use, run:

```bash
npm run build-storybook
```

or, if you use yarn:

```bash
yarn build-storybook
```

The static files will be generated in the `storybook-static` directory. You can deploy this directory to any static hosting service.

## File Structure

After installing Storybook, your project structure will include:

```
├── .storybook/           # Storybook configuration files
├── stories/              # Default directory for your stories
└── package.json          # Updated with Storybook scripts and dependencies
```

## Custom Configuration

You can customize Storybook by editing the configuration files in the `.storybook` directory:

- **`main.js`**: Configure addons, webpack, and other settings.
- **`preview.js`**: Add global decorators and parameters.
- **`manager.js`**: Customize the Storybook UI.

Refer to the [Storybook documentation](https://storybook.js.org/docs) for detailed configuration options.

## Troubleshooting

If you encounter issues:

- Ensure all dependencies are installed correctly by running:

  ```bash
  npm install
  ```

- Check for conflicting dependencies in `package.json`.
- Visit the [Storybook GitHub Issues](https://github.com/storybookjs/storybook/issues) page for support.

## Resources

- [Storybook Documentation](https://storybook.js.org/docs)
- [Storybook Addons](https://storybook.js.org/addons)
- [Storybook GitHub](https://github.com/storybookjs/storybook)
