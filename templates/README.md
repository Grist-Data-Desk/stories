# Grist-Data-Desk/stories

All {{ count }} of the data-driven stories we've open-sourced. Also available as [a CSV file](stories.csv). Thanks to the LA Times [Data Desk](https://github.com/datadesk) for the base!

| date | description | story | repo |
|:--|:--|:--|{% for obj in object_list %}
|  {{ obj.date }} | {{ obj.description }} | [📝]({{ obj.storyUrl }}) | [💻]({{ obj.repoUrl }}) |{% endfor %}
