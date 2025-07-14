# SuperMarketer – Marketing Framework for Claude

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-2.0.1-blue.svg)](https://github.com/NomenAK/SuperClaude)
[![GitHub issues](https://img.shields.io/github/issues/NomenAK/SuperClaude)](https://github.com/NomenAK/SuperClaude/issues)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/NomenAK/SuperClaude/blob/master/CONTRIBUTING.md)

**A configuration framework that enhances Claude with specialized marketing commands, personas, and workflows.**

## 🚀 Version 2.0.1 Update

IMPORTANT: Start Fresh by removing old files and dir in .claude (RULES.md MCP.md PERSONAS.md CLAUDE.md and /commands dir)

SuperClaude v2 introduces architectural improvements focused on maintainability and extensibility:

- **⚡ Streamlined Architecture**: @include reference system for configuration management
- **🎭 Personas as Flags**: 9 cognitive personas integrated into the flag system (`--persona-architect`, `--persona-security`, etc.)
- **📦 Enhanced Installer**: install.sh with update mode, dry-run, backup handling, and platform detection
- **🔧 Modular Design**: Template system for adding new commands and features
- **🎯 Unified Experience**: Consistent flag behavior across all commands

See [ROADMAP.md](ROADMAP.md) for future marketing ideas and contribution opportunities.

## 🎯 Background

Claude provides powerful capabilities but can benefit from:
- **Specialized expertise** for different marketing domains
- **Token efficiency** for large campaigns
- **Data-driven approaches** to marketing
- **Context preservation** during campaign iterations
- **Channel-specific thinking** for various tasks

## ✨ SuperClaude Features

SuperMarketer enhances Claude with:
- **Marketing Commands** for campaigns, SEO, branding, and analytics
- **9 Marketing Personas** for domain-specific expertise
- **Token Optimization** with compression options
- **Evidence-Based Approach** for data-driven decisions
- **MCP Integration** with Context7, Sequential, Magic, Puppeteer
- **Campaign Checkpoint Support** for safe experimentation
- **Introspection Mode** for framework improvement and troubleshooting

## 🚀 Installation

### Enhanced Installer v2.0.1
The installer provides various options:

```bash
git clone https://github.com/NomenAK/SuperClaude.git
cd SuperClaude

# Basic installation
./install.sh                           # Default: ~/.claude/

# Advanced options
./install.sh --dir /opt/claude        # Custom location
./install.sh --update                 # Update existing installation
./install.sh --dry-run --verbose      # Preview changes with details
./install.sh --force                  # Skip confirmations (automation)
./install.sh --log install.log        # Log all operations
```

**v2.0.1 Installer Features:**
- 🔄 **Update Mode**: Preserves customizations while updating
- 👁️ **Dry Run**: Preview changes before applying
- 💾 **Smart Backups**: Automatic backup with timestamping
- 🧹 **Clean Updates**: Removes obsolete files
- 🖥️ **Platform Detection**: Works with Linux, macOS, WSL
- 📊 **Progress Tracking**: Installation feedback

Zero dependencies. Installs to `~/.claude/` by default.

**Note:** After installation, all configuration files are located in `~/.claude/` (your home directory), not in the project directory.

## 💡 Core Capabilities

### 🧠 **Cognitive Personas (Now as Flags!)**
Switch between different approaches with persona flags:

```bash
/campaign --launch --persona-brand           # Strategic campaign planning
/seo --audit --persona-seo                   # Search optimization review
/ads --optimize --persona-ad                 # Advertising improvements
/partnership --outreach --persona-partnership # Collaboration opportunities
```

**v2.0.1 Update**: All 9 personas are now universal flags, available on every command for consistent access to specialized approaches.

### ⚡ **Marketing Commands**
Campaign and brand management:

**Campaign Management**
```bash
/campaign --launch --channels email,social   # Run digital campaign
/ads --create --budget 1000                  # Launch advertising
/seo --audit --report                        # SEO analysis
```

**Brand & Content**
```bash
/brand --design --guide                      # Brand asset creation
/content --plan --calendar                   # Content calendar
/social --schedule --persona-social          # Social engagement
```

**Analytics & Outreach**
```bash
/analytics --report --persona-analytics      # Performance tracking
/partnership --outreach --crm                # Partnership outreach
/optimize --iterate --persona-brand          # Campaign improvements
```

### 🎛️ **MCP Integration**
- **Context7**: Access to library documentation
- **Sequential**: Multi-step reasoning capabilities
- **Magic**: AI-generated UI components
- **Puppeteer**: Browser testing and automation

**⚠️ Important:** SuperClaude does not include MCP servers. You need to install them separately in Claude Code's MCP settings to use MCP-related flags (--c7, --seq, --magic, --pup).

### 📊 **Token Efficiency**
SuperClaude's @include template system helps manage token usage:
- **UltraCompressed mode** option for token reduction
- **Template references** for configuration management
- **Caching mechanisms** to avoid redundancy
- **Context-aware compression** options

## 🎮 Example Workflows

### Digital Campaign Launch
```bash
/campaign --launch --persona-brand                 # Plan campaign strategy
/ads --create --budget 5000                        # Set up advertising
/seo --audit --persona-seo                         # Optimize search presence
/content --plan --calendar                         # Content schedule
```

### SEO Performance Improvement
```bash
/seo --audit --persona-seo                         # Audit ranking factors
/optimize --iterate --persona-analytics            # Improve results
/analytics --report --persona-analytics            # Track metrics
```

### Marketing Framework Enhancement
```bash
/troubleshoot --introspect                         # Debug SuperMarketer behavior
/analyze --introspect --seq                        # Analyze framework patterns
/improve --introspect --uc                         # Optimize token usage
```

### Cross-Channel Execution
```bash
/campaign --launch --channels all --persona-brand  # Deploy across channels
/social --schedule --persona-social                # Social media actions
/analytics --report --persona-analytics            # Monitor performance
```

## 🎭 Available Personas

| Persona | Focus Area | Tools | Use Cases |
|---------|-----------|-------|-----------|
| **brand** | Brand strategy | Context7, Magic | Campaign positioning |
| **seo** | Search optimization | Sequential, Context7 | SEO audits |
| **ad** | Paid advertising | Magic, Puppeteer | Ad management |
| **partnership** | Partnerships | Sequential | Outreach planning |
| **content** | Content creation | Magic, Context7 | Blog and copywriting |
| **design** | Graphic design | Magic | Visual assets |
| **social** | Social media | Puppeteer, Context7 | Social engagement |
| **offline** | Offline marketing | Sequential | Event planning |
| **analytics** | Marketing analytics | Context7, Sequential | Performance reporting |

## 🛠️ Configuration Options

### Thinking Depth Control
```bash
# Standard analysis
/analyze --think

# Deeper analysis  
/design --think-hard

# Maximum depth
/troubleshoot --ultrathink
```

### Introspection Mode
```bash
# Enable self-aware analysis for SuperClaude improvement
/analyze --introspect

# Debug SuperClaude behavior
/troubleshoot --introspect --seq

# Optimize framework performance
/improve --introspect --persona-performance
```

### Token Management
```bash
# Standard mode
/campaign --launch --channels email

# With compression
/analyze --architecture --uc

# Native tools only
/scan --security --no-mcp
```

### Evidence-Based Marketing
SuperMarketer encourages:
- Documentation for campaign decisions
- Testing for content effectiveness
- Metrics for performance work
- Compliance validation for campaigns
- Analysis for strategic choices

## 📋 Command Categories

### Campaigns (3 Commands)
- `/campaign` - Launch and manage campaigns
- `/ads` - Paid advertising management
- `/seo` - Search optimization audits

### Content & Brand (5 Commands)
- `/brand` - Brand design and guidelines
- `/content` - Content planning and creation
- `/social` - Social media scheduling
- `/design` - Graphic asset creation
- `/document` - Marketing documentation

### Analytics & Outreach (6 Commands)
- `/analytics` - Performance reporting
- `/partnership` - Partnership outreach
- `/optimize` - Campaign optimization
- `/estimate` - Budget estimation
- `/cleanup` - Campaign cleanup
- `/git` - Repository management

### Workflow (5 Commands)
- `/load` - Project context loading
- `/task` - Task management
- `/spawn` - Parallel task execution
- `/explain` - Campaign explanations
- `/troubleshoot` - Debug framework issues

## 🔧 Technical Architecture v2

SuperClaude v2's architecture enables extensibility:

**🏗️ Modular Configuration**
- **CLAUDE.md** – Core configuration with @include references
- **.claude/shared/** – Centralized YAML templates
- **commands/shared/** – Reusable command patterns
- **@include System** – Template engine for configuration

- **Marketing Commands** – Campaign lifecycle coverage
- **Flag Inheritance** – Universal flags on all commands
- **Persona Integration** – 9 cognitive modes as flags
- **Template Validation** – Reference integrity checking

**📦 Architecture Benefits**
- **Single Source of Truth** – Centralized updates
- **Easy Extension** – Add new commands/flags
- **Consistent Behavior** – Unified flag handling
- **Reduced Duplication** – Template-based configuration

**✅ Quality Features**
- **Evidence-Based Approach** – Documentation encouraged
- **Research Integration** – Library documentation access
- **Error Recovery** – Graceful failure handling
- **Structured Output** – Organized file locations

## 📊 Comparison

| Aspect | Standard Claude | SuperMarketer Framework |
|--------|----------------|------------------------|
| **Expertise** | General responses | 9 marketing personas |
| **Commands** | Manual prompts | Marketing workflow commands |
| **Context** | Session-based | Campaign history support |
| **Tokens** | Standard usage | Compression options |
| **Approach** | General purpose | Data-driven marketing |
| **Documentation** | As needed | Systematic campaign docs |
| **Quality** | Variable | Validation patterns |
| **Integration** | Basic tools | MCP orchestration |

## 🔮 Use Cases

**Marketing Teams**
- Consistent approaches across channels
- Standardized campaign workflows
- Data-driven decisions
- Brand documentation practices

**Marketing Directors**
- Strategy reviews
- Performance optimization
- Creative quality improvement
- Team knowledge sharing

**Campaign Operations**
- Campaign deployment procedures
- Troubleshooting workflows
- Asset management
- Maintenance tasks

## 🎯 Suitability

**Good fit for:**
- ✅ Teams wanting consistent AI assistance
- ✅ Projects needing specialized approaches
- ✅ Evidence-based marketing practices
- ✅ Token-conscious workflows
- ✅ Domain-specific expertise needs

**May not suit:**
- ❌ Purely manual workflows
- ❌ Minimal configuration preferences
- ❌ Ad-hoc marketing styles
- ❌ Single-domain focus

## 🚦 Getting Started

1. **Install SuperClaude**
   ```bash
   git clone https://github.com/NomenAK/SuperClaude.git && cd SuperClaude && ./install.sh
   ```

2. **Validate Installation**
   ```bash
   /load                                    # Load project context
   /campaign --help                         # Verify command access
   /seo --audit --persona-seo               # Test personas
   ```

3. **Example Workflow**
   ```bash
   /campaign --launch --persona-brand       # Plan campaign
   /ads --create --budget 1000              # Launch ads
   /analytics --report --persona-analytics  # Analyze results
   ```

## 🛟 Support

- **Installation Help**: Run `./install.sh --help`
- **Command Details**: Check `~/.claude/commands/`
- **Contributing**: See [CONTRIBUTING.md](CONTRIBUTING.md)
- **Issues**: [GitHub Issues](https://github.com/NomenAK/SuperClaude/issues)

## 🤝 Community

SuperClaude welcomes contributions:
- **New Personas** for specialized workflows
- **Commands** for domain-specific operations
- **Patterns** for marketing practices
- **Integrations** for productivity tools

Join the community: [Discussions](https://github.com/NomenAK/SuperClaude/discussions)

## 📈 Version 2.0.1 Changes

**🎯 Architecture Improvements:**
- **Configuration Management**: @include reference system
- **Token Efficiency**: Compression options maintained
- **Command System**: Unified flag inheritance
- **Persona System**: Now available as flags
- **Installer**: Enhanced with new modes
- **Maintenance**: Centralized configuration

**📊 Framework Details:**
- **Commands**: 19 specialized commands
- **Personas**: 9 cognitive approaches
- **MCP Servers**: 4 integrations
- **Methodology**: Evidence-based approach
- **Usage**: By marketing teams

## 🎉 Enhance Your Marketing

SuperMarketer provides a structured approach to using Claude with specialized marketing commands, personas, and workflows.

---

*SuperMarketer v2.0.1 – Marketing framework for Claude*

[⭐ Star on GitHub](https://github.com/NomenAK/SuperClaude) | [💬 Discussions](https://github.com/NomenAK/SuperClaude/discussions) | [🐛 Report Issues](https://github.com/NomenAK/SuperClaude/issues)

# Star History

<a href="https://www.star-history.com/#NomenAK/SuperClaude&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=NomenAK/SuperClaude&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=NomenAK/SuperClaude&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=NomenAK/SuperClaude&type=Date" />
 </picture>
</a>