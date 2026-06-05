# Nipa — Editorial Substack-Inspired Site ✍️✨

Welcome to a highly refined, minimalist personal writing space and research archive. This site is inspired by Substack's clean, high-contrast, modern editorial aesthetic.

> **Live Site:** [isratnipa28.github.io](https://isratnipa28.github.io)

---

## 🎨 Design Philosophy & Aesthetic

This website is styled with **zero visual clutter**, prioritizing deep reading and content presentation:
* **Color Palette**: Rich high-contrast near-black text (`#111111`), slate gray secondary details (`#666666`), crisp borders (`1px solid #EAEAEA`), and an organic rust orange branding accent (`#FF5A1F`).
* **Typography**: Beautiful system serif stack (`Georgia, Cambria, serif`) for headings and publication logo, paired with clean, modern system sans-serif (`-apple-system, BlinkMacSystemFont, ...`) for UI elements and reading blocks.
* **Selection Highlight**: Warm organic highlight tint (`#FFF3ED`).
* **Dark Mode**: Compliant custom dark theme utilizing soft, rich off-black surfaces (`#0C0C0C`) to reduce eye strain, strictly avoiding pure black/white contrasts and purple/violet tones.

---

## 🧭 Key Features & Layout Components

| Feature | Detail / Design Specification |
| :--- | :--- |
| **Sticky Navigation Bar** | Global `64px` height header with Serif branding, simple Archive/About text links, and a pill-shaped subscription call-to-action. |
| **Asymmetric Grid** | Homepage Hero section with a split 65% / 35% layout presenting the featured post and a numbered Trending list (`01`, `02`, `03`). |
| **Chronological Feed** | Centered 720px width notes feed including article category tags, descriptive summaries, post like counters, and square thumbnails. |
| **Deep Reading Container** | Single-column reading container restricted to exactly `720px` max-width with `18px` text, `1.8` line-height, and custom left-border blockquotes. |
| **Subscription Breakout** | Inline subscription panel nested inside article flows with minimal inputs and high-contrast solid action buttons. |
| **Reading Progress Bar** | Fixed progress bar indicator at the top matching scroll levels. |
| **Keyboard Navigation** | Core navigation mapping: browse posts with `j`/`k`, and open using `Enter`. |
| **Giscus Comments** | Secure comments via GitHub Discussions, no heavy backend framework. |
| **Adaptive Breakpoints** | Columns stack vertically <768px, and square thumbnail icons hide <480px. |

---

## 📂 Directory Structure

```
├── index.md                 ← Homepage (quote, tasks in YAML metadata)
├── writing.md               ← Writing section archive page (clean layout)
├── philosophy.md            ← Philosophy notes page
├── about.md                 ← About page
├── feed.xml                 ← RSS feed generator
├── _config.yml              ← Jekyll site settings
├── _posts/                  ← Blog posts (YYYY-MM-DD-title.md)
├── _layouts/
│   ├── default.html         ← Base template (header, theme toggle, lightbox)
│   ├── home.html            ← Homepage Asymmetric Grid & Feed template
│   ├── post.html            ← Deep reading article template (categories, newsletter)
│   └── page.html            ← Single-column standard page template
└── assets/
    ├── style.css            ← Vanilla CSS styling with custom CSS variables
    ├── images/              ← Image assets
    └── pdfs/                ← PDF downloads
```

---

## 🚀 Getting Started

### Local Setup & Development

To customize and build this site locally:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/isratnipa28/isratnipa28.github.io.git
   cd isratnipa28.github.io
   ```

2. **Jekyll Deployment**:
   Since the site runs on standard Jekyll configurations, you can build it locally with Ruby:
   ```bash
   bundle install
   bundle exec jekyll serve
   ```

3. **Writing a New Article**:
   Add a markdown file under `_posts/` with the template:
   ```markdown
   ---
   layout: post
   title: "Your Article Title"
   description: "A short, engaging teaser subtitle."
   category: "Research"
   tags: [gis, machine-learning]
   ---
   
   Your content goes here...
   ```

---

## 🛡️ Verification & Performance Audits

We utilize the Antigravity Kit to scan and audit directory performance, accessibility (UX), and code hygiene:
* **UX Audit**: Verifies typography constraints, Fitts' law target sizes, Hick's law complexity boundaries, and contrast ratios.
* **SEO Audit**: Assures heading sequence hierarchy, alt-tag presence, and Open Graph tags.
* **Security Scan**: Checks for dependency vulnerabilities and exposed credentials.

To run the master checks suite:
```bash
python3 .agent/scripts/checklist.py .
```

---

## 📄 License

This theme is licensed under the [MIT License](LICENSE). Feel free to fork, customize, and make it your own!
