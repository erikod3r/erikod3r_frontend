# theer1k

It is built with Next.js, Tailwind CSS, Flowbite, and TypeScript to provide a seamless developer experience.

### Features

Engineer experience first:

- ⚡ [Next.js](https://nextjs.org) for Static Site Generator

- 🔥 Type checking [TypeScript](https://www.typescriptlang.org)

- 💎 Integrate with [Tailwind CSS](https://tailwindcss.com)

- ✅ Strict Mode for TypeScript and React 18

- 📏 Linter with [ESLint](https://eslint.org) (default NextJS, NextJS Core Web Vitals, Tailwind CSS and Airbnb configuration)

- 💖 Code Formatter with [Prettier](https://prettier.io)

- 🦊 Husky for Git Hooks

- 🚫 Lint-staged for running linters on Git staged files

- 🚓 Lint git commit with Commitlint

- 📓 Write standard compliant commit messages with Commitizen

- 🦺 Unit Testing with Jest and React Testing Library

- 🧪 E2E Testing with Cypress

- 👷 Run tests on pull request with GitHub Actions

- 🎉 Storybook for UI development

- 🎁 Automatic changelog generation with Semantic Release

- 🔍 Visual testing with Percy (Optional)

- 💡 Absolute Imports using `@` prefix

- 🗂 VSCode configuration: Debug, Settings, Tasks and extension for PostCSS, ESLint, Prettier, TypeScript, Jest

- 🤖 SEO metadata, JSON-LD and Open Graph tags with Next SEO

- 🗺️ Sitemap.xml and robots.txt with next-sitemap

- ⚙️ [Bundler Analyzer](https://www.npmjs.com/package/@next/bundle-analyzer)

- 🖱️ One click deployment with Vercel or Netlify (or manual deployment to any hosting services)

- 🌈 Include a FREE minimalist theme

- 💯 Maximize lighthouse score

Built-in feature from Next.js:

- ☕ Minify HTML & CSS

- 💨 Live reload

- ✅ Cache busting

### Philosophy

- All the Next.js pages are statically generated by default. You can easily switch to SSR adding `getServerSideProps` to your page.

- Minimal code

- SEO-friendly

- 🚀 Production-ready

### Requirements

- Node.js 18+ and [pnpm](https://pnpm.io/pt/)

### Getting started

Run the following command on your local environment:

```shell

git clone --depth=1  https://github.com/theer1k/portfolio.git

cd portfolio

pnpm install
```
Then, you can run locally in development mode with live reload:

```shell
pnpm run dev
```

Open http://localhost:3000 with your favorite browser to see your project.

```shell
┌── __mocks__                       # Mocks for testing
├── .github                         # GitHub folder
├── .husky                          # Husky configuration
├── .storybook                      # Storybook configuration
├── .vscode                         # VSCode configuration
├── cypress                         # Cypress e2e tests files
├── public                          # Public assets folder
├── src                             # Source code
│   ├── components                  # Components (reusable)
│   │   ├── hoc                     # High Order Components
│   │   ├── ui                      # UI (Atomic Design)
│   │   │   ├── atoms               # Atoms
│   │   │   ├── molecules           # Molecules
│   │   │   └── organisms           # Organisms
│   ├── configs                     # Config files
│   ├── hooks                       # Hooks (reusable)
│   ├── layouts                     # Layouts components
│   ├── pages                       # Next JS Pages
│   ├── pages.test                  # Next JS Pages tests (this avoids tests to be treated as a Next.js pages)
│   ├── styles                      # Styles folder
│   ├── templates                   # Default template
│   └── utils                       # Utility functions
├── cypress.config.js               # Cypress configuration
├── jest.config.js                  # Jest configuration
├── next.config.js                  # NextJS configuration
├── postcss.config.js               # PostCSS configuration
├── README.md                       # README file
├── tailwind.config.js              # Tailwind CSS configuration
└── tsconfig.json                   # TypeScript configuration
```

### Customization

Here is some of the most important files to customize:

- `public/apple-touch-icon.png`, `public/favicon.ico`, `public/favicon-16x16.png` and `public/favicon-32x32.png`: website favicon, generate from https://favicon.io/favicon-converter/

- `src/styles/global.css`: CSS file using Tailwind CSS

- `src/configs/AppConfig.ts`: configuration file

- `src/templates/Main.tsx`: default theme

- `next-sitemap.config.js`: sitemap configuration

You have access to the whole code source if you need further customization. The provided code is only example for you to start your project. The sky is the limit 🚀.

### Commit Message Format

The project enforces [Conventional Commits](https://www.conventionalcommits.org/) specification. This means that all your commit messages must be formatted according to the specification. To help you write commit messages, the project uses [Commitizen](https://github.com/commitizen/cz-cli), an interactive CLI that guides you through the commit process. To use it, run the following command:

```shell
pnpm run commit
```

One of the benefits of using Conventional Commits is that it allows us to automatically generate a `CHANGELOG` file. It also allows us to automatically determine the next version number based on the types of commits that are included in a release.

### Deploy to production

You can see the results locally in production mode with:

```shell

$  pnpm run build

$  pnpm run start

```

The generated HTML and CSS files are minified (built-in feature from Next js). It will also remove unused CSS from [Tailwind CSS](https://tailwindcss.com).

You can create an optimized production build with:

```shell
pnpm run build-prod
```

Now, your blog is ready to be deployed. All generated files are located at `out` folder, which you can deploy with any hosting service.

### Testing

All tests are colocated with the source code inside the same directory. So, it makes it easier to find them. Unfortunately, it is not possible with the `pages` folder which is used by Next.js for routing. So, what is why we have a `pages.test` folder to write tests from files located in `pages` folder.

### Deploy to Vercel

Deploy this Next JS Boilerplate on Vercel in one click:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/git/external?repository-url=https%3A%2F%2Fgithub.com%2Fixartz%2FNext-js-Boilerplate)

### VSCode information (optional)

If you are VSCode users, you can have a better integration with VSCode by installing the suggested extension in `.vscode/extension.json`. The starter code comes up with Settings for a seamless integration with VSCode. The Debug configuration is also provided for frontend and backend debugging experience.

With the plugins installed on your VSCode, ESLint and Prettier can automatically fix the code and show you the errors. Same goes for testing, you can install VSCode Jest extension to automatically run your tests and it also show the code coverage in context.

Pro tips: if you need a project wide type checking with TypeScript, you can run a build with <kbd>Cmd</kbd> + <kbd>Shift</kbd> + <kbd>B</kbd> on Mac.

### Contributions

Everyone is welcome to contribute to this project. Feel free to open an issue if you have question or found a bug. Totally open to any suggestions and improvements.

### License

Licensed under the MIT License, Copyright © 2023

See [LICENSE](LICENSE) for more information.

---

Made with ♥ by [theer1k](https://indianboy.com.br/)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/erikhenriquealvescunha/)
[![LinkedIn](https://img.shields.io/badge/dev.to-0A0A0A?style=for-the-badge&logo=dev.to&logoColor=white)](https://dev.to/theer1k)