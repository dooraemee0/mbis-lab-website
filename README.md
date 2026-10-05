Visit **[dooraemee0.github.io/mbis-lab-website](https://dooraemee0.github.io/mbis-lab-website)** 🚀

# MBIS Lab Website

Official website source for the Multimodal Biomedical Imaging and System Laboratory at DGIST.

- Current GitHub Pages site: <https://dooraemee0.github.io/mbis-lab-website/>
- Planned custom domain: <https://mbis.dgist.ac.kr/>
- Planned repository owner: [MBIS-Git](https://github.com/MBIS-Git)

## Editing the website

The repository is the source of truth. Do not edit generated files in `_site/` or files copied to the NAS web directory.

```bash
git clone https://github.com/MBIS-Git/mbis-lab-website.git
cd mbis-lab-website
bundle install
bundle exec jekyll serve
```

Open <http://localhost:4000>, make changes, and verify the result. Then publish the source changes:

```bash
git add <changed-files>
git commit -m "Describe the website update"
git push origin main
```

A push to `main` runs the existing GitHub Actions workflow, builds the Jekyll site, and publishes the result to the `gh-pages` branch.

### Where to edit

| Content | Location |
|---|---|
| Research areas | `_data/research.yaml` |
| Research projects | `_data/projects.yaml` |
| Publications | `publications/index.md`, `_data/publications.yaml` |
| Members | `_members/` and `images/people/` |
| News | `_data/activity_news.yaml` and `images/blog/news/` |
| Awards | `_data/activity_awards.yaml` and `images/blog/award/` |
| Photos | `_data/activity_photos.yaml` and `images/blog/photo/` |
| AI seminars | `_data/activity_ai_seminars.yaml` and `images/blog/ai-seminar/` |

## GitHub access

At least two lab members should have repository admin access. Other maintainers normally need `Write` access.

After transferring the repository to `MBIS-Git`:

1. Open `Settings → Collaborators and teams`.
2. Give the PI and the primary website manager `Admin` access.
3. Give additional maintainers `Write` access.
4. Keep individual GitHub accounts; do not share one password or access token.

## Custom domain

Complete these steps only after GitHub Pages is enabled for the `MBIS-Git` organization.

1. In the repository, open `Settings → Pages`.
2. Confirm that the publishing source is the `gh-pages` branch and `/ (root)` directory.
3. Set the custom domain to `mbis.dgist.ac.kr`.
4. Ask the DGIST DNS administrator to replace the current DNS record with:

   ```text
   Type:   CNAME
   Name:   mbis
   Target: mbis-git.github.io
   ```

5. After DNS propagation and certificate issuance, enable `Enforce HTTPS` in GitHub Pages.

Do not add the custom domain before the organization has Pages enabled and the DNS change is scheduled; doing so can make the current GitHub Pages URL redirect to an unavailable domain.

## NAS backup and deployment

GitHub Pages is the recommended public host. The NAS should keep two separate items:

1. **Source backup** — a clone of this entire repository, including `.git`.
2. **Deployment backup** — the latest NAS ZIP generated from `_site/`.

Suggested NAS layout:

```text
/volume1/MBIS/website-source/     # repository clone; not publicly served
/volume1/MBIS/website-backups/    # dated deployment ZIP files
/volume1/web/mbis/                # optional NAS-hosted copy of _site contents
```

Create a NAS deployment ZIP locally:

```bash
bundle exec jekyll build
(cd _site && zip -qr ../mbis-lab-website-nas.zip .)
```

If the NAS must host the site, extract the ZIP contents directly into `/volume1/web/mbis/`. `index.html` must be directly inside that directory. The Jekyll source folders (`_data`, `_includes`, `_layouts`, and so on) should not be placed in the public web directory.

## Recovery

On a new computer or after a NAS failure:

```bash
git clone https://github.com/MBIS-Git/mbis-lab-website.git
cd mbis-lab-website
bundle install
bundle exec jekyll build
```

All permanent changes must be committed and pushed to GitHub so that maintenance does not depend on one person's computer or NAS account.
