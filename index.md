---
layout: page
title: Dynamism Dance | Home
tagline: Supporting tagline
---
{% include JB/setup %}


<!-- Example row of columns -->
<div id="carousel-example-generic" class="carousel slide" data-ride="carousel">
  <ol class="carousel-indicators">
    <li data-target="#carousel-example-generic" data-slide-to="0" class="active"></li>
    <li data-target="#carousel-example-generic" data-slide-to="1" class=""></li>
    <li data-target="#carousel-example-generic" data-slide-to="2" class=""></li>
  </ol>
  <div class="carousel-inner" role="listbox">
    <div class="item active" style="background-image: url('{{ HOME_PATH }}assets/images/carousel1.jpg'); background-size: cover; background-repeat:no-repeat; background-position: top; background-attachment: fixed;">
      <div class="carousel-caption">
        <p lingdex="133">Cras justo odio, dapibus ac facilisis in, egestas eget quam. Donec id elit non mi porta gravida at eget metus. Nullam id dolor id nibh ultricies vehicula ut id elit.</p>
      </div>
    </div>
    <div class="item" style="background-image: url('{{ HOME_PATH }}assets/images/carousel2.jpg'); background-size: cover; background-position: center; background-attachment: fixed;">
      <div class="carousel-caption">
        <p lingdex="133">Cras justo odio, dapibus ac facilisis in, egestas eget quam. Donec id elit non mi porta gravida at eget metus. Nullam id dolor id nibh ultricies vehicula ut id elit.</p>
      </div>
    </div>
    <div class="item" style="background-image: url('{{ HOME_PATH }}assets/images/carousel3.jpg'); background-size: cover; background-position: center; background-attachment: fixed;">
      <div class="carousel-caption">
        <p lingdex="133">Cras justo odio, dapibus ac facilisis in, egestas eget quam. Donec id elit non mi porta gravida at eget metus. Nullam id dolor id nibh ultricies vehicula ut id elit.</p>
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
  <div class="container-fluid" >
    <div class="container" >
      <div class="row">
        <div class="col-lg-4">
          <img class="img-circle" src="{{ HOME_PATH }}assets/images/head1.jpeg" alt="Generic placeholder image" style="width: 140px; height: 140px;">
          <h2>Heading</h2>
          <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod. Nullam id dolor id nibh ultricies vehicula ut id elit. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Praesent commodo cursus magna.</p>
          <p><a class="btn btn-default" href="#" role="button">View details &raquo;</a></p>
        </div><!-- /.col-lg-4 -->
        <div class="col-lg-4">
          <img class="img-circle" src="{{ HOME_PATH }}assets/images/head2.jpeg" alt="Generic placeholder image" style="width: 140px; height: 140px;">
          <h2>Heading</h2>
          <p>Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Cras mattis consectetur purus sit amet fermentum. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh.</p>
          <p><a class="btn btn-default" href="#" role="button">View details &raquo;</a></p>
        </div><!-- /.col-lg-4 -->
        <div class="col-lg-4">
          <img class="img-circle" src="{{ HOME_PATH }}assets/images/head3.jpeg" alt="Generic placeholder image" style="width: 140px; height: 140px;">
          <h2>Heading</h2>
          <p>Donec sed odio dui. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Vestibulum id ligula porta felis euismod semper. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.</p>
          <p><a class="btn btn-default" href="#" role="button">View details &raquo;</a></p>
        </div><!-- /.col-lg-4 -->
      </div><!-- /.row -->
    </div> <!-- /.container -->
  </div>

  <hr class="featurette-divider">

  <!-- START THE FEATURETTES -->
  <div class="row featurette" style="background-color:#f6f6f6">
    <div class="container">
      <div class="col-md-6">
        <h2 class="featurette-heading">First featurette heading. <span class="text-muted">It'll blow your mind.</span></h2>
        <p class="lead">Donec ullamcorper nulla non metus auctor fringilla. Vestibulum id ligula porta felis euismod semper. Praesent commodo cursus magna, vel scelerisque nisl consectetur. Fusce dapibus, tellus ac cursus commodo.</p>
      </div>
      <div class="col-md-6">
        <img class="featurette-image img-responsive" src="{{ HOME_PATH }}assets/images/feature2.jpg" alt="Generic placeholder image">
      </div>
    </div>
  </div>

  <hr class="featurette-divider">

  <div class="row featurette">
    <div class="container">
      <div class="col-md-8">
        <img class="featurette-image img-responsive" src="{{ HOME_PATH }}assets/images/feature1.jpg" alt="Generic placeholder image">
      </div>
      <div class="col-md-4">
        <h2 class="featurette-heading">Oh yeah, it's that good. <span class="text-muted">See for yourself.</span></h2>
        <p class="lead">Donec ullamcorper.</p>
      </div>
    </div>
  </div>

  <hr class="featurette-divider">

  <div class="row featurette" style="background-color:#f6f6f6">
    <div class="container">
      <div class="col-md-7">
        <h2 class="featurette-heading">And lastly, this one. <span class="text-muted">Checkmate.</span></h2>
        <p class="lead">Donec ullamcorper nulla non metus auctor fringilla. Vestibulum id ligula porta felis euismod semper. Praesent commodo cursus magna, vel scelerisque nisl consectetur. Fusce dapibus, tellus ac cursus commodo.</p>
      </div>
      <div class="col-md-5">
        <img class="featurette-image img-responsive" data-src="holder.js/500x500/auto" alt="Generic placeholder image">
      </div>
    </div>
  </div>
</div>
<!-- /END THE FEATURETTES -->


