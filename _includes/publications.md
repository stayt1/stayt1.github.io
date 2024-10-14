<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
<div class="pub-row">
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %} 
      <a class="btn btn-sm z-depth-0" style="font-size:12px;">{{ link.notes }}</a>
      {% endif %}
      {% if link.ccfa %} 
      <a class="btn btn-sm z-depth-0" style="font-size:12px;background-color: rgb(255, 204, 204);">CCF-A</a>
      {% endif %}
      {% if link.ccfb %} 
      <a class="btn btn-sm z-depth-0" style="font-size:12px;background-color: rgb(204, 204, 255);">CCF-B</a>
      {% endif %}
      {% if link.ccfc %} 
      <a class="btn btn-sm z-depth-0" style="font-size:12px;background-color: rgb(204, 255, 204);">CCF-C</a>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>
{% endfor %}

</ol>
</div>

