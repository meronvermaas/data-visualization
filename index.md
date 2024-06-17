---
title: Home
---

# A short Practical guide to Data Visualization!

{% include figure.html img="datavisualizationhandbook_cover.png" alt="intro image here" caption="from 'a short Data Visualiztion Handbook by Iraklis Vretzakis'" width="75%" %}

*Programming beginners in R ans/or Python will be empowered to harness basic data analysis tools essential for Neuroscientific research and beyond. We will provide basic practical insights and hands-on experience to enhance your research analysis capabilities. Don't miss this opportunity to enhance your skill set and network with fellow enthusiasts.*

<div class="toc" markdown="1">
## Contents:

{% for lesson in site.pages %}
{% if lesson.nav == true %}- [{{ lesson.title }}]({{ lesson.url | relative_url }}){% endif %}
{% endfor %}
</div>

Hosted by [Vrije Universiteit Amsterdam](http://www.vu.nl/), {{ site.pub_year }}.
 
> built using [Jekyll](https://jekyllrb.com/) and [GitHub Pages](https://pages.github.com/)
>
> images and content: cc-by-sa <a href="https://github.com/{{ site.github_username }}">{{ site.author }}</a> {{ site.pub_year}} (get [source code]({{ site.repo }})).
> Last build date: {{ site.time | date: "%Y-%m-%d" }}.
>
> <a href="http://creativecommons.org/licenses/by-sa/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" alt="Creative Commons License" /></a>
