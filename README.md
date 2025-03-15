# NpmStats Documentation

A comprehensive documentation site for the NpmStats API platform, built with Mintlify.

## 🚀 Getting Started

### Initial Setup

1. Clone the empty repository:
```bash
git clone https://github.com/yokesh-ks/ingeniousclan_npmstats_docs.git
cd ingeniousclan_npmstats_docs
```

2. Initialize the documentation structure:
```bash
# Create basic directory structure
mkdir -p api-reference/endpoints guides

# Create essential files
touch mint.json
touch introduction.mdx
touch api-reference/introduction.mdx
```

3. Configure `mint.json`:
```json
{
  "name": "NpmStats",
  "logo": {
    "light": "/logo/light.png",
    "dark": "/logo/dark.png"
  },
  "favicon": "/favicon.png",
  "colors": {
    "primary": "#0D9373",
    "light": "#07C983",
    "dark": "#0D9373"
  },
  "navigation": [
    {
      "group": "Getting Started",
      "pages": ["introduction"]
    },
    {
      "group": "API Reference",
      "pages": [
        "api-reference/introduction",
        "api-reference/endpoints/package-stats",
        "api-reference/endpoints/bundle-size",
        "api-reference/endpoints/dependencies",
        "api-reference/endpoints/security",
        "api-reference/endpoints/versions",
        "api-reference/endpoints/search",
        "api-reference/endpoints/similar",
        "api-reference/endpoints/health",
        "api-reference/endpoints/webhooks"
      ]
    }
  ]
}
```

## 📚 Documentation Content

Our documentation covers:

- 📊 **API Reference**: Complete API endpoints documentation
- 🚀 **Quick Start Guides**: Get started with NpmStats
- 📦 **SDK Examples**: Code samples for multiple languages
- 🔧 **Integration Guides**: Detailed implementation tutorials
- 🛡️ **Security Best Practices**: Authentication and security guidelines

## 🛠️ Development

### Prerequisites

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview documentation changes locally:

```bash
npm i -g mintlify
```

### Local Development

1. Start the development server:
```bash
mintlify dev
```

2. The documentation will be available at `http://localhost:3000`

### Making Changes

1. **Content Structure**:
   - `/api-reference/*` - API documentation
   - `/guides/*` - User guides and tutorials
   - `/introduction.mdx` - Landing page
   - `mint.json` - Site configuration

2. **Adding New Pages**:
   - Create `.mdx` files in the appropriate directory
   - Update `mint.json` navigation if needed
   - Follow the Mintlify [component guidelines](https://mintlify.com/docs/components)

3. **Testing Changes**:
   - Use `mintlify dev` to preview changes
   - Check responsive layouts
   - Verify all links and navigation

### Publishing Changes

Changes are automatically deployed when pushed to the main branch through our GitHub integration.

#### Deployment Steps:

1. Push changes to the main branch:
```bash
git add .
git commit -m "Add documentation content"
git push origin main
```

2. GitHub Actions will trigger automatic deployment
3. Changes will be live within a few minutes

## 🔍 Troubleshooting

Common issues and solutions:

- **Mintlify dev not running**: 
  ```bash
  mintlify install  # Re-install dependencies
  ```
- **404 Page Errors**: 
  - Ensure you're in the correct directory with `mint.json`
  - Check file paths in navigation
- **Preview Not Updating**: 
  - Clear browser cache
  - Restart development server

## 📝 Contributing

We welcome contributions to improve our documentation:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

Please follow our [contribution guidelines](CONTRIBUTING.md).

## 🔗 Useful Links

- [NpmStats Platform](https://npmstats.ingeniousclan.com)
- [API Status](https://status.npmstats.ingeniousclan.com)
- [Mintlify Documentation](https://mintlify.com/docs)
- [Community Discord](https://discord.gg/npmstats)
- [Documentation Repository](https://github.com/yokesh-ks/ingeniousclan_npmstats_docs)

## 💬 Support

Need help? Contact us through:

- [Documentation Issues](https://github.com/yokesh-ks/ingeniousclan_npmstats_docs/issues)
- [Discord Community](https://discord.gg/npmstats)
- Email: docs@npmstats.ingeniousclan.com

## 📄 License

This documentation is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ by [IngeniousclanTech](https://ingeniousclan.com) 