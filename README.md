# xsd-editor-pro
Browser based XSD tree editor and generator. Paste any XSD, explore it as a tree, tweak the structure, and generate a clean schema in seconds.

# XSD Editor Pro - Universal XSD Tree Editor

XSD Editor Pro is a single page, browser based tool for working with XML Schema (XSD) without any heavy IDEs, plugins, or backend services.

Paste an XSD, inspect it as a tree, tweak the structure, and generate a clean, formatted schema that you can download or copy back into your project.

---

## Why this exists

Working directly in raw XSD is painful:

- Deeply nested structures are hard to see in a normal editor.
- Attributes, documentation, and min/max occurrences are scattered all over the place.
- A small change often needs edits in multiple spots.

This tool gives you a focused, table driven view of your schema so you can think in terms of elements and attributes, not angle brackets.

Everything runs 100 percent in the browser. No data is sent anywhere.

---

## Features at a glance

- **Paste any XSD**  
  Drop in an existing schema and let the tool parse and map it into an editable tree.

- **Tree based editor**  
  - Visual hierarchy with indentation and badges for complex types and attributes  
  - Resizable columns for Name, Category, Type, Min, Max, Use/Default, Description  
  - Per row description with automatic annotation generation in the output XSD

- **Add, remove, and reorder structure**  
  - Add sibling or child nodes with one click or keyboard shortcuts  
  - Attribute support with `use` and default values  
  - Safe delete that removes a node and its full subtree

- **Smart search**  
  - Search tree nodes by name, description, type, or even XPath like paths  
  - Highlights matches and expands parent complex types so you can see context  
  - Separate search box for the generated XSD with next/previous navigation

- **XSD generation and validation**  
  - Generates a full `<xs:schema>` with root element, complex types, sequences, attributes, and annotations  
  - Optional target namespace and `elementFormDefault` metadata (internally tracked)  
  - Client side XML validation using `DOMParser` so you can catch basic syntax issues

- **Clipboard and download**  
  - Copy the generated XSD to the clipboard with one click  
  - Download as `<RootElementName>.xsd` using a client side Blob

- **Dark mode and auto save**  
  - Dark and light themes with a simple toggle, stored in `localStorage`  
  - Auto save of the full tree, metadata, selection, and original XSD per browser, with a restore prompt on load

- **No backend, no build step**  
  One HTML file, one `<script>` block, nothing else. Perfect for GitHub Pages.

---

## Getting started

You can use this in two ways:

### 1. Use it on GitHub Pages

Once the repo is wired to GitHub Pages, open:

```text
https://<your-username>.github.io/xsd-editor-pro/

