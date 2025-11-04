# Contributing to Mintlify Starter Kit

Thank you for your interest in contributing to this documentation! This guide will help you make effective contributions.

## How to Contribute

### Reporting Issues

Before creating an issue:
1. Search existing issues to avoid duplicates
2. Check the [troubleshooting guide](README.md#troubleshooting)
3. Verify you're using Node.js 19+

When creating an issue, include:
- Clear description of the problem
- Steps to reproduce
- Expected vs actual behavior
- Environment details (OS, Node version, CLI version)
- Screenshots if applicable

### Suggesting Enhancements

Enhancement suggestions are welcome! Please:
- Explain the use case and benefit
- Provide examples of how it would work
- Consider if it fits the starter kit scope
- Check if similar functionality exists

## Making Changes

### Getting Started

1. **Fork and clone the repository**
   ```bash
   git clone https://github.com/your-username/starter.git
   cd starter
   ```

2. **Install dependencies**
   ```bash
   npm i -g mint
   ```

3. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

4. **Start the development server**
   ```bash
   mint dev
   ```

### Writing Documentation

Follow these guidelines when editing documentation:

#### Content Standards

- **Use second-person voice** ("you" instead of "we")
- **Be concise** - Get to the point quickly
- **Be accurate** - Test all code examples before submitting
- **Be inclusive** - Use gender-neutral language
- **Be helpful** - Anticipate user questions

#### Formatting

- **Frontmatter**: All `.mdx` files must include `title` and `description`
  ```yaml
  ---
  title: "Page Title"
  description: "Brief description for SEO and navigation"
  ---
  ```

- **Headings**: Use proper hierarchy (don't skip levels)
  ```markdown
  ## Main Section
  ### Subsection
  #### Detail
  ```

- **Code blocks**: Always specify the language
  ````markdown
  ```bash
  npm i -g mint
  ```
  ````

- **Links**: Use relative paths for internal links
  ```markdown
  [Good](/quickstart)
  [Bad](https://starter.mintlify.com/quickstart)
  ```

- **Images**: Include descriptive alt text
  ```markdown
  ![Screenshot of the dashboard showing deployment status](/images/dashboard.png)
  ```

#### Components

Use Mintlify components consistently:

```mdx
<Note>
  Helpful contextual information
</Note>

<Warning>
  Important warnings or cautions
</Warning>

<Tip>
  Pro tips and best practices
</Tip>

<Card title="Card Title" icon="icon-name" href="/path">
  Card description
</Card>
```

### Testing Your Changes

Before submitting:

1. **Preview locally**
   ```bash
   mint dev
   ```

2. **Check for broken links**
   ```bash
   mint broken-links
   ```

3. **Verify navigation**
   - Ensure new pages appear in `docs.json`
   - Test all navigation links work
   - Check mobile responsiveness

4. **Test code examples**
   - Run all code snippets to ensure they work
   - Verify commands produce expected output
   - Test on the specified platform/environment

### Committing Changes

1. **Write clear commit messages**
   ```bash
   git commit -m "Fix: Correct npm command in development guide"
   git commit -m "Docs: Add troubleshooting section for port conflicts"
   git commit -m "Feature: Add VS Code setup guide"
   ```

2. **Use conventional commit prefixes**
   - `Fix:` - Bug fixes
   - `Docs:` - Documentation changes
   - `Feature:` - New features or pages
   - `Chore:` - Maintenance tasks
   - `Refactor:` - Code/content restructuring

3. **Keep commits focused**
   - One logical change per commit
   - Avoid mixing unrelated changes

### Submitting Pull Requests

1. **Push your branch**
   ```bash
   git push origin feature/your-feature-name
   ```

2. **Create a pull request** with:
   - Clear title summarizing the change
   - Description of what changed and why
   - Screenshots for visual changes
   - Reference to related issues (if any)

3. **PR checklist**
   - [ ] All new pages have frontmatter
   - [ ] Code examples are tested
   - [ ] Links are relative, not absolute
   - [ ] Images have alt text
   - [ ] Navigation updated if needed
   - [ ] No broken links
   - [ ] Preview looks good locally

## Style Guide

### Voice and Tone

- **Professional but friendly** - Approachable without being casual
- **Clear and direct** - Avoid jargon and complexity
- **Empowering** - Help users succeed independently

### Terminology

Use consistent terminology:
- "docs" or "documentation" (not "docsite")
- "page" (not "document" or "file")
- "code block" (not "code snippet" for multi-line code)
- "CLI" (not "command line" after first mention)

### Common Patterns

**Prerequisites section:**
```markdown
<Info>
  **Prerequisites**:
  - Node.js version 19 or higher
  - Active Mintlify account
</Info>
```

**Step-by-step instructions:**
```markdown
<Steps>
  <Step title="First step">
    Instructions for step one
  </Step>
  <Step title="Second step">
    Instructions for step two
  </Step>
</Steps>
```

## Questions?

- Check the [Mintlify documentation](https://mintlify.com/docs)
- Ask in [community forums](https://mintlify.com/community)
- Review existing pages for examples

## Code of Conduct

- Be respectful and inclusive
- Welcome newcomers
- Provide constructive feedback
- Focus on what's best for users

Thank you for contributing to better documentation!
