# Rulebook Company Documentation

Official documentation for Rulebook Company - machine-readable market microstructure data for institutional trading desks.

Real-time, structured data feeds covering exchange rules, fee schedules, and order types across 40+ equity, options, and futures venues. Built for quantitative hedge funds, market makers, and institutional traders.

This documentation site contains:

- **Getting Started** - Quick integration guide and sample data
- **User Guides** - Integration patterns for trading systems
- **Core Concepts** - Market microstructure data explained
- **API Reference** - Complete API documentation with examples

**[View the live documentation](https://docs.rulebook.company)**

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview your documentation changes locally. To install, use the following command:

```
npm i -g mint
```

Run the following command at the root of your documentation, where your `docs.json` is located:

```
mint dev
```

View your local preview at `http://localhost:3000`.

## Publishing Changes

Changes are automatically deployed to production when pushed to the `main` branch via the Mintlify GitHub App integration.

## Contributing

We welcome contributions to improve our documentation! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## Need Help?

### Troubleshooting

- If your dev environment isn't running: Run `mint update` to ensure you have the most recent version of the CLI.
- If a page loads as a 404: Make sure you are running in a folder with a valid `docs.json`.

### Resources

- [Rulebook Company Website](https://rulebookcompany.com)
- [Support](mailto:support@rulebook.company)
- [Mintlify Documentation](https://mintlify.com/docs) - Platform documentation

## License

MIT License - See [LICENSE](LICENSE) for details.
