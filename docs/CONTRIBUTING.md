# Contributing to Vulnemon

Thank you for your interest in contributing to Vulnemon! 🦊

## How to Contribute

### 1. Creating Labs (Easiest way to contribute!)

Each lab is a self-contained challenge with:
- A Docker container running the vulnerable application
- A `lab.yml` config file with metadata
- A `solution.md` file (kept private, for maintainers only)

See [LAB_CREATION.md](LAB_CREATION.md) for the full guide.

### 2. Frontend Development

We use Next.js 14+, React, TypeScript, and Tailwind CSS.

```bash
cd vulnemon
npm install
npm run dev
```

### 3. Bug Reports

Open an issue with:
- Steps to reproduce
- Expected vs actual behavior
- Screenshots if applicable

### 4. Feature Requests

Open an issue with the `feature-request` label describing:
- The problem you're solving
- Your proposed solution
- Any alternatives considered

## Pull Request Process

1. Fork the repo
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Make your changes
4. Test locally
5. Commit with clear messages: `git commit -m 'Add: Description of change'`
6. Push and open a PR

## Code Style

- Use TypeScript for all new code
- Follow existing code patterns
- Write meaningful commit messages
- Comment complex logic

## Questions?

Email: prem@reddoralabs.com
