# Home

**THIS IS Proof of Concept - remove all FIXME and TODO before creating prod repo**

Several of the EuroLinux documentation are open source and hosted on GitHub and
GitHub pages. There are also docs for our customer that are available at
[EuroLinux Support Portal](https://support.euro-linux.com). You can make changes and
even create documentation via pull requests.

Open sourcing documentation allows us to:

- Streamline changes in documentation in easy to understand manner
- Everyone can create requests for particular topic via [Issue Creation on
  GitHub FIXME](https://github.com/AlexBaranowski/docs-example-2/issues/new/choose)
- Build community and engage it in process

## How documentation is organized?

Documentation is organized in the following manner:

- JumpStarts - Installation guides with extras
- HowTo - How To guides on various topics
- Errats - EuroLinux erratas in the form of the web pages
- Release Notes 
 
## Contributors guide

We are using `mkdocs` with `mkdocs-material` to build and style our
documentation.

- [MkDocs site](https://mkdocs.readthedocs.io/en/stable/)
- [Material for MkDocs site](https://squidfunk.github.io/mkdocs-material/)


### Setup environment locally

Because MkDocs is Python based to run this documentation locally you need at
least:

- python3 (3.6+)
- pip
- virutalenv

Installed on your system.


Firstly lets create virtualenv, so you don't bloat your system python
libraries and environment:
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

Now you are ready to install mkdocs and other Python packages:
```
pip install -r requirements.txt
```

After it serving documentation on your host is as easy as running:
```
mkdocs serve
```

To build documentation invoke:
```
mkdocs build
```

It will build documentation and save it into `site` directory

!!! warning "Please don't include site directory in pull requests"
    Because we deploy this documentation with GitHub Pages the `site` directory
    is not gitignored


### Markdown cheat sheet for this project
We created simple cheat sheet for MkDocs markdown syntax with extensions
enabled in this project. It can be found
[Here](HowTo/documentation-markdown.md)
