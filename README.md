# Linux Docs-as-Code Demo

A small documentation site that shows a docs-as-code workflow: tutorials are written in
AsciiDoc, stored in Git, and built into a website automatically with GitHub Actions and
GitHub Pages.

## Contents

- `index.adoc` - site home page
- `ssh-basics.adoc` - tutorial: Getting started with SSH on Linux
- `.github/workflows/pages.yml` - builds the HTML and deploys it to GitHub Pages

## Build locally

Install Asciidoctor (`sudo dnf install rubygem-asciidoctor` on Fedora, or
`sudo apt install asciidoctor` on Ubuntu), then run:

```bash
mkdir -p _site
asciidoctor -D _site *.adoc
```

Open `_site/index.html` in your browser.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

MIT - see [LICENSE](LICENSE).
