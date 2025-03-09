# Grocery Gooose Site

Grocery Goose is a site that allows you to learn about the grocery goose app and sign up for the waitlist.

## Development

### Running the site locally


#### Create a virtual environment and install dependencies (3.11.3)

```bash
pyenv virtualenv 3.11.3 grocery-goose-site-3.11.3
```

```bash
pyenv activate grocery-goose-site-3.11.3
```

```bash
pip install -r requirements.txt
```

```bash
mkdocs serve
```

Visit `http://127.0.0.1:8000` to view the site.

### Deploying the site

```bash
mkdocs gh-deploy
```

This will deploy the site to the `gh-pages` branch.

### Updating the site

```bash
mkdocs build
```