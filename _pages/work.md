---
layout: page
title: Work
permalink: /work/
---

<div class="work-intro">
  Welcome to my Work page!  
  Here I document my ongoing research, projects, collaborations, and progress logs.  
  This space reflects not just my output, but also the process — the growth, the setbacks, and the teamwork that shapes it all. ✨
</div>

<!-- full-width grid ↓ -->
<div class="work-grid">

  <!-- Work Log -->
  <div class="work-block">
    <h3>Work Log</h3>
    <p>My weekly logs tracking effort and reflection.</p>
    {% include section-preview.html category="worklog" limit="3" %}
    <a href="{{ site.baseurl }}/categories/worklog" class="button">More →</a>
  </div>

  <!-- Projects -->
  <div class="work-block">
    <h3>Projects</h3>
    <p>My GitHub repos, code experiments, and personal builds.</p>
    {% include section-preview.html category="projects" limit="3" %}
    <a href="{{ site.baseurl }}/categories/projects" class="button">More →</a>
  </div>

  <!-- Collaborations -->
  <div class="work-block">
    <h3>Collaborations</h3>
    <p>Team efforts, lab mates, and shared experiments.</p>
    {% include section-preview.html category="collaborations" limit="3" %}
    <a href="{{ site.baseurl }}/categories/collaborations" class="button">More →</a>
  </div>

  <!-- Publications -->
  <div class="work-block">
    <h3>Publications</h3>
    <p>One day, this will bloom with my papers 🌸 (coming soon!)</p>
    {% include section-preview.html category="publications" limit="3" %}
    <a href="{{ site.baseurl }}/categories/publications" class="button">More →</a>
  </div>

</div>
