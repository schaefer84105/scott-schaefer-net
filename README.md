# scott-schaefer.net static site

GitHub Pages-ready static replacement for the existing WordPress site.

## Publish

1. Create a PUBLIC GitHub repository. A simple name such as `scott-schaefer.net` is fine.
2. Upload everything in this folder to the root of the repository.
3. In GitHub: **Settings -> Pages -> Build and deployment -> Deploy from a branch**.
4. Select **main** and **/(root)**, then save.
5. Under **Custom domain**, enter `scott-schaefer.net` and save.
6. Do not change the live DNS until the GitHub Pages preview is working.

## DNS cutover

At your domain/DNS provider, point the apex domain to GitHub Pages with A records:

- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

Also create a CNAME record for `www` pointing to `YOUR-GITHUB-USERNAME.github.io`.

After DNS has propagated and GitHub shows the domain is configured correctly, enable **Enforce HTTPS** in Settings -> Pages.

## Existing URLs preserved

- `/`
- `/bio/`
- `/contact-information/`
- `/cv/`

The headshot and CV PDF have been copied into this repository, so the finished site will not depend on the old WordPress host.
