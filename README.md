# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.

## Deployment (GitHub Pages)

This project is set up to deploy to GitHub Pages using a GitHub Actions workflow.

- The workflow file is `.github/workflows/deploy.yml` and runs on `push` to the `main` branch.
- It builds the Vite app (`npm run build`) and publishes the `./dist` folder to GitHub Pages.

To enable Pages for this repository:

1. In your GitHub repository go to `Settings` → `Pages`.
2. Under "Build and deployment" select "GitHub Actions" (it may already be selected).
3. Under "Build and deployment" ensure the branch is set to `gh-pages` or the Pages service is configured to use the action (the Actions workflow will publish to Pages automatically).

After pushing to `main`, the Action will run and publish the site. You can monitor workflow runs under the repository's `Actions` tab.
