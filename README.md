# ssh-to-PKGBUILD

Arch Linux PKGBUILD recipes for [ssh-to](https://github.com/xsigil/ssh-to).

## Packages

* **`PKGBUILD`**: Stable release package.
* **`PKGBUILD-git`**: Tracks the latest master branch commit.

---

## Installation

### Manual Installation via `makepkg`

```bash
git clone [https://github.com/xsigil/ssh-to-PKGBUILD.git](https://github.com/xsigil/ssh-to-PKGBUILD.git)
cd ssh-to-PKGBUILD

# Build and install the git version
makepkg -p PKGBUILD-git -si

```

---

## Upstream

* Source: [https://github.com/xsigil/ssh-to](https://www.google.com/url?sa=E&source=gmail&q=https://github.com/xsigil/ssh-to)
* License: MIT
EOF

cat << 'EOF' > .gitignore
/pkg/
/src/
/ssh-to/
*.pkg.tar.*
*.log
EOF

```

#### 4. `ssh-to-PKGBUILD` を GitHub に公開

```bash
git init
git add PKGBUILD PKGBUILD-git README.md .gitignore
git commit -m "feat: initial commit of PKGBUILD definitions for ssh-to"

gh repo create ssh-to-PKGBUILD --public --source=. --remote=origin --push

```
