# app.myers.io

Static landing and per-app support/marketing pages served at
[app.myers.io](https://app.myers.io/).

Each published app gets its own folder (e.g. `pickled/`) containing a
marketing page (`index.html`) and a support page (`support/index.html`).

## Deployment

Deployed by the Ansible playbook in the `Config` repo
(`ansible/vps.yml`), which syncs this repo to `/var/www/app` and serves it
via nginx (`Config/nginx/app.myers.io`). This is plain static content with
no build step.
