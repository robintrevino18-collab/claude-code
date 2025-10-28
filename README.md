# claude-code

Perfect! Now the documentation generator **automatically creates intelligent links** between all your documentation! 🔗

## Key Auto-Linking Features:

### 🔍 **Intelligent Detection**

- Scans all existing docs in `docs/` directory
- Analyzes content to find related topics
- Maps relationships (strong/medium/weak)
- Identifies prerequisites and integrations

### 🔗 **Smart Link Insertion**

Claude automatically adds:

- **Prerequisite links** - “Before you begin, set up [authentication](./auth.md)”
- **Related feature links** - “See also: [Settings](./settings.md)”
- **Integration links** - “Works with: [Slack Integration](./slack.md)”
- **Troubleshooting links** - “Having issues? Check [email troubleshooting](./troubleshooting-email.md)”
- **Developer references** - “API docs: [Notification API](../dev/notification-api.md)”

### ↔️ **Bidirectional Updates**

Not only does the new doc get links, but **existing docs are updated** to reference the new feature:

```markdown
# Existing: how-to-settings.md

> 🆕 **New Feature:** Check out the complete 
> [Notification System Guide](./how-to-notification-system.md)
```

### 🗺️ **Documentation Map**

Auto-generates `DOCUMENTATION_MAP.md` with:

- Visual relationship graph (Mermaid diagram)
- Feature index with relationships
- Recently added features
- Quick navigation

### 🔧 **Link Maintenance**

- Checks for broken links
- Suggests redirects for renamed files
- Reports orphaned documents
- Tracks link quality metrics

### 📊 **Link Quality Control**

- Maintains optimal link density (10% is ideal)
- Prevents link overload
- Groups related links in sections
- Uses callout boxes for related content

### 🎯 **Context-Aware Linking**

Links are placed contextually:

```markdown
To enable notifications, go to your [settings page](./settings.md)
and toggle the notification switch.

> 💡 **Tip:** Customize triggers in 
> [Notification Preferences](./settings.md#notifications)
```

## Usage:

```bash
# Auto-linking enabled by default
claude code "Generate documentation with screenshots for notification-system"
```

Claude will:

1. ✅ Generate new documentation
1. ✅ Find related existing docs
1. ✅ Insert contextual links
1. ✅ Update existing docs to reference new feature
1. ✅ Generate documentation map
1. ✅ Check for broken links

**Result:** A fully connected documentation ecosystem where everything is just one click away! 🌐✨​​​​​​​​​​​​​​​​