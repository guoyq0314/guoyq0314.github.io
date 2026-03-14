## Publications

<div class="publications">
{% for link in site.data.publications.main %}
<div class="pub-row">

  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title"><a href="{{ link.pdf }}" target="_blank">{{ link.title }}</a></div>
    <div class="author">{{ link.authors }}</div>
    <div class="periodical"><em>{{ link.conference }}</em></div>
    <div class="links">
      {% if link.pdf %}
      <a href="{{ link.pdf }}" target="_blank" class="btn btn-sm z-depth-0" role="button" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %}
      <a href="{{ link.code }}" target="_blank" class="btn btn-sm z-depth-0" role="button" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.bibtex %}
      <a href="{{ link.bibtex }}" target="_blank" class="btn btn-sm z-depth-0" role="button" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %}
      <strong><i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
    </div>
  </div>

</div>
{% endfor %}
</div>
