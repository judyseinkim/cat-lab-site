# CAT Lab Website

Built with Quarto. Warm earthy design, clean sans-serif throughout.

## Quick start

```bash
quarto preview           # live preview at localhost:4444
quarto publish gh-pages  # deploy to GitHub Pages
```

## Files

| File | Purpose |
|------|---------|
| _quarto.yml | Site config and nav |
| styles.css | All visual design |
| index.qmd | Home — logo + description |
| people.qmd | People + bios |
| publications.qmd | Publications list |
| projects.qmd | Research lines + join |
| news.qmd | News feed |
| images/ | Photos and project figures |

## Common edits

### Add your logo
Put cat-lab-logo.png in images/, then in index.qmd replace:
  <div class="logo-placeholder">CAT</div>
with:
  <img src="images/cat-lab-logo.png" class="lab-logo" alt="CAT Lab logo">

### Add a person photo
In people.qmd, replace the avatar div for that person:
  <div class="person-avatar">AC</div>  →  <img src="images/alice-chen.jpg" class="person-photo" alt="Dr. Alice Chen">

### Add a project figure
In projects.qmd, find the panel and replace:
  <div class="fig-pill"></div>
  <div class="fig-label">Figure / image</div>
with:
  <img src="images/project1.png" alt="Short description">

### Add a publication (paste under the right year in publications.qmd)
<div class="pub-entry">
  <div class="pub-dot"></div>
  <div>
    <div class="pub-title">Title here</div>
    <div class="pub-meta">Author, A. — <em>Journal</em>, vol, pages</div>
    <div class="pub-links"><a href="URL">PDF</a></div>
  </div>
</div>

### Add a news item (paste at the top of news.qmd)
<div class="news-entry">
  <div class="news-date">Mon<br>YYYY</div>
  <div>
    <span class="news-badge badge-paper">New paper</span>
    <div class="news-title">Title</div>
    <div class="news-body">Body text.</div>
  </div>
</div>
Badge options: badge-paper, badge-award, badge-event, badge-lab

### Change colors (top of styles.css)
--accent: #b85c38   (terracotta)
--pink:   #fab3cc   (logo pink, used for dots/badges)
--bg:     #f7f3ed   (page background)
