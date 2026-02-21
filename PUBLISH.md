# Publishing Electrobun Skills to GitHub

This guide explains how to publish the electrobun-skills repository to GitHub.

## Step 1: Create GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Repository name: `electrobun-skills`
3. Description: "Specialized skills for building desktop applications with Electrobun"
4. Set to **Public** (required for skills.sh)
5. Do NOT initialize with README, .gitignore, or LICENSE (we already have them)
6. Click "Create repository"

## Step 2: Push to GitHub

```bash
cd /Users/rajachintada/Projects/electrobun-skills

# Add remote (replace with your GitHub username/org)
git remote add origin https://github.com/blackboardsh/electrobun-skills.git

# Or if using SSH:
# git remote add origin git@github.com:blackboardsh/electrobun-skills.git

# Push to GitHub
git push -u origin main
```

## Step 3: Create First Release

```bash
# Tag the initial release
git tag -a v1.0.0 -m "Initial release: 6 comprehensive Electrobun skills"

# Push tags
git push origin v1.0.0
```

Or create release via GitHub UI:
1. Go to repository → Releases → "Draft a new release"
2. Tag: `v1.0.0`
3. Title: "v1.0.0 - Initial Release"
4. Description:
   ```
   First release of Electrobun Skills!

   ## Skills Included

   - **electrobun** - Core framework guide
   - **electrobun-window-management** - Multi-window patterns
   - **electrobun-rpc-patterns** - Type-safe RPC communication
   - **electrobun-native-ui** - Native menus, tray, dialogs
   - **electrobun-distribution** - Packaging and auto-updates
   - **electrobun-debugging** - Development workflow

   All skills follow Anthropic skill-creator best practices.

   ## Installation

   ```bash
   npx skills add blackboardsh/electrobun-skills/electrobun
   ```

   See README for full documentation.
   ```
5. Click "Publish release"

## Step 4: Test Installation

```bash
# Test installing a skill
npx skills add blackboardsh/electrobun-skills/electrobun

# Verify it works with GitHub Copilot CLI
# Ask Copilot about Electrobun and see if skill triggers
```

## Step 5: Submit to skills.sh

1. Go to [skills.sh](https://skills.sh/)
2. Look for "Submit a skill" or similar option
3. Submit repository URL: `https://github.com/blackboardsh/electrobun-skills`
4. Skills.sh will validate and index the repository

Note: Skills.sh automatically discovers skills in `skills/` directories and reads metadata from package.json.

## Repository Structure

```
electrobun-skills/
├── README.md              # Main documentation
├── CONTRIBUTING.md        # Contribution guidelines
├── LICENSE               # MIT License
├── package.json          # Package metadata with skills listing
├── .gitignore           # Git ignore rules
└── skills/              # All skills
    ├── electrobun/
    │   └── SKILL.md
    ├── electrobun-window-management/
    │   └── SKILL.md
    ├── electrobun-rpc-patterns/
    │   └── SKILL.md
    ├── electrobun-native-ui/
    │   └── SKILL.md
    ├── electrobun-distribution/
    │   └── SKILL.md
    └── electrobun-debugging/
        └── SKILL.md
```

## Maintenance

### Adding New Skills

1. Create new directory in `skills/`
2. Add SKILL.md following guidelines in CONTRIBUTING.md
3. Update package.json `skills` section
4. Commit and push
5. Create new release

### Updating Existing Skills

1. Edit SKILL.md files
2. Commit changes
3. Create new release with version bump
4. Users can update with `npx skills add --force`

## Verification Checklist

- [ ] Repository is public on GitHub
- [ ] README.md is comprehensive and clear
- [ ] All SKILL.md files have proper frontmatter
- [ ] package.json lists all skills
- [ ] LICENSE file exists (MIT)
- [ ] First release (v1.0.0) is tagged
- [ ] Skills can be installed via npx
- [ ] Repository submitted to skills.sh

## Support

- **Issues**: Use GitHub Issues for bug reports and feature requests
- **Discussions**: Use GitHub Discussions for questions and ideas
- **Discord**: Join [Electrobun Discord](https://discord.gg/ueKE4tjaCE)
