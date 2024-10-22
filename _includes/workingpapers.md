<h2 id="publications" style="margin: 2px 0px -15px;">Working Papers</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.workingpapers.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% endif %}
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.journal }}">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
    <div class="links">
      {% if link.wp %} 
      <a href="{{ link.wp }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">working paper</a>
      {% endif %}
      {% if link.bgpe %} 
      <a href="{{ link.bgpe }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">bgpe discussion paper</a>
      {% endif %}
	  {% if link.wifowp %} 
      <a href="{{ link.wifowp }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">wifo discussion paper</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">project page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">bibtex</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>

<br>

{% endfor %}

</ol>
</div>
