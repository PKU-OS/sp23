---
layout: page
title: Schedule
nav_order: 1
currWeekNumber: 1
---

# {{ site.tagline }}
{: .mb-2 }
Peking University, 2023 Spring
{: .mb-0 .fs-6 .text-grey-dk-000 }

<img src="/sp23/assets/images/pkuos.svg">

<p>
<a href="https://pkuflyingpig.gitbook.io/pintos/" class="btn btn-purple">Project Gitbook</a>
<a href="https://course.pku.edu.cn" class="btn btn-green">PKU Course Website</a>
<a href="https://piazza.com/pku.edu.cn/spring2023/04834490" class="btn btn-blue">Piazza</a>
</p>

{% if site.announcements %}
{{ site.announcements.last }}
[Previous Announcements](announcements.md){: .btn .btn-outline .fs-3 }
{% endif %}

## Schedule
{% for module in site.modules %}
<a name="week-{{module.weekNumber}}"></a>
{{ module }}
{% endfor %}
