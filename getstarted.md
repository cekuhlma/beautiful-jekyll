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
/* Shared base styles */
[class^="gs-section-"] {
  background: #ffffff;
  border: 1px solid #e5e7eb; /* light gray */
  border-radius: 10px;
  padding: 16px 20px;
  margin: 18px 0;
  box-shadow: 0 4px 10px rgba(0,0,0,0.05);
}

/* Headings */
[class^="gs-section-"] h3 {
  margin-top: 0;
  font-size: 1.3rem;
  font-weight: 600;
}

/* Paragraphs */
[class^="gs-section-"] p {
  line-height: 1.6;
  margin-bottom: 0.6em;
}

/* Step-specific accents */
.gs-section-01 {
  border-left: 5px solid #ef4444; /* red */
}
.gs-section-01 h3 { color: #b91c1c; }

.gs-section-02 {
  border-left: 5px solid #2563eb; /* blue */
}
.gs-section-02 h3 { color: #1e3a8a; }

.gs-section-03 {
  border-left: 5px solid #16a34a; /* green */
}
.gs-section-03 h3 { color: #166534; }

.gs-section-04 {
  border-left: 5px solid #9333ea; /* purple */
}
.gs-section-04 h3 { color: #581c87; }

/* Optional: subtle hover lift */
[class^="gs-section-"]:hover {
  transform: translateY(-2px);
  transition: transform .15s ease, box-shadow .15s ease;
  box-shadow: 0 8px 18px rgba(0,0,0,0.08);
}
</style>


