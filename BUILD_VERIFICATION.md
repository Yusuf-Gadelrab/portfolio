# SEO site build verification

## File tree

```text
seo_site/
├── .nojekyll
├── 404.html
├── about/index.html
├── favicon.svg
├── index.html
├── intakekit/index.html
├── research/index.html
├── robots.txt
├── sitemap.xml
├── writing/
│   ├── index.html
│   ├── parsing-freight-messages/index.html
│   ├── local-language-models-private-data/index.html
│   └── bilingual-programming-syntax/index.html
├── yusuf_headshot.jpg
├── yusuf-headshot.jpg
├── PUBLISH.md
└── BUILD_VERIFICATION.md
```

## Target-keyword map

| URL | Primary target keyword | Supporting terms |
|---|---|---|
| `/` | Yusuf Gadelrab | SJSU computer science, AI builder, CS tutor |
| `/research/` | Yusuf Gadelrab ACM SIGCSE 2026 | bilingual coding, adaptive curriculum maps, inclusive CS learning |
| `/intakekit/` | local-first intake parsing | WhatsApp load parsing, SMS intake, local document parsing |
| `/writing/` | Yusuf Gadelrab technical writing | freight automation, private AI, CS education |
| `/writing/parsing-freight-messages/` | freight intake automation | parse freight messages, structured load data, WhatsApp load parsing |
| `/writing/local-language-models-private-data/` | local-first document parsing | small language models locally, private client data |
| `/writing/bilingual-programming-syntax/` | bilingual computer science education | programming syntax, inclusive CS learning |
| `/about/` | Yusuf Gadelrab contact | SJSU CS tutor, student researcher |

## Automated checks completed

- Every HTML page has exactly one `h1`.
- Primary pages have unique titles shorter than 60 characters and unique meta descriptions between 140 and 160 characters.
- Canonicals, Open Graph tags, Twitter card tags, and descriptive headshot alt text are present.
- Every JSON-LD block parses as valid JSON.
- Internal links point to existing local pages.
- Every planned public route returned HTTP 200 from a local static preview.
- `robots.txt`, `sitemap.xml`, `.nojekyll`, `PUBLISH.md`, favicon, and the supplied `yusuf_headshot.jpg` asset are present.
- No `lorem` or `TODO` placeholder text was found in site HTML.
- Visible article-body counts: freight parsing 928 words; local models 925 words; bilingual programming 957 words. Both research summaries are within the requested 300–500-word range.

Run `python /home/user/workspace/validate_seo_site.py` from this workspace to repeat the structural checks.
