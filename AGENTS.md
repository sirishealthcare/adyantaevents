# Repository Guidelines

## Project Structure & Module Organization

This repository is a small website rather than a compiled application. The main landing page is `index.html`; supporting pages and feeds are kept at the root alongside `main.css` and `style.css`. The landing page contains substantial page-specific markup and scripts, while reusable page styling and browser behavior live in the root stylesheets and `assets/js/`. `assets/css/`, `assets/js/`, `assets/fonts/`, `assets/images/`, and `assets/video/` hold frontend dependencies and site media. The `assets/libraries/PHPMailer/` and `assets/vendor/` directories provide PHP mailer and Composer runtime files used by the enquiry handler. `bk/` contains a separate older set of pages and styles.

## Build, Test, and Development Commands

No root-level package manifest, Makefile, or other build configuration defines build, lint, test, or development commands. The site has no configured automated build step. PHP is used by `business_enquiry.html`, so form handling requires a PHP-capable web server; opening the page as a static file will not execute that handler.

## Coding Style & Naming Conventions

No repository-level linter or formatter configuration is present. Keep edits consistent with the target file: page markup is primarily HTML, styles are split between CSS files, and interactive behavior uses JavaScript in `assets/js/` or page-level scripts. Preserve existing asset paths and filenames when updating references.

## Testing Guidelines

No test framework, test files, or test command is configured in the repository. Validate frontend changes in a browser and exercise enquiry handling only in a PHP-capable environment.

## Commit & Pull Request Guidelines

The available Git history contains only the initial `First commit`; it does not establish a commit-message convention. No pull-request template was found.
