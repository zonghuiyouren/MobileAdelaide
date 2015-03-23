---
layout: page
title: Dynamism Dance | Home
tagline: Supporting tagline
---
{% include JB/setup %}


<style>
  body {
    background-image: url('/assets/images/background_home.jpg');
    background-position: center;
    background-attachment: fixed;
  }
</style>

<!-- Example row of columns -->
<div id="carousel-example-generic" class="carousel slide" data-ride="carousel">
  <ol class="carousel-indicators">
    {% for carousel in site.tags.carousel %}
      {% if carousel.language == page.language %}
        <li data-target="#carousel-example-generic" data-slide-to="{{forloop.index0 | divided_by: 2}}" class="{{carousel.tags[1]}}"></li>
      {% endif %}
    {% endfor %}
  </ol>
  <div class="carousel-inner" role="listbox">
    {% for carousel in site.tags.carousel %}
      {% if carousel.language == page.language %}
        <div class="item {{carousel.tags[1]}}">
          <div class="fill" style="background-image:url('{{ HOME_PATH }}assets/images/carousel/{{carousel.image}}');">
            <div class="carousel-caption">
              <h3>{{carousel.title}}</h3>
              <p lingdex="133">{{carousel.description}}</p>
            </div>
          </div>
        </div>
      {% endif %}
    {% endfor %}
  </div>
  <a class="left carousel-control" href="#carousel-example-generic" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel-example-generic" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>




<!-- Marketing messaging and featurettes
================================================== -->
<!-- Wrap the rest of the page in another container to center all the content. -->

<div class="container-fluid marketing">
  <!-- Three columns of text below the carousel -->
  <div class="container-fluid" style="background-color:rgba(255,255,255,0.8); padding-top: 60px;">
    <div class="container" >
      <div class="row">
          {% for vip in site.tags.vip %}
            {% if vip.language == page.language %}
              <div class="col-sm-4">
                <img class="img-circle" src="{{ HOME_PATH }}assets/images/home/{{vip.image}}" alt="{{vip.title}}" style="width: 140px; height: 140px;">
                <h2>{{vip.title}}</h2>
                <p><strong>{{vip.position}}</strong></p>
                <p>{{vip.description}}</p>
                <p><a class="btn btn-default" href="{{vip.url}}" role="button">View details &raquo;</a></p>
              </div><!-- /.col-md-4 -->
            {% endif %}
          {% endfor %}

      </div><!-- /.row -->
    </div> <!-- /.container -->
  </div>

  <hr class="featurette-divider">

  <!-- START THE FEATURETTES -->
  <div class="row featurette" style="background-color:#f6f6f6">
    <div class="container">
      <div class="col-md-6">
        {% for mei in site.tags.meigroup %}
          {% if mei.language == page.language %}
            {% assign theurl = mei.url %}
          {% endif %}
        {% endfor %}
        <h2 class="featurette-heading">The Mei's Dance Group</h2>
        <p class="lead">The Mei's Dance Group is South Australia's first dance group to combine eastern and western cultural elements, incorporating Chinese flavours upon the original framework of Mei's Dance Company, founded in February 2014 after a long effort owing to the enthusiasm of head of company Qingmei Zhou.</p>
        <p><a class="btn btn-default" href="{{theurl}}" role="button">View details &raquo;</a></p>
      </div>
      <div class="col-md-6">
        <img class="featurette-image img-responsive" src="{{ HOME_PATH }}assets/images/home/mei.png" alt="Generic placeholder image">
      </div>
    </div>
  </div>



  <hr class="featurette-divider">
  <div class="row featurette">
    <div class="container" style="height:300px;">
      <div class="row">
        <div class="col-md-3 pull-right">
          <img src="/assets/images/logo_red.png" alt="" class="img-cicle" style="width:150px;height:150px;">
        </div>
      </div>
    </div>
  </div>



  <div class="row featurette" style="background-color:#f6f6f6">
    <div class="container" style="padding-bottom: 20px;">
      <!-- the limit here should be the double number of the news you want to post on the home page -->
      {% for news in site.tags.news limit:6 %}
        {% if page.language == news.language %}
          <div class="col-md-4" style="padding-top: 20px;">
            <article class="box style">
              <a href="{{news.url}}" class="image featured"><img src="/assets/images/news/{{news.image}}" alt=""></a>
              <h3><a href="{{news.url}}">{{news.title}}</a></h3>
              <p>{{news.description}}</p>
            </article>
          </div>
        {% endif %}
      {% endfor %}
    </div>
  </div> 


  <div class="row featurette" style="background-color:rgba(255,255,255,0.8);">
    <div class="container" style="height:300px; text-align: center;">
        <h2>SPONSORS</h2>
        <div class="row sponsor-container">
          {% for sponsor in site.tags.sponsor %}
          {% if sponsor.language == page.language %}
            <div class="col-md-6">
              <a href="{{sponsor.website}}">
                <img class="img-thumbnail sponsor-height" src="/assets/images/sponsors/{{sponsor.image}}" alt="{{sponsor.title}}">
                <p>{{sponsor.description}}</p>
              </a>
            </div>
          {% endif %}
          {% endfor %}
        </div>
    </div>
  </div>

<!--   <div class="row featurette" style="background-color:#f6f6f6">
    <div class="container">
      <h2 class="featurette-heading" style="text-align: center; font-size: 60px; margin-top: 30px; margin-bottom: 50px;">Choose your favorite class<span class="text-muted"></span></h2>
      {% for dance in site.dances %} 
        <div class="col-sm-4 col-md-2">
          <img  class="homeclasses img-circle"  style="background-color: #f1a7b7">
          <span class="text-class"><span>{{dance}}</span></span>
        </div>
      {% endfor %}
    </div>
  </div> -->

</div>
<!-- /END THE FEATURETTES -->

