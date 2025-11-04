# Mintlify Starter Kit

A comprehensive documentation starter template built with [Mintlify](https://mintlify.com). This starter kit provides a production-ready foundation for creating beautiful, interactive documentation sites.

## What's Included

This starter kit contains:

- **Guide pages** - Step-by-step tutorials and how-to guides
- **Navigation** - Pre-configured tab and sidebar navigation
- **Customizations** - Theme colors, logos, and branding
- **API reference pages** - OpenAPI/Swagger integration examples
- **Popular components** - Cards, accordions, code blocks, and more
- **AI tools guides** - Documentation for Claude Code, Cursor, and Windsurf

**[Follow the full quickstart guide](https://starter.mintlify.com/quickstart)**

## Quick Start

### Prerequisites

- Node.js version 19 or higher
- Git for version control

### Local Development

1. **Clone this repository**
   ```bash
   git clone <your-repo-url>
   cd <your-repo-name>
   ```

2. **Install the Mintlify CLI**
   ```bash
   npm i -g mint
   ```

3. **Start the development server**
   ```bash
   mint dev
   ```

4. **View your docs**

   Open [http://localhost:3000](http://localhost:3000) in your browser. Changes auto-reload as you edit files.

## Project Structure

```
.
├── docs.json           # Main configuration file
├── index.mdx          # Homepage
├── quickstart.mdx     # Quick start guide
├── essentials/        # Core documentation guides
├── api-reference/     # API documentation examples
├── ai-tools/          # AI tools integration guides
├── images/            # Image assets
└── logo/              # Logo files (light/dark mode)
```

## Customization

### Update Site Metadata

Edit `docs.json` to customize:
- Site name and colors
- Navigation structure
- Logo and favicon
- Footer social links

### Add New Pages

1. Create a new `.mdx` file in the appropriate directory
2. Add frontmatter with `title` and `description`
3. Update `docs.json` to include the page in navigation

## Publishing Changes

### Automatic Deployment

1. Install the [Mintlify GitHub app](https://dashboard.mintlify.com/settings/organization/github-app) from your dashboard
2. Push changes to your default branch
3. Changes deploy automatically to production

### Manual Deployment

See the [Mintlify deployment documentation](https://mintlify.com/docs/settings/deployment) for alternative deployment options.

## Troubleshooting

### Common Issues

**Development server won't start**
- Ensure Node.js version 19+ is installed: `node --version`
- Update the CLI: `npm update -g mint`
- Clear Mintlify cache: Remove `~/.mintlify` folder

**404 errors on pages**
- Verify you're in a directory with `docs.json`
- Check that page paths in `docs.json` match file names
- Ensure frontmatter is present on all `.mdx` files

**Port already in use**
- Specify a different port: `mint dev --port 3333`
- Kill the process using port 3000

**Sharp module errors on Mac**
- Remove CLI: `npm remove -g mint`
- Update to Node.js v19+
- Reinstall CLI: `npm i -g mint`

**Broken links**
- Run link validation: `mint broken-links`
- Use relative paths for internal links
- Ensure all referenced pages exist

### Get Help

- [Mintlify documentation](https://mintlify.com/docs)
- [Community support](https://mintlify.com/community)
- [GitHub issues](https://github.com/mintlify/starter/issues)

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on contributing to this documentation.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
