# Contributions

Hi! We are happy that you thought of contributing! If you have any suggestions or issues, please raise it [here](https://github.com/codersforcauses/tech-docs/issues). I would be happy if you could provide pull requests, if you know how to do it [here](https://github.com/codersforcauses/tech-docs/pulls).

## Structure

### Folder Structure

The structure of this repo is as follows:

```
├── docs                    // Folders for documentation
│   ├── CNAME
│   ├── contributions.md
│   ├── deployment_and_automated_site_deployment.md
│   ├── flavoured_markdown.md
│   ├── images              // Assets
│   │   └── ...
│   │
│   ├── index.md
│   └── writing_markdown.md
├── LICENSE
├── mkdocs.yml              // MkDocs Configuration
├── overrides
│   └── partials
│       └── footer.html
├── README.md
└── requirements.txt
```

## Installation

### Ye olde way

```bash
python -m venv .venv
./.venv/Scripts/activate
pip install -r requirements.txt
mkdocs serve
```

### Docker

```bash
docker compose up
```

## Commands

- `mkdocs new [dir-name]` - Create a new project.
- `mkdocs serve` - Start the live-reloading docs server. Very helpful when you want to take a look at the docs before deploying.
- `mkdocs build` - Build the documentation site.
- `mkdocs -h` - Print help message and exit.
- `mkdocs gh-deploy` - Deploy in github pages
- `pip freeze > requirements.txt` - Generate a requirements.txt file

## Web Documentation Configuration

For full documentation visit:

- [mkdocs.org](https://www.mkdocs.org) for the generic MkDocs
- [PyMdown Extensions](https://facelessuser.github.io/pymdown-extensions/) for the different extensions that are installed
- [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) for the customisation of the web server documentation.
