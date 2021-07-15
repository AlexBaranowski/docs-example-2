# Home

**THIS IS Proof of Concept - remove all FIXME and TODO before creating prod repo**

Several of the EuroLinux documentation are open source and hosted on GitHub and
GitHub pages. There are also docs for our customer that are available at
[EuroLinux Support Portal](https://support.euro-linux.com). You can make changes and
even create documentation via pull requests.

Open sourcing documentation allows us to:

- Streamline changes in documentation in easy to understand manner
- Everyone can create requests for particular topic via [Issue Creation on
  GitHub FIXME]()
- Build community and engage it in process

## Contriubution guide

We are using `mkdocs` with `mkdocs-material` to build and style our
documentation.

- [MkDocs site](https://mkdocs.readthedocs.io/en/stable/)
- [Material for MkDocs site](https://squidfunk.github.io/mkdocs-material/)

### Setup environment locally

Firstly it's good idea to create virtualenv, so you don't bloat your system
python environment:
```
virtualenv -p /usr/bin/python3 venv
```
Then activate virtualenv

Bash:
```bash
. venv/bin/activate
```
Fish:
```fish
. venv/bin/activate.fish
```

Now you are ready to install mkdocs and python packages:
```
pip install -r requirements.txt
```

## How to run or build

Run:
```
mkdocs serve
```

Build:
```
mkdocs build
```

### mkdocs-material

In theory this is just template, but it's template that really work


### Markdown cheetsheet for this project
[Here](HowTo/documentation-markdown.md)

