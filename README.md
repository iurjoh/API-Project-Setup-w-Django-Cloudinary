# Django and Cloudinary setup exercise

[Português (Brasil)](README.pt-BR.md) | **English**

An early Django configuration exercise with Cloudinary media-storage settings. The repository name describes an API setup, but the reviewed URL configuration exposes only the Django admin route; this is not documented as a completed API.

**Documentation reviewed:** 2026-10-01. No tests, migrations or runtime checks were run.

## Purpose and development record

The project starts from the Code Institute student template. `manage.py` and the `API_PROJECT/` settings/URL files are present. The previous root README was generic template guidance, not a project-specific planning record. No completed design process or API feature history is invented here.

## Architecture and configuration

Django project configuration is in `API_PROJECT/`. `urls.py` currently includes `admin/` only. Settings use SQLite (`db.sqlite3`) and a Cloudinary media-storage class.

The configuration is incomplete: adjacent entries in `INSTALLED_APPS` lack commas, which concatenates strings into invalid app names. A root `requirements.txt` was not found; exact dependency installation cannot be reproduced from a pinned dependency file in this review.

## Security before reuse

The public settings file contains a literal development `SECRET_KEY`, and `DEBUG` is enabled. Do not reuse that key for a deployed service. Use a new environment-managed key for any real installation and review debug, hosts, media credentials and access rules. This documentation does not reproduce or use the key, change configuration or publish the app.

## Local setup status

Do not treat the old template instructions as a verified setup recipe. First fix `INSTALLED_APPS`, record dependencies, separate local secrets and validate configuration. Then use an isolated environment and fictional data to test the project with `python3 manage.py check` before migrations or runtime use. No successful run is claimed here.

## Design, tests and snapshots

This is backend setup work, not a finished UI. The update read settings, URL configuration, `manage.py` and the previous README only. Future checks should cover configuration, database migrations, media storage and permissions. Dated screenshots of safe example output belong in `docs/assets/`; no fresh snapshot is embedded.

## Credits and license

Code Institute student template and third-party Django/Cloudinary software. No root `LICENSE` was found in this review. Preserve their terms; this update does not apply MIT over third-party code or mistake template release notes for the author's development history.
