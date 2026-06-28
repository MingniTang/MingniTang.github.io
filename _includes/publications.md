<h1 id="publications"></h1>

<h2 style="margin: 60px 0px 10px;">Publications</h2>

<div class="publications">
<ol class="bibliography">

{% for publication in site.data.publications.main %}

<li>
<div class="pub-row">
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      {% assign publication_link = publication.pdf | default: publication.paper %}
      {% if publication_link %}
      <div class="title"><a href="{{ publication_link }}">{{ publication.title }}</a></div>
      {% else %}
      <div class="title">{{ publication.title }}</div>
      {% endif %}
      <div class="author">{{ publication.authors }}</div>
      <div class="periodical"><em>{{ publication.conference }}</em></div>
    <div class="links">
      {% if publication.pdf %}
      <a href="{{ publication.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% else %}
      <span class="btn btn-sm z-depth-0 disabled" style="font-size:12px;">PDF</span>
      {% endif %}
      {% if publication.paper %}
      <a href="{{ publication.paper }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Paper</a>
      {% else %}
      <span class="btn btn-sm z-depth-0 disabled" style="font-size:12px;">Paper</span>
      {% endif %}
      {% if publication.code %}
      <a href="{{ publication.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% else %}
      <span class="btn btn-sm z-depth-0 disabled" style="font-size:12px;">Code</span>
      {% endif %}
    </div>
  </div>
</div>
</li>
{% endfor %}
</ol>
</div>
