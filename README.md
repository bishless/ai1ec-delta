# ai1ec-delta

Flat-ish theme for All-in-One Event Calendar

## Temp idea dump

```twig
{# set categories = event.categories_html #}
{% if categories is not empty %}
	{% for term in categories %}
		{% if event.term.color is empty %}
			<i class="delta-color-swatch ai1ec-fa ai1ec-fa-circle-o {{ term.term_id | raw }}"></i>
		{% else %}
			<i class="delta-color-swatch ai1ec-fa ai1ec-fa-circle {{ term.term_id | raw }}" {{ event.term.color | raw }}></i>
		{% endif %}
	{% endfor %}
{% endif %}
```
