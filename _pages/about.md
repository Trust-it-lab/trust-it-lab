---
permalink: /
title: "Trust-It Lab - Purdue University Northwest"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

<!-- EDIT ME: the biography shown on the home page. -->

Shafkat is a tenure-track assistant professor and the PI of the **Trustworthy, Robust & Secure Intelligent Systems (Trust-It) lab** in the computer science department at **Purdue University Northwest**. He is also affiliated with **Purdue CERIAS**. He completed his PhD in Computer Science from Purdue University West Lafayette. He is broadly interested in **AI, cybersecurity, and edge security**. His research focuses on developing robust and trustworthy AI agents and safeguarding critical infrastructures/systems when AI agents are integrated into traditional systems.

His research outcomes have been published in high-impact venues such as IEEE Intelligent Systems, IEEE Transactions on Artificial Intelligence, IEEE Internet of Things Journal, IEEE Transactions on Industrial Informatics, IEEE Network, IEEE WoWMoM, IEEE LCN, IEEE ISGT NA, etc. He has led the preparation of multiple grant proposals for leading funding agencies. He was awarded the **Purdue Employee Merit Recognition Award** in 2024 and recognized as an **excellent reviewer by the IEEE Communications Society** in 2023.

News
======

{% comment %}
  News items come from the /_news/ folder (newest first) - see /_news/README.md.
  The same items also appear on the /news/ page.
{% endcomment %}

{% assign news_items = site.news | sort: "date" | reverse %}
{% if news_items.size == 0 %}
<p>No news yet.</p>
{% else %}
<ul class="news-list">
{% for item in news_items %}
  <li><span class="news-list__date">[{{ item.date | date: "%Y/%-m" }}]</span> {{ item.content | markdownify | remove: "<p>" | remove: "</p>" | strip }}</li>
{% endfor %}
</ul>
{% endif %}
