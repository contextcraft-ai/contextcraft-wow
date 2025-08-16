# ContextCraft WOW Repository

Multi-methodology project management templates for AI-assisted development.

## 🎯 Overview

This repository provides a multi-branch Git system serving as the single source of truth for project management methodologies. Each branch contains a complete methodology implementation that can be integrated into any project via git submodules.

## 🌿 Available Methodologies

- **main** - Default epic/feat/story structure (balanced approach)
- **ryan-singer** - Shape Up methodology (6-week cycles, appetite-driven)
- **minimal** - Stories-only lightweight approach (coming soon)
- **agile** - Sprint-based agile with velocity tracking (coming soon)

## 🚀 Quick Start

### Add to Your Project

```bash
# Add as submodule to your project
git submodule add -b main https://github.com/contextcraft-ai/contextcraft-wow.git docs/.wow

# Switch to a different methodology
cd docs/.wow
git checkout ryan-singer
```

### Project Structure

```
your-project/
├── docs/
│   └── .wow/                    # This submodule
│       ├── WOW.md              # Methodology documentation
│       ├── CLAUDE.md           # AI persona context
│       ├── templates/          # Story/epic templates
│       ├── safeguards/         # Validation rules
│       └── examples/           # Sample projects
```

## 📁 Repository Structure

Each methodology branch contains:

- `WOW.md` - Core methodology documentation
- `CLAUDE.md` - AI persona contexts and prompts
- `templates/` - Story, epic, and task templates
- `safeguards/` - Validation rules and git hooks
- `examples/` - Sample project structures
- `personas/` - AI coaching personalities

## 🔄 Switching Methodologies

```bash
# List available methodologies
git branch -r

# Switch methodology
git checkout ryan-singer

# Update your project
cd ../..
git add docs/.wow
git commit -m "Switch to Shape Up methodology"
```

## 📝 Template Usage

Templates use Mustache/Handlebars syntax for variables:

```markdown
# Epic: {{epicName}}
**Created**: {{createdDate}}
**Methodology**: {{methodology}}
```

## 🛡️ Safeguards

Each methodology includes:
- Git hooks for format validation
- todotxt.org compliance checking
- Methodology-specific rules
- CI/CD integration templates

## 🤝 Contributing

1. Fork this repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

For new methodology branches, please follow the branch structure guidelines in `docs/contributing.md`.

## 📖 Documentation

- [Integration Guide](docs/integration.md)
- [Migration Guide](docs/migration.md)
- [Methodology Comparison](docs/comparison.md)

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details.

## 🔗 Links

- [ContextCraft Organization](https://github.com/contextcraft-ai)
- [Documentation](https://github.com/contextcraft-ai/contextcraft-wow/wiki)
- [Issues](https://github.com/contextcraft-ai/contextcraft-wow/issues)
- [Discussions](https://github.com/contextcraft-ai/contextcraft-wow/discussions)

---

*Part of the ContextCraft ecosystem for AI-assisted development.*