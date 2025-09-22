---
layout: page
title: Getting Started
subtitle: How to fork, configure, and deploy
---

<div class="gs-section-01" markdown="1">

### 1. Fork this project
Fork this project by clicking the __*Fork*__ button at the top right corner of this page. Forking means that you now copied this entire project and all the files into your account.
</div>

<div class="gs-section-02" markdown="1">

### 2. Rename the project to `<yourusername>.github.io`
Click on __*Settings*__ at the top (the cog icon) and on that page you'll have an option to rename the project (*Repository name*). This will create a website with the **Beautiful Jekyll** template that will be available at `https://<yourusername>.github.io` within a couple minutes (check out the [FAQ](https://beautifuljekyll.com/faq/#custom-domain) if you want to use a different project name). If after a few minutes your website is still not ready, try making any edit to any file, just to force GitHub to re-build your site.
</div>

<div class="gs-section-03" markdown="1">

### 3. Customize your website settings
Edit the `_config.yml` file to change any settings you want. To edit the file, click on it to view the file and then click on the pencil icon to edit it (watch the video tutorial above if you're confused). The settings in the file are self-explanatory and there are comments inside the file to help you understand what each setting does. Any line that begins with a hashtag (`#`) is a comment, and the other lines are actual settings.

Note that in the video above only one setting in the `_config.yml` file is edited. **You should actually go through the rest of the settings as well. Don't be lazy, go through all the settings!**
</div>

<div class="gs-section-04" markdown="1">

### 4. Congratulations! You have a website!
After you save your changes to the `_config.yml` file (by clicking on *Commit changes* as the video tutorial shows), your website should be ready in a minute or two at `https://<yourusername>.github.io`. Every time you make a change to any file, your website will get rebuilt and should be updated in about a minute or so. Your website will be initialized with several sample blog posts and a couple other pages.

Note that this was the easy way to *create* your website, but it does come at a cost: when Beautiful Jekyll gains new features in the future, *updating* your website to include all the latest features is cumbersome. See the [FAQ](https://beautifuljekyll.com/faq/#updating) for help with upgrading in the future.
</div>

<!-- Put the style tag at the very bottom of the page -->
<style>
/* === Design tokens (light & dark) === */
:root {
  --bg: #ffffff;
  --fg: #1f2937;         /* slate-800 */
  --muted: #6b7280;      /* gray-500 */
  --card: #ffffff;
  --card-border: #e5e7eb;/* gray-200 */
  --accent: #0ea5e9;     /* sky-500 */
  --accent-600: #0284c7; /* sky-600 */
  --accent-50: #f0f9ff;  /* sky-50 */
  --success: #16a34a;    /* green-600 */
  --shadow: 0 6px 18px rgba(2, 132, 199, 0.08);
}

@media (prefers-color-scheme: dark) {
  :root {
    --bg: #0b1220;
    --fg: #e5e7eb;
    --muted: #9ca3af;
    --card: #0f172a;         /* slate-900 */
    --card-border: #1f2937;  /* slate-800 */
    --accent: #38bdf8;
    --accent-600: #0ea5e9;
    --accent-50: #06263a;
    --success: #22c55e;
    --shadow: 0 8px 20px rgba(56, 189, 248, 0.12);
  }
}

/* === Page container === */
.gs {
  background: var(--bg);
  color: var(--fg);
  display: grid;
  gap: 18px;
}

/* === Step cards === */
.step-card {
  position: relative;
  background: var(--card);
  border: 1px solid var(--card-border);
  border-radius: 14px;
  padding: 18px 18px 16px 18px;
  box-shadow: var(--shadow);
}

.step-card h3 {
  margin: 0 0 8px 0;
  font-size: 1.25rem;
  line-height: 1.25;
  letter-spacing: .2px;
}

.step-card p { margin: 0 0 10px 0; color: var(--fg); }
.step-card code { background: var(--accent-50); padding: 2px 6px; border-radius: 6px; }

/* === Number badge === */
.step-badge {
  position: absolute;
  top: -12px; left: -12px;
  width: 36px; height: 36px;
  display: grid; place-items: center;
  background: var(--accent);
  color: white; font-weight: 700;
  border-radius: 10px;
  box-shadow: 0 4px 10px rgba(2, 132, 199, 0.25);
}

/* === Lists & meta info === */
.checklist { list-style: none; padding-left: 0; margin: 8px 0 0 0; }
.checklist li {
  position: relative; padding-left: 26px; margin: 6px 0; color: var(--fg);
}
.checklist li::before {
  content: "✓";
  position: absolute; left: 0; top: 0;
  color: var(--success); font-weight: 700;
}

.meta { list-style: none; padding-left: 0; margin: 8px 0 0 0; color: var(--muted); }
.meta li { margin: 4px 0; }

/* === Inline notes === */
.note {
  margin-top: 10px;
  padding: 10px 12px;
  background: var(--accent-50);
  border: 1px solid var(--card-border);
  border-left: 4px solid var(--accent-600);
  border-radius: 10px;
  color: var(--fg);
}

/* === Code snippet block (subtle) === */
.snippet {
  background: var(--bg);
  border: 1px dashed var(--card-border);
  border-radius: 10px;
  padding: 10px 12px;
  overflow-x: auto;
  margin: 10px 0 0 0;
}

/* === Nice hover lift for cards (no motion sickness) === */
@media (hover: hover) {
  .step-card { transition: transform .15s ease, box-shadow .15s ease; }
  .step-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 12px 26px rgba(2,132,199,0.10);
  }
}

/* === Tighten default markdown spacing inside .step-card === */
.step-card :is(p, ul, ol, pre, .note, .snippet) + :is(p, ul, ol, pre, .note, .snippet) {
  margin-top: 8px;
}
</style>

