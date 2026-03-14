## Publications

<style>
.pub-item {
  margin-bottom: 16px;
  padding-left: 16px;
  border-left: 3px solid #4a90d9;
  line-height: 1.6;
}
.pub-title {
  font-weight: bold;
  color: inherit;
  text-decoration: none !important;
}
.pub-authors {
  color: #555;
  font-size: 0.95em;
}
.pub-journal {
  font-style: italic;
  color: #444;
  font-size: 0.95em;
}
.pub-links a {
  font-size: 0.85em;
  margin-right: 6px;
  color: #4a90d9;
}
.pub-notes {
  font-size: 0.85em;
  color: #e74d3c;
  font-weight: bold;
}
</style>

{% for link in site.data.publications.main %}
<div class="pub-item">
  <div class="pub-title">{{ link.title }}</div>
  <div class="pub-authors">{{ link.authors }}</div>
  <div class="pub-journal">{{ link.conference }}</div>
  <div class="pub-links">
    {% if link.pdf %}<a href="{{ link.pdf }}" target="_blank">[PDF]</a>{% endif %}
    {% if link.code %}<a href="{{ link.code }}" target="_blank">[Code]</a>{% endif %}
    {% if link.bibtex %}<a href="{{ link.bibtex }}" target="_blank">[BibTeX]</a>{% endif %}
    {% if link.notes %}<span class="pub-notes">{{ link.notes }}</span>{% endif %}
  </div>
</div>
{% endfor %}
