# Project Structure

```
amazon-prime-eda-project/
|
|-- data/
|   |-- titles.csv              # Core content metadata (9,871 rows)
|   |-- credits.csv             # Cast and crew information (124,235 rows)
|
|-- notebooks/
|   |-- amazon_prime_eda.ipynb              # Main EDA notebook (executed with outputs)
|
|-- images/
|   |-- content_growth_timeline.png
|   |-- country_treemap.png
|   |-- genre_decade_heatmap.png
|   |-- genre_distribution.png
|   |-- genre_growth.png
|   |-- missing_values_bar.png
|   |-- missing_values_heatmap.png
|   |-- movie_vs_tv.png
|   |-- top_countries.png
|   |-- top_directors.png
|   |-- correlation_heatmap.png
|   |-- missing_correlation.png
|
|-- interactive_charts/             # Plotly charts as HTML (open locally)
|   |-- content_growth_timeline.html
|   |-- movie_vs_tv.html
|   |-- top_countries.html
|   |-- genre_distribution.html
|   |-- genre_growth.html
|   |-- top_directors.html
|   |-- top_actors.html
|   |-- rating_distribution.html
|   |-- runtime_by_genre.html
|   |-- country_genre_sunburst.html
|
|
|-- README.md
|-- LICENSE
|-- .gitignore
|-- requirements.txt
|-- environment.yml
|-- CHANGELOG.md
|-- CONTRIBUTING.md
|-- project_structure.md
|-- dataset_description.md
|-- business_questions.md
```
