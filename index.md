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
    <li data-target="#carousel-example-generic" data-slide-to="0" class="active"></li>
    <li data-target="#carousel-example-generic" data-slide-to="1" class=""></li>
    <li data-target="#carousel-example-generic" data-slide-to="2" class=""></li>
  </ol>
  <div class="carousel-inner" role="listbox">
    <div class="item active">
      <div class="fill" style="background-image:url('{{ HOME_PATH }}assets/images/carousel1.jpg'); background-position:center;">
        <div class="carousel-caption">
          <p lingdex="133"> Not First slide description</p>
        </div>
      </div>
    </div>
    <div class="item">
      <div class="fill" style="background-image:url('{{ HOME_PATH }}assets/images/carousel2.jpg');">
      <div class="carousel-caption">
        <p lingdex="133">Second slide description</p>
      </div>
      </div>
    </div>
    <div class="item">
      <div class="fill" style="background-image:url('{{ HOME_PATH }}assets/images/carousel3.jpg');">
      <div class="carousel-caption">
        <p lingdex="133">Third slide description</p>
      </div>
      </div>
    </div>
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
        <div class="col-sm-4">
          {% for qingmei in site.tags.qingmei %}
            {% if qingmei.language == page.language %}
              {% assign theurl = qingmei.url %}
            {% endif %}
          {% endfor %}
          <img class="img-circle" src="{{ HOME_PATH }}assets/images/head1.jpeg" alt="Generic placeholder image" style="width: 140px; height: 140px;">
          <h2>Qingmei Zhou</h2>
          <p><strong>Artistic Director and Head of Group</strong></p>
          <p><a class="btn btn-default" href="{{theurl}}" role="button">View details &raquo;</a></p>
        </div><!-- /.col-md-4 -->

        <div class="col-sm-4">
          {% for huijun in site.tags.huijun %}
            {% if huijun.language == page.language %}
              {% assign theurl = huijun.url %}
            {% endif %}
          {% endfor %}
          <img class="img-circle" src="{{ HOME_PATH }}assets/images/home/GengHuijun.jpg" alt="Generic placeholder image" style="width: 140px; height: 140px;">
          <h2>Huijun Geng</h2>
          <p><strong>Honorary Artistic Director/Choreographer</strong></p>
          <p><a class="btn btn-default" href="{{theurl}}" role="button">View details &raquo;</a></p>
        </div><!-- /.col-md-4 -->
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
        <img class="featurette-image img-responsive" src="{{ HOME_PATH }}assets/images/feature2.jpg" alt="Generic placeholder image">
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

