<h1 id="publications"></h1>

<h2 style="margin: 60px 0px 10px;">Publications</h2>

<div class="publications">
<ol class="bibliography">

{% for publication in site.data.publications.main %}

<li>
<div class="pub-row">
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="citation">{{ publication.citation }}</div>
      {% if publication.status %}
      <div class="periodical"><em>{{ publication.status }}</em></div>
      {% endif %}
    {% if publication.pdf or publication.anthology or publication.arxiv or publication.code or publication.dataset %}
    <div class="links">
      {% if publication.pdf %}
      <a href="{{ publication.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if publication.anthology %}
      <a href="{{ publication.anthology }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Anthology</a>
      {% endif %}
      {% if publication.arxiv %}
      <a href="{{ publication.arxiv }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">arXiv</a>
      {% endif %}
      {% if publication.code %}
      <a href="{{ publication.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if publication.dataset %}
      <a href="{{ publication.dataset }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Dataset</a>
      {% endif %}
    </div>
    {% endif %}
  </div>
</div>
</li>
{% endfor %}
</ol>
</div>
