<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  {% include head.html %}
  <title></title>
</head>
<body>
<div class="container-fluid">
  <div class="row header-row">
    <div class="col-md-12">
      <header class="well well-sm"><h1 id="site-title">{{site.title}}</h1></header>
    </div>
  </div>
  
  {{content}}

</div>
</body>
</html>
