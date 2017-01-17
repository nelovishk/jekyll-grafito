---
layout: default
---
<div class="row main home">
  <div class="col-md-6 content">{{content}}</div>
  <div class="col-md-6 sidebar right">
    <ul class="collections-list">
      {% for collection in site.collections %}
        {% if collection.grafito %}
          <li class="collection">
            <a href="/{{collection.label}}/index.html">

              {% if collection.name %}
                {{ collection.name }}
              {% else %}
                {{ collection.label }}
              {% endif %}
            </a>

            <ul class="collection-items">
            {% for doc in collection.docs %}
              <li><a href="{{doc.url}}">
              {% if doc.name %}
                {{doc.name}}
              {% else %}
                {{doc.title}}
              {% endif %}
              </a></li>
            {% endfor %}
            </ul>
          </li>
        {% endif %}
      {% endfor %}
    </ul>
  </div>
</div>
