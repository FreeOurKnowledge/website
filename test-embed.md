---
layout: post
title: Mapping the Publishing Deadlock
subtitle: A survey of the barriers reported by stakeholders in scholarly publishing
gh-repo: freeourknowledge/community
cover-img: /assets/img/stakeholder-blank-2.png
thumbnail-img: /assets/img/stakeholder-fill.png
share-img: /assets/img/stakeholder-fill.png
twitter-img: "https://github.com/FreeOurKnowledge/website/blob/master/assets/img/stakeholder-fill.png?raw=true"
twitter-card: "https://github.com/FreeOurKnowledge/website/blob/master/assets/img/stakeholder-fill.png?raw=true"
comments: true
permalink: /test-embed/
sitemap: false
---

## The survey:

Free Our Knowledge campaigns have historically asked you to take action and be part of a collective effort to enact change, but in this one, we want to hear your perspective about why that might not be possible.

When it comes to making the scholarly publishing system more fair and open, there are many perceived obstacles that are mentioned as reasons why individuals won't take action on their own. Every stakeholder group in scholarly publishing can explain why the move has to come from someone else. We want to find out whether that's true.

We're mapping scholarly publishing as a set of relationships between the groups that make it up: who each group sees as the obstacle, what holds them back, and what they believe they could actually do. 

The survey is five open questions, each answerable in a few sentences, and takes under ten minutes. 

If you work on the publisher, funder, university administration, or infrastructure side — or know someone who does, we are especially interested in these perspectives, as variety will make or break the results. Scepticism is also welcome: dissenting opinions are all the more valuable for a complete picture. 

#### Complete the survey here:

[Open Science Stakeholders Survey — Hosted by Radboud University](https://questions.socsci.ru.nl/index.php/942866?lang=en)

## The stakeholder map

Once you've completed the survey, feel free to examine the interactive stakeholder map below, which maps the relationships between stakeholders in scholarly publishing. Hovering over the edges between nodes provides a description of the influence between one group and another, including financial, organizational, technical and reputational. Clicking on any node provides more detailed information.

The responses from the survey will be mapped along this structure, and the results are planned to be presented at the [Open Science Festival in Delft, 14 October 2026](https://opensciencefestival.nl).


<div class="graph-embed">
  <iframe src="https://ltk1.github.io/open-science-graph/?embed=1" style="position:absolute;inset:0;width:100%;height:100%;border:0"></iframe>
</div>

<script>
(function () {
  var ALLOWED = ['https://ltk1.github.io'];
  (function () {
    var wrap = document.querySelector('.graph-embed');
    window.addEventListener('message', function (e) {
      if (ALLOWED.indexOf(e.origin) === -1) return;
      if (!e.data || e.data.type !== 'osg-expand') return;
      wrap.classList.toggle('expanded', !!e.data.expanded);
      if (e.data.expanded) wrap.scrollIntoView({ behavior: 'smooth', block: 'center' });
    });
  })();
  var wrap = document.querySelector('.graph-embed');
  window.addEventListener('message', function (e) {
    if (ALLOWED.indexOf(e.origin) === -1) return;
    if (e.origin !== 'https://ltk1.github.io') return;
    if (!e.data || e.data.type !== 'osg-expand') return;
    wrap.classList.toggle('expanded', !!e.data.expanded);
    if (e.data.expanded) wrap.scrollIntoView({ behavior: 'smooth', block: 'center' });
  });
})();
</script>

<style>
.graph-embed { position: relative; width: 100%; height: min(70vh, 620px); margin: 1.5rem 0; transition: height .35s ease; }
.graph-embed.expanded {
  height: min(78vh, 700px);
  width: min(150%, 96vw);
  position: relative;
  left: 50%;
  transform: translateX(-50%);
}
.graph-embed iframe { position: absolute; inset: 0; width: 100%; height: 100%; border: 0; border-radius: 6px; }
body { font-family: sans-serif; margin: 2rem auto; max-width: 800px; }
</style>