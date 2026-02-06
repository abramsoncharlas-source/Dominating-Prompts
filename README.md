# Dominating Prompts

This repository contains a minimal GitHub Pages site for dominatingprompts.com. Files added by GitHub Copilot Chat Assistant include a basic index.html, a CNAME to claim the custom domain, a simple stylesheet, and a GitHub Actions workflow that runs static checks (HTML validation, link checking, accessibility checks) on pushes to main.

To publish the site:
1. Ensure Pages is enabled for the `main` branch (root) in repository Settings → Pages.
2. Add DNS records for `dominatingprompts.com` at your domain provider:
   - Apex (dominatingprompts.com): A records to GitHub Pages IPs: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153 (or ALIAS/ANAME).
   - www: CNAME to abramsoncharlas-source.github.io
3. Wait for DNS propagation and verify the custom domain under Settings → Pages.

CI workflow will run on every push to main. See .github/workflows/pages-check.yml for details.
