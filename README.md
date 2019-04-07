# rotate-3d-items-on-click

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Rotate menu</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.3.1/css/bootstrap-grid.min.css">
  <style>
    * {box-sizing: border-box}
    body {
      font-family: sans-serif;
      overflow-x: hidden;
    }
    ul {list-style-type: none;}
    a {text-decoration: none;}

    .rotate-items {
      transition: .3s;
      transform-origin: 0 50%;
    }
    .card {
      border: 1px solid rgba(0,0,0,.125);
      border-radius: .25rem;
      text-align: center;
    }
    .card-header {
      padding: .75rem 1.25rem;
      margin-bottom: 0;
      background-color: rgba(0,0,0,.03);
      border-bottom: 1px solid rgba(0,0,0,.125);
    }
    .card-body {
      padding: 1.25rem;
    }
    .btn {
      display: inline-block;
      font-weight: 400;
      color: #212529;
      text-align: center;
      -webkit-user-select: none;
      -moz-user-select: none;
      -ms-user-select: none;
      user-select: none;
      background-color: transparent;
      border: 1px solid transparent;
      padding: .5rem 1rem;
      font-size: 1rem;
      line-height: 1.5;
      border-radius: .25rem;
      cursor: pointer;
      display: block;
      width: 100%;
    }
    .btn-primary {
      color: #fff;
      background-color: #007bff;
      border-color: #007bff;
    }

    .close-btn {
      color: #fff;
      font-size: 30px;
      position: fixed;
      top: 10px;
      right: 10px;
    }

    .more-menu{
      position: fixed;
      right: 0;
      top: 0;
      max-width: 400px;
      height: 100%;
      background-color: #333;
      color: #fff;
      padding: 40px;
      transition: .3s;
      transform: translateX(100%);
      z-index: 5;
    }
    
    .more-menu:target {
      transform: translateX(0);
    }
    .more-menu:target ~ .rotate-items {
      transform: perspective(1000px) rotateY(10deg);
    }
  </style>
</head>

<body>

  <div class="more-menu" id="free">
    <a href="#close" class="close-btn">&times;</a>
    <h4 class="my-0">Free</h4>
    <p>Далеко-далеко за словесными, горами в стране гласных и согласных живут рыбные тексты. Большой, дороге.</p>
  </div>
  <div class="more-menu" id="pro">
    <a href="#close" class="close-btn">&times;</a>
    <h4 class="my-0">Pro</h4>
    <p>Далеко-далеко за словесными, горами в стране гласных и согласных живут рыбные тексты. Большой, дороге.</p>
  </div>
  <div class="more-menu" id="enterprise">
    <a href="#close" class="close-btn">&times;</a>
    <h4 class="my-0">Enterprise</h4>
    <p>Далеко-далеко за словесными, горами в стране гласных и согласных живут рыбные тексты. Большой, дороге.</p>
  </div>

  <div class="rotate-items mt-5">
    <div class="container">

      <div class="row">

        <div class="col-md-4">
          <div class="card">
            <div class="card-header">
              <h4 class="my-0">Free</h4>
            </div>
            <div class="card-body">
              <h1 class="card-title">$0 <small>/ mo</small></h1>
              <ul>
                <li>10 users included</li>
                <li>2 GB of storage</li>
                <li>Email support</li>
                <li>Help center access</li>
              </ul>
              <a href="#free" class="btn btn-primary">More info</a>
            </div>
          </div>
        </div>

        <div class="col-md-4">
          <div class="card">
            <div class="card-header">
              <h4 class="my-0">Pro</h4>
            </div>
            <div class="card-body">
              <h1 class="card-title">$0 <small>/ mo</small></h1>
              <ul>
                <li>10 users included</li>
                <li>2 GB of storage</li>
                <li>Email support</li>
                <li>Help center access</li>
              </ul>
              <a href="#pro" class="btn btn-primary">More info</a>
            </div>
          </div>
        </div>

        <div class="col-md-4">
          <div class="card">
            <div class="card-header">
              <h4 class="my-0">Enterprise</h4>
            </div>
            <div class="card-body">
              <h1 class="card-title">$0 <small>/ mo</small></h1>
              <ul>
                <li>10 users included</li>
                <li>2 GB of storage</li>
                <li>Email support</li>
                <li>Help center access</li>
              </ul>
              <a href="#enterprise" class="btn btn-primary">More info</a>
            </div>
          </div>
        </div>

      </div>

    </div>
  </div>


</body>

</html>
```
