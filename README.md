# Smart Library Management System

A browser-based library workspace, adapted by **Shakshi Jaiswal** from the original MIT-licensed C++ project by **Malik Moiz Ahmad Awan**.

## Website

https://Shakshi123jaiswal.github.io/smart-library-management-system/

The web app supports adding and removing books, searching by title / author / ID, sorting, borrowing and returning, FIFO waiting lists with automatic issue on return, and undo for the last 50 changes. Duplicate IDs and duplicate borrowers are rejected. Books on loan cannot be removed.

Data is saved in this browser’s local storage. This is a personal demo, not a shared library database: there are no accounts, server, permissions, or cross-device synchronization. Don't enter sensitive information. Clearing browser data removes your collection. Undo history lasts only for the current page session.

## Run the website locally

Serve the `docs` directory with any static web server, for example:

```sh
python3 -m http.server 8000 --directory docs
```

Open http://localhost:8000. No build step or dependencies are needed. Optional Google Fonts fall back to system fonts when offline.

## Deployment

GitHub Pages serves `docs/` from the `main` branch. Changes to `docs/index.html`, `docs/style.css`, or `docs/app.js` update the site after the next Pages build.

## Original C++ version

The original source is preserved in `src/` and `include/`. Run `make` then `./library` for the console app. See [README-CPP.md](README-CPP.md) for the original documentation. The website reimplements the behavior in JavaScript; it does not compile or execute the C++ source.

## Credits and license

- Web adaptation, interface and browser functionality: **Shakshi Jaiswal**.
- Original C++ implementation: **Malik Moiz Ahmad Awan**, BS Computer Science, University of Gujrat.
- MIT License. The original copyright notice is retained in [LICENSE](LICENSE).
