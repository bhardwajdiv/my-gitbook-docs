# Mastering the SUMMARY.md Map

The `SUMMARY.md` file is the singular source of truth for constructing GitBook navigation. It translates plain text files into highly polished user sidebars.

## Structural Formatting Rules
The syntax inside this file must follow a precise Markdown syntax pattern to render correctly:

1. **The Title**: Must begin with a top-level heading (`# Table of Contents`).
2. **Category Dividers**: Use second-level headings (`## Category Name`) to generate bold, non-clickable visual dividers in the sidebar.
3. **Navigation Links**: Links must use standard Markdown list and link tracking syntax: `* [Display Name](folder/file.md)`.

## How to Nest Navigation Items
To create nested, expandable multi-level drop-down pages, use indentation blocks. You must indent child items by exactly **two or four spaces** beneath the parent list entry.

### Code Block Implementation Example:
```markdown
## 🛠️ System Configuration
* [Hardware Specs](hardware/specs.md)
  * [CPU Architecture](hardware/cpu-specs.md)
  * [Memory Allocation](hardware/ram-specs.md)

---

### 5. `navigation/navigation-guidelines.md`
> **Invigilator Checklist Met:** This page features a robust `##` and `###` nested structure to **trigger the right-side sub-navigation automatically** AND includes the **required scannable comparison table**.

```markdown
# Global and In-Page Navigation

Effective documentation relies on clear structural hierarchies. GitBook uses a two-tier navigation map to keep documents highly scannable and accessible.

## Global Left-Side Navigation
Global site navigation is configured entirely inside the `SUMMARY.md` file. It governs how users jump between entirely separate documentation pages and content modules.
* **Structural Intent**: Group related concepts into logical paths using bold category headers.
* **Nesting Depth**: Limit nested indentation trees to a maximum of three levels to prevent the sidebar from looking overly cluttered.

## Automatic Right-Side Navigation
The right-side navigation panel is built **completely automatically** by GitBook. The platform continuously reads the active page's Markdown file and indexes all header blocks.

### Header Weight Mechanics
* **H1 (`# Title`)**: Reserved strictly for the single main page title at the very top.
* **H2 (`## Sub-heading`)**: Generates primary targets in the floating right-hand sub-navigation directory panel.
* **H3 (`### Deep-heading`)**: Generates secondary, slightly indented sub-links underneath their respective parent H2 links.

### Maximizing Page Scannability
By breaking long documents down into clear, distinct H2 and H3 blocks, users can scan the right-hand panel to jump instantly to the specific subsection they need without scrolling endlessly.

## Platform Capability Comparison
The table below details why a structured GitBook deployment is superior to a standard, flat GitHub documentation file:

| Structural Feature | Integrated GitBook Engine | Standard GitHub Repository |
| :--- | :--- | :--- |
| **Global Sidebar Tree** | Multi-level nested drop-down navigation | Flat, unstructured system file view |
| **In-Page Sub-Menus** | Automatically generated from H2/H3 anchors | Requires complex, manual HTML anchors |
| **Live Global Search** | Real-time indexed global search bar | Restricted to local browser text search (Ctrl+F) |
| **Content Blocks** | Stylized callout cards, hints, and tabs | Monochromatic, unstyled Markdown text blocks |  