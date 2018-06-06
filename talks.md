---
layout: page
title: Tech Talks
permalink: /talks/
---

<div style="display: flex; flex-wrap: wrap; width: 100%">
    {% for talk in site.data.talks %}
        <div style="max-width: 350px; margin: 10px">
            <center>
                <a href="{{ talk.url }}" target="_blank"><h3> {{ talk.title }}</h3></a>
                <img src="{{ talk.img }}" style="width: 75%" /> <br />
                <b>Date:</b> {{talk.date}} <br/>
                <b>Presenter(s):</b> {{talk.presenters}}<br/>
                <b>Location: </b> {{talk.location}}<br/>
                {{ talk.info }}<br/><br/>
                <p><i>{{talk.description}}</i></p> 
            </center>
        </div>
    {% endfor %}
</div>
