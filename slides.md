---
# try also 'default' to start simple
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /images/warren-young-adult.jpg
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# persist drawings in exports and build
drawings:
  persist: false
# page transition
# transition: slide-left
# use UnoCSS
css: unocss
---

# 🔥 Potsie v2 💥


Learning Analytics Charts That Rock! 🤘

<logos-twitter /> [@quitterie_lcs](https://twitter.com/quitterie_lcs) // <logos-mastodon-icon /> [@jmaupetit](https://mamot.fr/@jmaupetit) // <logos-twitter /> [@open_fun](https://twitter.com/open_fun)


---
layout: statement
---
## Disclaimer

> Presented product is still POC. We are still experimenting on it. Our intend
> here is to give you a sneak peek of what it could be and get early-stage
> feedback.

<style>
blockquote {
  margin: 4rem;
  padding: 1rem;
}
blockquote p {
  font-size: 1.5rem;
  line-height: 2.5rem;
}
</style>

---
layout: image-right
image: /images/potsie-screenshot.jpg
---

# Potsie

Grafana dashboards suite for learning analytics.

<br/>
<br/>

Potsie is a collaborative insightful distribution of dashboards for Grafana
from xAPI statements in an Elasticsearch data lake.

<br/>
<br/>

<logos-github-icon /> https://github.com/openfun/potsie

<style>
img {
  margin: 2rem;
}
</style>

---
layout: image-right
image: /images/warren-middle-age.jpg
transition: fade
src: sections/limits-potsie.md
---

---
layout: two-cols
src: sections/origin-warren.md
---

---
layout: section
---

## Sneak peek

---
layout: full
src: sections/sneak-peek.md
---

---
layout: full
---

## `DailyViews` component in action!

![](/images/warren-sneak-peek.gif)


---
layout: full
---

# Check this out!

<div class="grid grid-cols-2 gap-4 credits">
  <div class="grid grid-cols-2 gap-4">
    <div>
      <a href="https://openfun.github.io/2023-openedx-con-warren/">
        Slides
      </a>
      <br/>
      <img src="/images/qr-code-slides.png" />
    </div>
    <div>
      <logos-github-icon />
      <a href="https://github.com/openfun/warren">
        openfun/warren
      </a>
      <img src="/images/qr-code-project.png" />
    </div>
  </div>
  <div>
      <img class="logo" src="/images/logo-openfun.png"  width="200" />
      <br />
      <img class="logo" src="/images/logos-finance.png" />
  </div>
</div>

<style>
.credits {
  margin-top: 5rem;
  text-align: center;
}
.logo {
  display: block;
  margin: 1rem auto;
}
</style>

