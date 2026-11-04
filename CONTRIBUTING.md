# Contributing to HSE CS Open Source

Thank you for helping maintain this collection of open-source projects and resources created by HSE CS staff and students. Contributions can include new projects, corrected links, updated descriptions, and improvements to the documentation.

## Add or update a project

To suggest a project, simply [open an issue](https://github.com/hse-cs/open-source/issues/new) with a link to the project and, optionally, a link to its associated paper. A paper is not required. We will add the project to the collection ourselves; you do not need to submit a pull request.

If you prefer to add or update an entry yourself, follow these steps:

1. Check [README.md](README.md) for an existing entry to avoid duplicates.
2. Make sure the project or resource is publicly accessible. For software projects, check that the repository includes an open-source license.
3. Add the entry to the appropriate year in `README.md`. Use the release or publication year, and keep year sections in descending order.
4. Follow the existing format, using an English title and a concise, factual description where needed:

   ```markdown
   - [Project title or short description](https://github.com/owner/repository) - **Project name**, [paper](https://example.org/paper) (2026)
   ```

   Omit the paper link if there is no associated publication. Prefer a direct repository link and a stable publication link, such as a DOI, publisher page, or arXiv abstract.

For corrections, briefly explain what was inaccurate and provide a source when relevant. Problems with a listed project's code should be reported in that project's own repository.

## Edit the website

The website is built with MkDocs:

- `README.md` contains the project catalog. `docs/index.md` includes it automatically, so edit the catalog in `README.md`.
- `mkdocs.yml` contains the site configuration and navigation.
- `site/` contains generated output and is ignored by Git. Do not commit generated files.

Keep the documentation in English and follow the surrounding Markdown style.

### Preview locally

From the repository root, create a Python virtual environment and install the packages used by the site:

```sh
python3 -m venv .venv
source .venv/bin/activate
python -m pip install mkdocs markdown-include
python -m mkdocs serve
```

On Windows, activate the environment with `.venv\Scripts\activate` instead. Open the local address printed by MkDocs and check the affected pages, formatting, and links.

To check that the site builds, run:

```sh
python -m mkdocs build
```

## Submit a pull request

1. Fork the repository and create a branch for your change.
2. Keep the change focused and avoid unrelated reformatting.
3. Check the Markdown preview and open any links you added or changed. For website changes, preview and build the site using the commands above.
4. Open a pull request with a clear title and a short description of what changed, why, and how you checked it. Include supporting sources and related issue links where applicable.
5. Address review feedback in the same pull request.

Small additions and fixes can be submitted directly as pull requests. For larger structural changes or questions about whether a resource belongs in the collection, open an issue first.

## License and communication

Contributions to this repository are made under its [MIT license](LICENSE). Listed projects retain their own licenses.

Be respectful and constructive in issues, pull requests, and reviews. Discuss the proposed changes and give credit to project authors.
