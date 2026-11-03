# Security settings checklist

These are GitHub settings, not files, so they have to be switched on in the web UI.
Do them once on a computer; most take a single click.

## 1. Your account
- [ ] **2FA on** with an authenticator app or passkey: github.com/settings/security
- [ ] Save your **recovery codes** in a password manager

## 2. Organization: github.com/organizations/neuro-kitchen/settings
- [ ] **Authentication security → Require two-factor authentication** for everyone in the org
- [ ] **Member privileges → Base permissions: Read.** Grant Write per repo, never org-wide.
- [ ] **Member privileges → Repository creation:** only you, while you're solo
- [ ] **Actions → General → Workflow permissions: "Read repository contents"**,
      and untick "Allow GitHub Actions to create and approve pull requests"
- [ ] **Actions → General → Fork pull request workflows:** require approval for all outside collaborators
- [ ] **Code security → Configurations:** apply the **GitHub recommended** configuration to all repos.
      It turns on Dependabot alerts and security updates, secret scanning, push protection,
      and private vulnerability reporting.
- [ ] **GitHub Apps → Claude → Configure:** limit repository access to only the repos Claude should work on

## 3. Protect `main` in every repo
Org settings → **Repository → Rulesets → New ruleset → New branch ruleset**:
- [ ] Name: `protect-main`, Enforcement: **Active**
- [ ] Target repositories: **All repositories**
- [ ] Target branches: **Include default branch**
- [ ] Tick **Restrict deletions**
- [ ] Tick **Block force pushes**
- [ ] Tick **Require a pull request before merging** (required approvals: 0 while you're solo)
- [ ] Bypass list: leave empty, or add only yourself (Organization admin) for emergencies

## 4. In each project repo
- [ ] Add a `LICENSE` file: **Add file → Create new file**, name it `LICENSE`, then pick
      **Choose a license template → Apache License 2.0**
- [ ] Copy `per-repo-templates/dependabot.yml` to `.github/dependabot.yml`
- [ ] Copy `per-repo-templates/CITATION.cff` to the repo root and fill it in
- [ ] **Settings → General:** untick "Allow merge commits" if you prefer squash merges (optional)
