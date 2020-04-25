---
layout: default
folder: /content/5resources/
title: Transformaction
---

## Main article

<p class="update">This needs a huge update. In the meantime something on the building of this website.</p>

## A more robust GitHub Pages development path

GitHub Pages (GHP) is a seemingly attractive package for someone who wants a simple blog site. Create an account, choose a theme (I chose Cayman), start writing content directly on GitHub. OK the GitHub "editor" is somewhat primitive, but it will do. In any case the ability to edit the site from various devices is useful.

That's the route I took, but then things got gradually difficult.

**Frequent updates** were potentially problematic. My site had around 10 pages of initial content and required significant hundreds of updates over a few weeks: generally pure content with hundreds of GitHub deploys. Leaving aside any GHP limits on frequent updating, I longed for the old days; an offline editor and previewing facility.

**A simple approach to managing offline content offline** was only partially successful. Using GitHub desktop initially seemed to do the trick. After a simple cloning of a depository to the desktop the file structure appeared in the Windows Explorer: I could manage items trick items such as images simply by putting them in the appropriate folder and "pushing" them up to my repository.

**Offline development: take 1.** I had in fact already got hold of Visual Studio Code and was using to edit my site offline, pushing up to the web as required. VS Code can be used to get a partial preview, but this is not perfect. I took advice from someone smarter than me: no, I needed proper offline development, with a server to preview.

**Offline development: the crisis.** Reading up, I installed Ruby and Jekyll, the static site manager behind GHP. I got used to using the Terminal functionality within VS Code to launch my site. But what was going on? My offline site looked nothing like my online site. Online was pretty, but offline all the menus and styling had disappeared. Worse, looking behing the scenes the pages weren't even valid HTML: all information before the content &mdash; DOCTYPE, headers etc &mdash; was missing. Worse, the Cayman theme was not incomptabile with the latest version of Jekyll. Ouch.

**The rescue.** Not for the first time my son weighed in, developing his [Blank Jekyll Site](https://github.com/BenjaminEHowe/jekyll-blank/blob/master/README.md) &mdash; not bad as he had never used GHP or Jekyll before! This delivered a GHP website I could copy and download. It had no third-party theming, beyond simple and visible use of HTML, CSS and Jekyll's liquid.

This site was syntactically valid, online and offline and could be previewed.

**Final pieces to the jigsaw.** The final pieces required real care. While the site was entirey valid it had none of the content I wanted and the styling was completly missing. Here's what I did, step by step.

1. **Bring in a new home page.** This was a test that things wouldn't break and that the offline previews worked as expected. It did. I needed to include <code>layout: default</code> in the front matter.

1. **Create new stylesheets.** These were main.css and newstyles.css. I first looked at the online version of my site. I could see that the Cayman theme had stored the final version of the CSS in the stylesheet <code>/assets/css/style.css?v=5be31a03258f445a6a97192a32d60e88e13b0784</code>. The stylesheet was minified, so I used an online CSS prettifier. It contained:

+ Standard CSS: normalize.css v3.0.2 and Cayman tailoring. I copied this into main.css.
+ After this, my own tweaks to the CSS. I copied this into newstyles.css.

1. **Update the default layout.** in <code>/_layouts/default.html</code>. I changed this to refer to the main.css and newstyles.css. Previewing confirmed that things seemed to be working.

1. **Update the navigation.** There were three parts to this:

+ Import the <code>/_data/lists.yml</code> file &mdash; the named navigation parts
+ Import the <code>/_includes/navigation.html</code> file &mdash; the looping liquid
+ Do a liquid-based include in the <code>/_layouts/default.html</code> file

1. **Update the remaining content.** This was a copy/paste of five folders, not forgetting to do the <code>layout: default</code> updates in the front matter.

Here's the old stuff.{: .update}

**Build, improve, optimize** is more than a strapline: I have specific tools and techniques, covering reinsurance, underwriting, distribution, assumptions, price and profit - helping you to thrive.

But here's the problem. What I can't say.

Therefore ... rationale for writing articles and their content.
{: .update}

## Professional articles

+ **Events, dear boy, events:** how Excel can have your back.
+ **Tables:** data analysis.

## Personal articles

+ **Optimizing a classical music collection:** MP3s across multiple devices.

## Working together

**Transformaction** is an actuarial consultancy with deep experience of price competitive markets and particular expertise in the insurance protection sector. Founder [Andrew Howe](https://www.linkedin.com/in/maverickactuary/) has worked with market leaders and challengers: IFA market insurers, aggregator brands and Friendly Societies.

### You may be:

+ **An insurer facing strategic or competitive challenges.** I have the expertise and toolkit, developed over many years, to help you to enter markets, develop products and maximize profits, by trading off prices, volume and much more.
+ **An insurer short of actuarial resources.** Perhaps you require support with product development, analytics, pricing or market entry. I can help, advising **and** delivering.
+ **A reinsurer.** I can fill a technical or operational gap for your actual or potential client, supplying expertise in the areas of experience investigations, distributor analytics and pricing, for example. This enables you to focus on your core business, while effectively providing the support that your actual or potential client needs.

### How we might work together:

+ **Create and review your options:** simple evidence-based analyses and recommendations.
+ **Collaborate deeply:** from strategic engagement with CEOs right through to operational work.
+ **Deliver faster than you imagine:** I can be as “hands-on” as you wish at delivery stage.

### Typical projects:

+ **Capability review.** Ensuring your pricing and analytics team and processes are 2020s-fit.
+ **Pricing and analytics.** I can supply bench strength, as a one-off or on an ongoing basis.
+ **Product development and market entry.** I can work with you, with focus and at pace.

### To do
Generate a google sitemap.
