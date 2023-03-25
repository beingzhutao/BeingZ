

```
## contact
`<div class="row g-5 mb-5">
  <div>
    <h3 class="fw-bold border-bottom pb-3 mb-5">Contact</h3>
    {% for contact in site.data.settings.contacts %}
    <div class="row g-5 mb-5">
      <div class="col-md-8">
        <h4>{{ contact.name }}</h4>
        <p>Email: {{ contact.email }}</p>
        <p>Department: {{ contact.department }}</p>
        <p>Institution: {{ contact.institution }}</p>
      </div>
      <div class="col-md-4">
        <img src="{{ site.github.url }}/{{ contact.image }}" alt="Contact" width="50%">
      </div>
    </div>
    {% endfor %}
  </div>
</div> `



## include publications.html
<div class="row g-5 mb-5">
  <div>
    <h3 class="fw-bold border-bottom pb-3 mb-5">Publications</h3>
    {% if page.title == "Home" %}
      {% for item in site.data.publications.featured %}
        <p><a href="{{ item.url }}">{{ item.name }}</a></p>
      {% endfor %}
    {% else %}
      {% for item in site.data.publications.index %}
        <p><a href="{{ item.url }}">{{ item.name }}</a></p>
      {% endfor %}
    {% endif %}
  </div>
</div>




```