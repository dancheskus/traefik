# Basic `traefik` container setup

This setup allows you to run `traefik` container with corresponding settings
- ACME challenge will try to receive `wildcard` certificates for url's that other containers requested
- All `http://` requests will be redirected to `https://`
- All `https://www.example.com` requests will be redirected to `https://example.com`
- Only registred in `traefik` url's will be accessible. wrong.example.com will not be accessible (no `traefik`'s 404 page). correct.example.com will be accessible.

#### Running container
`docker-compose up -d`

---
Read about react connected to `traefik` [setup](https://github.com/dancheskus/traefik_react_project_setup)