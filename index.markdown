---
title: 'Yucatalks'
layout: app
---
<div class="container">
  <div class="mdc-layout-grid">
    <div class="mdc-layout-grid__inner">
      <div class="mdc-layout-grid__cell mdc-layout-grid__cell--span-4">
        <div class="right-align">
          <img src="./assets/images/logo_shadow.svg" class="logo">
        </div>
      </div>
      <div class="mdc-layout-grid__cell mdc-layout-grid__cell--span-8 typewriter-container">
          <div data-controller="typewriter">
              COMING
          </div>
      </div>
    </div>
    </div>
    <div class="mdc-layout-grid">
        <div class="mdc-layout-grid__inner">
            {% for post in site.posts %}
                <div class="mdc-layout-grid__cell mdc-layout-grid__cell--span-4">
                    <div class="mdc-card radius mycard">
                        <div class="mdc-card__content card-padding">
                            <div class="mdc-card__meta">
                                <p class="card-date">{{ post.date | date_to_string }}</p>
                            </div>
                            <article class="mdc-typography--body2">
                                <h2 class="card-title"><a href="{{post.url}}" class="title-link">{{post.title}}</a></h2>
                                <div class="card-overflow card-text">
                                  <p class="card-description-text">{{ post.description }}</p>
                                </div>
                            </article>
                        </div>
                    </div>
                </div>
            {% endfor %}
    </div>
</div>
</div>