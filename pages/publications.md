---
layout              : default
show_meta           : false
title               : "Publications at BIG"
subheadline         : ""
teaser              : ""
header: no
permalink           : "/publications/"

---

{% assign publications = site.publications | sort: "year" | reverse %}


<div class="row" style="margin-top: 3rem">
    <h1>{{ page.title }}</h1>
</div>


<div>
    {% for pub in publications %}
    <div class="row" style="margin-bottom: 2rem;">
        <div class="medium-4 small-8 columns">
            <img src="{{ pub.image }}" class="pub-image" />
        </div>
        <div class="medium-8 columns">
            <h4>{{ pub.title }}</h4>
            <div>{{ pub.publication_abbrv }}</div>
            <div>{{ pub.authors }}</div>
            <div>
                {% if pub.paper_url %}
                    <a href="{{pub.paper_url}}" target="_blank" class="paper-link">
                        Paper
                    </a>
                {% endif %}
                {% if pub.website %}
                    |
                    <a href="{{pub.website}}" target="_blank" class="paper-link">
                        Project
                    </a>
                {% endif %}
                {% if pub.colab %}
                    |
                    <a href="{{pub.colab}}" target="_blank">
                        <img src="{{site.urlimg}}colab.png" style="height:2rem" />
                    </a>
                {% endif %}
                {% if pub.github %}
                    |
                    <a href="{{pub.github}}" target="_blank">
                        <img src="{{site.urlimg}}github.png" style="height:1.5rem" />
                    </a>
                {% endif %}
                {% if pub.demo %}
                    |
                    <a href="{{pub.demo}}" target="_blank" class="paper-link">
                        Demo
                    </a>
                {% endif %}
                {% if pub.video %}
                    |
                    <a href="{{pub.video}}" target="_blank" class="paper-link">
                        Video
                    </a>
                {% endif %}
                {% if pub.presentation %}
                    |
                    <a href="{{pub.presentation}}" target="_blank" class="paper-link">
                        Presentation
                    </a>
                {% endif %}
                {% if pub.twitter %}
                    |
                    <a href="{{pub.twitter}}" target="_blank">
                        <img src="{{site.urlimg}}twitter.ico" style="height:1.5rem" />
                    </a>
                {% endif %}
            </div>
        </div>
    </div>
    {% endfor %}
</div>