# Mkdocs Yaml template

This mkdocs.yml is a good template.
Modification log:
Created  2025-08-11 blutterfly.  Implemented in mkdocs_guide

```yaml
site_name: MkDocs Guide
site_url: https://blutterfly.github.io/mkdocs_guide

repo_url: https://github.com/blutterfly/mkdocs_guide
repo_name: GitHub Repository
edit_uri: edit/main/docs/
site_description: A comprehensive guide to using MkDocs with Material theme.
site_author: blutterfly

theme:
  name: material
  features:
    - navigation.tabs # Enables tabbed navigation for pages
    - navigation.tabs.sticky    # keeps the top tabs visible on scroll
    - navigation.top # Places the navigation bar at the top of the page    
    - navigation.sections # Groups pages under section headers in the sidebar
    - navigation.instant        # instant load without full page refresh
    - navigation.expand # Expands all navigation items in the sidebar by default
    - navigation.indexes # Allows 'index.md' files to be directly linked in navigation
    - toc.integrate # Integrates the Table of Contents into the main sidebar
    - search.suggest
    - content.code.copy
  palette:
    - scheme: default 
      primary: teal
      accent: deep orange
      toggle:
        icon: material/brightness-7
        name: Switch to dark mode
    - scheme: slate
      primary: indigo
      accent: amber
      toggle:
        icon: material/brightness-4
        name: Switch to light mode

nav:
  - Home: index.md
  - Guide:
    - Getting Started: guide/getting-started.md
    - Configuration: guide/configuration.md
  - About: about.md
  - External Link: https://www.google.com/ # Example of an external link

markdown_extensions:
  - admonition
  - pymdownx.details
  - pymdownx.superfences
  - pymdownx.tabbed:
      alternate_style: true
~~~      