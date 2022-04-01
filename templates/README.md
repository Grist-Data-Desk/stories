# Grist-Data-Desk/stories

All {{ count }} of our computational notebooks. Also available as [a CSV file](stories.csv). Thanks to the LA Times [Data Desk](https://github.com/datadesk) for the base!

| date | slug | description |
|:--|:--|:--|{% for obj in object_list %}
|  {{ obj.date }} | [{{ obj.slug }}]({{ obj.url }}) | {{ obj.description }} |{% endfor %}
