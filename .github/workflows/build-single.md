# Build a Single Dynmap Version via GitHub Actions

This workflow lets **maintainers and contributors** safely build a **specific Dynmap version** for **Bukkit, Forge, or Fabric** using GitHub Actions.  
You can also **automatically create a GitHub prerelease** with the built artifacts.

---

## ⚠️ **Required Repository Secret**

| Secret Name | Purpose |
|------------|--------|
| `TOKEN_GITHUB` | GitHub PAT with: <br> • **Repo access**: Full (current repo + S3 deps) <br> • **Permissions**: `contents: read & write` (for release assets) |

> Generate at: [github.com/settings/personal-access-token](https://github.com/settings/personal-access-tokens) (select **repo** scope)

---

## 🚀 How to Use

1. Go to **Actions** → Select **"Build single Dynmap version"**
2. Click **"Run workflow"**
3. Choose:
   - **Branch**: usually `v3.0`
   - **Platform**: `bukkit`, `forge`, or `fabric`
   - **Dynmap Game Version**: `1.21.5`
   - **Create Prerelease?** (optional) → auto-generates release + tag *(token required)*
4. Click **Run workflow**

Done! Your build will appear in the workflow run and (if enabled) as a prerelease.