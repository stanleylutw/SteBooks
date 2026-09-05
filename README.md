# STeBooks

史丹利的免費電子書網站。

網站適合直接用 GitHub Pages 發布，根目錄的 `index.html` 是整個電子書網站入口，各章節放在 `chapters/` 底下。

## Project Structure

```text
STeBooks/
  index.html
  chapters/
    chapter-01/
      index.html
      00_preface.html
      01_philosophy.html
      style.css
      assets/
        cover.png
        toc.png
```

## Add A New Chapter

1. Create a folder such as `chapters/chapter-02/`.
2. Add that chapter's `index.html`, article pages, `style.css`, and images.
3. Update the book list in the root `index.html`.
4. Commit the change:

```bash
git add .
git commit -m "Add chapter 02"
git push origin main
```

## GitHub Pages

In GitHub, open `Settings > Pages`, then publish from the `main` branch root.

Expected site URL:

```text
https://stanleylutw.github.io/SteBooks/
```
