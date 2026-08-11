# Publish to GitHub

**Project author:** Yagni Patel

Use whichever GitHub account you want. The package is account-agnostic; no GitHub username is embedded in the repository files. Public-facing project attribution is set to Yagni Patel.

Recommended repository name:

```text
microsoft-dcf-analysis
```

## Recommended repository metadata

**Description**

```text
Segment-driven Microsoft DCF, reverse DCF, ROIC, lease-adjusted UFCF, Buffett-inspired assessment, and AI/cloud investment memo.
```

**Topics**

```text
financial-modeling
dcf
valuation
microsoft
corporate-finance
equity-research
business-analytics
excel
reverse-dcf
roic
investment-memo
```

## Browser upload method

1. Sign in to the GitHub account you want to use.
2. Create a new **public** repository named `microsoft-dcf-analysis`.
3. Do not initialize it with a README, `.gitignore`, or license because this package already contains those files.
4. Open the empty repository and select **uploading an existing file**.
5. Upload the **contents** of the `microsoft-dcf-analysis` folder, preserving the `assets`, `data`, `docs`, and `model` directories.
6. Use the commit message:

```text
Initial release: Microsoft DCF, business-quality analysis, and investment memo
```

7. Confirm that `assets/dashboard_overview.png` and `assets/buffett_5_tenets.png` render in the README.
8. Pin the repository on your GitHub profile.

## Git command method

Replace `<YOUR_GITHUB_USERNAME>` with the account you intend to use.

```bash
git init
git add .
git commit -m "Initial release: Microsoft DCF, business-quality analysis, and investment memo"
git branch -M main
git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/microsoft-dcf-analysis.git
git push -u origin main
```

## Before publishing

- Open the Excel model and confirm formulas recalculate without warnings.
- Keep the educational-use and not-investment-advice disclaimer.
- Verify that the valuation date and market price are clearly disclosed.
- Do not include personal student IDs, school login details, or SharePoint URLs.
