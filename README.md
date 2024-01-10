# UAS DJANGO
## Pameran Design Arsitektur Berbasis Web (statis) 

```
Raja Happyanto (ketua) / 312210235
Mohammad Hapiyansyah (wakil) / 312210243
Muhammad Ryamizard Ryopa Sakti (anggota) /312210185
Sahrul Ridwansyah (anggota) / 312210063
```

# 1. Register

![Screenshot (119)](https://github.com/sahrul180304/uasdjango/assets/115526901/f4e7a653-30bc-4fb6-b08c-5f874476ab1c)

# 2. login

![login](https://github.com/sahrul180304/uasdjango/assets/115526901/a2deb743-3dc0-42a3-882d-4024bd855b08)

# 3. home 
![Screenshot (115)](https://github.com/sahrul180304/uasdjango/assets/115526901/b4af2861-46fc-4c51-8fd0-d53b51417729)
![Screenshot (114)](https://github.com/sahrul180304/uasdjango/assets/115526901/d012dd68-1703-4939-b433-7f2480111c7c)
![Screenshot (113)](https://github.com/sahrul180304/uasdjango/assets/115526901/70eda9ca-f9b6-47e3-8f82-1152d9776024)


# 4. creat profile

![Screenshot (117)](https://github.com/sahrul180304/uasdjango/assets/115526901/a23f9ee4-7419-4a36-8a54-480fa40c1993)
![Screenshot (116)](https://github.com/sahrul180304/uasdjango/assets/115526901/cdb68eb9-cd3e-40d5-a715-2697e8df901b)
![Screenshot (118)](https://github.com/sahrul180304/uasdjango/assets/115526901/106a5562-671f-46c8-a53c-6f145eb11f50)


# index code 
```

{% extends 'base.html' %}

{% block title %}Home{% endblock title %}


{% block body %}
{% if messages %}
{% for message in messages %}
<div class="alert alert-{{ message.tags }} warning alert-dismissible fade show" role="alert">
  <strong>{{ message }}</strong>
  <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
</div>
{% endfor %}
{% endif %}
<!-- Slider starts -->
<div id="carouselExampleInterval" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active" data-bs-interval="2000">
      <img src="../static/img/dpn1.jpg" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <h5>konsultaion your project</h5>
        <p>Visualisasikan rumah anda dengan kami</p>
        <a href="#baa" class="btn btn-primary btn-md" tabindex="-1" role="button" aria-disabled="true">Make an
          Appointment</a>
        <a href="#dep1" class="btn btn-primary btn-md" tabindex="-1" role="button" aria-disabled="true">View
          Departments</a>
      </div>
    </div>
    <div class="carousel-item" data-bs-interval="2000">
      <img src="../static/img/ft2.jpg" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <h5>konsultaion your project</h5>
        <p>Visualisasikan rumah anda dengan kami</p>
        <a href="#baa" class="btn btn-primary btn-md" tabindex="-1" role="button" aria-disabled="true">Make an
          Appointment</a>
        <a href="#dep1" class="btn btn-primary btn-md" tabindex="-1" role="button" aria-disabled="true">View
          Departments</a>
      </div>
    </div>
    <div class="carousel-item" data-bs-interval="2000">
      <img src="../static/img/ft3.jpg" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <<h5>konsultaion your project</h5>
        <p>Visualisasikan rumah anda dengan kami</p>
        <a href="#baa" class="btn btn-primary btn-md" tabindex="-1" role="button" aria-disabled="true">Make an
          Appointment</a>
        <a href="#dep1" class="btn btn-primary btn-md" tabindex="-1" role="button" aria-disabled="true">View
          Departments</a>
      </div>
    </div>
    <div class="carousel-item" data-bs-interval="2000">
      <img src="../static/img/ft4.jpg" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <h5>konsultaion your project</h5>
        <p>Visualisasikan rumah anda dengan kami</p>

        <a href="#baa" class="btn btn-primary btn-md" tabindex="-1" role="button" aria-disabled="true">konsultasi
          Design</a>
        <a href="#dep1" class="btn btn-primary btn-md" tabindex="-1" role="button" aria-disabled="true">View
          Our team</a>
      </div>
    </div>
    <div class="carousel-item">
      <img src="../static/img/ft5.jpg" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <h5>konsultaion your project</h5>
        <p>Visualisasikan rumah anda dengan kami</p>
        <a href="#baa" class="btn btn-primary btn-md" tabindex="-1" role="button" aria-disabled="true">Make an
          Appointment</a>
        <a href="#dep1" class="btn btn-primary btn-md" tabindex="-1" role="button" aria-disabled="true">View
          Departments</a>
      </div>
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleInterval" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleInterval" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
<!-- Slider ends -->


<!-- <div class="d-grid gap-2 col-6 mx-auto">
  
</div> -->

<!-- card system starts -->
<div class="cards mt-3 p-5" style="background-color: #fbfbfb;">
  <div class="container">
    <div class="row">
      <div class="col-sm-4">
        <div class="card">
          <div class="card-body">
            <h5 class="card-title alert alert-primary">Top Rated Designer</h5>
            <p class="card-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Odio ipsam eligendi,
              consectetur ex fugiat assumenda optio nam sit officia harum repellendus voluptates perferendis, pariatur
              quis vero, consequatur beatae totam iure!</p>
            <a href="#" class="btn btn-outline-primary">see more</a>
          </div>
        </div>
      </div>
      <div class="col-sm-4">
        <div class="card">
          <div class="card-body">
            <h5 class="card-title alert alert-primary">Designer</h5>
            <p class="card-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Odio ipsam eligendi,
              consectetur ex fugiat assumenda optio nam sit officia harum repellendus voluptates perferendis, pariatur
              quis vero, consequatur beatae totam iure!</p>
            <a href="/emDoc" class="btn btn-outline-primary btn-md" tabindex="-1" role="button"
              aria-disabled="true">Find designer</a>
          </div>
        </div>
      </div>
      <div class="col-sm-4">
        <div class="card">
          <div class="card-body "> 
            <h5 class="card-title alert alert-primary">Opening Hours</h5>
            <div class="row  g-1 p-2 pb-2">
              <div class="col-sm-5">
                <ul class="list-group">
                  <li class="list-group-item">Mon to Fri</li>
                  <li class="list-group-item">Saturday</li>
                  <li class="list-group-item">Sunday</li>
                </ul>
              </div>
              <div class="col-sm-2">
                <ul class="list-group">
                  <li class="list-group-item">--</li>
                  <li class="list-group-item">--</li>
                  <li class="list-group-item">--</li>
                </ul>
              </div>
              <div class="col-sm-5">
                <ul class="list-group">
                  <li class="list-group-item">8:00 - 17:00</li>
                  <li class="list-group-item">7:30 - 17:30</li>
                  <li class="list-group-item">9:30 - 15:00</li>
                </ul>

              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- card system ends -->

<div class="container mt-3 pt-5 pb-5" id="baa">
  <div class="row">
    <div class="col-6">
      <h4 class="card-title alert alert-primary p-3">Book an Appointment</h4>
      <div class="form d-flex p-3">
        <form action="" method="post">
          {% csrf_token %}
          <div class="row">
            {% if doc and dep %}
            <div class="col-6">
              <select class="form-select form-select" aria-label=".form-select-sm example" id="sedep" name="sedep"
                required>
                <option selected>Select Department</option>
                {% for d in dep %}
                <option>{{d.dep_name}}</option>
                {% endfor %}
              </select>
              <div class="input-group mt-3">
                <input type="text" class="form-control" placeholder="your name" aria-label="Username"
                  aria-describedby="basic-addon1" id="name" name="name" required>
              </div>
              <div class="mt-3">
                <input type="email" class="form-control" id="mail" name="mail" aria-describedby="emailHelp"
                  placeholder="your email" required>
              </div>

            </div>
            <div class="col-6">
              <select class="form-select form-select" aria-label=".form-select-sm example" id="sedoc" name="sedoc"
                required>
                <option selected>Select Doctor</option>
                {% for de in dep %}
                {% for do in doc %}
                {% if de.dep_name == do.department %}
                <option>{{do.doctor_name}}</option>
                {% endif %}
                {% endfor %}
                {% endfor %}
              </select>
              <div class="input-group mt-3">
                <input type="text" class="form-control" placeholder="phone number" aria-label="Username"
                  aria-describedby="basic-addon1" id="phone" name="phone" required>
              </div>

              <div class="input-group date mt-3" id="datepicker">
                <input type="text" class="form-control" id="date" name="date" required />
                <span class="input-group-append" style="cursor: pointer;">
                  <span class="input-group-text bg-light d-block">
                    <i class="fa fa-calendar"></i>
                  </span>
                </span>
              </div>
            </div>
            <div class="d-grid gap-2 col-6 mx-auto">
              <button type="submit" class="btn btn-outline-primary mt-3">Make a Payment</button>

            </div>


            {% endif %}

          </div>
        </form>
      </div>
    </div>
    <div class="col-6 p-3">
      <div class="faq pt-1 pb-1" style="color: #084298;">
        <h6>FAQ</h6>
      </div>
      <div class="class pt-2 pb-2">
        <h4>
          Have Some Questions?
        </h4>
      </div>
      <div class="accordion" id="accordionExample">
        <div class="accordion-item">
          <h2 class="accordion-header" id="headingOne">
            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne"
              aria-expanded="true" aria-controls="collapseOne">
              What is your Appointment policy?
            </button>
          </h2>
          <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne"
            data-bs-parent="#accordionExample">
            <div class="accordion-body">
              Lorem ipsum dolor, sit amet consectetur adipisicing elit. Assumenda corporis temporibus autem nemo,
              repudiandae deserunt praesentium sed velit illo natus?
            </div>
          </div>
        </div>
        <div class="accordion-item">
          <h2 class="accordion-header" id="headingTwo">
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
              data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
              What should I do if I'm ill?
            </button>
          </h2>
          <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo"
            data-bs-parent="#accordionExample">
            <div class="accordion-body">
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Tenetur animi expedita velit, consectetur vitae
              repellendus neque perferendis facilis impedit quod?
            </div>
          </div>
        </div>
        <div class="accordion-item">
          <h2 class="accordion-header" id="headingThree">
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
              data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
              What are your regular office houre?
            </button>
          </h2>
          <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree"
            data-bs-parent="#accordionExample">
            <div class="accordion-body">
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolorem asperiores amet ea totam ipsam sapiente
              sint praesentium, omnis quasi sed!
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- departmenst section starts -->
<div class="departments pt-5 pb-5" id="dep1" style="background-color: #fbfbfb;">
  <div class="container">
    <div class="row">
      <div class="col-4">
        <div class="dep">
          <h4 class="card-title alert alert-primary p-3">portofolio</h4>
        </div>
        <div class="list">
          <ul class="list-group list-group-flush">
            {% if dep %}
            {% for d in dep %}
            <a href="./{{d.dep_name}}" class="list-group-item list-group-item-action">{{d.dep_name}}</a>
            {% endfor %}
            {% endif %}
          </ul>
        </div>
      </div>
      <div class="col-8">
        <div class="ino pt-1 pb-1 mt-2" style="color: #084298;">
          <h6>Innovation</h6>
        </div>
        <div class="ourdep pt-2 pb-2">
          <h4>Our Work</h4>
        </div>
        <div class="owl-carousel owl-theme">
          <div class="item">
            <div class="card border-0 shadow">
              <img src="../static/img/ft5.jpg" alt="" style="height: 162px;">
              <div class="card-body">
                <h4>house design</h4>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Id, debitis.</p>
                <a href="#" class="btn btn-outline-primary btn-sm" tabindex="-1" role="button">see more</a>
              </div>
            </div>
          </div>
          <!-- item ends -->
          <div class="item">
            <div class="card border-0 shadow">
              <img src="../static/img/ft2.jpg" alt="" style="height: 162px;">
              <div class="card-body">
                <h4>house design</h4>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Id, debitis.</p>
                <a href="#" class="btn btn-outline-primary btn-sm" tabindex="-1" role="button">see more</a>
              </div>
            </div>
          </div>
          <div class="item">
            <div class="card border-0 shadow">
              <img src="../static/img/ft3.jpg" alt="" style="height: 162px;">
              <div class="card-body">
                <h4>Gastroenterologists</h4>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Id, debitis.</p>
                <a href="#" class="btn btn-outline-primary btn-sm" tabindex="-1" role="button">see more</a>
              </div>
            </div>
          </div>
          <div class="item">
            <div class="card border-0 shadow">
              <img src="../static/img/ft4.jpg" alt="" style="height: 162px;">
              <div class="card-body">
                <h4>house design</h4>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Id, debitis.</p>
                <a href="#" class="btn btn-outline-primary btn-sm" tabindex="-1" role="button">see more</a>
              </div>
            </div>
          </div>
          <div class="item">
            <div class="card border-0 shadow">
              <img src="../static/img/ft4.jpg" alt="" style="height: 162px;">
              <div class="card-body">
                <h4>Psychiatry</h4>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Id, debitis.</p>
                <a href="#" class="btn btn-outline-primary btn-sm" tabindex="-1" role="button">see more</a>
              </div>
            </div>
          </div>
          <div class="item">
            <div class="card border-0 shadow">
              <img src="../static/img/ft4.jpg" alt="" style="height: 162px;">
              <div class="card-body">
                <h4>house design</h4>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Id, debitis.</p>
                <a href="#" class="btn btn-outline-primary btn-sm" tabindex="-1" role="button">see more</a>
              </div>
            </div>
          </div>
          <div class="item">
            <div class="card border-0 shadow">
              <img src="../static/img/ft5.jpg" alt="" style="height: 162px;">
              <div class="card-body">
                <h4>house design</h4>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Id, debitis.</p>
                <a href="#" class="btn btn-outline-primary btn-sm" tabindex="-1" role="button">see more</a>
              </div>
            </div>
          </div>
        </div>


      </div>
    </div>
  </div>
</div>
<!-- departmenst section ends -->
<!-- review section starts -->
<div class="review pt-5 pb-5">
  <div class="container">
    
    <h4 class="card-title alert alert-primary p-3 text-center">Terimakasih telah berkunjung</h4>
    
    <div class="owl-carousel owl-theme">
      {% if re %}
      {% for rev in re %}
      <div class="item">
        <div class="card mb-3" style="max-width: 540px;">
          <div class="row g-0">
            <div class="col-md-4">
              <img src="../static/img/emdoc1.svg" class="img-fluid rounded-start" alt="..." style="width: 100%;
            height: 14vw;object-fit: cover;">
            </div>
            <div class="col-md-8">
              <div class="card-body">
                <h5 class="card-title">{{rev.name}}</h5>
                <p class="card-text">{{rev.reviews}}</p>
                <p class="card-text"><small class="text-muted">Published at : {{rev.time}}</small></p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- item ends -->
      {% endfor %}
      {% endif %}

    </div>

  </div>
</div>
<!-- review section ends -->


<!-- footer section -->
<div class="footer">
  <footer class="bg-primary d-flex p-2">
      <span class="text-light text-center m-auto"
        >All rights reserverd &copy; Universitas pelita bangsa .kelompokoop</span>
    </footer>
</div>
<!-- footer section -->





<script src="../static/cla.js"></script>
<script>
  $('.owl-carousel').owlCarousel({
    loop: true,
    margin: 10,
    nav: true,
    responsive: {
      0: {
        items: 1
      },
      600: {
        items: 3
      },
      1000: {
        items: 3
      }
    }
  })
</script>



{% endblock body %}
```
# base code
```
{% extends 'base.html' %}

{% block title %}Contact{% endblock title %}

{% block body %}

<!-- alert message -->
{% if messages %}
{% for message in messages %}
<div class="alert alert-{{ message.tags }} warning alert-dismissible fade show" role="alert">
    <strong>{{ message }}</strong> 
    <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
</div>
{% endfor %}
{% endif %}


<h1>hello this is a contact page</h1>
{% if user.is_authenticated %}
<h1>my name is {{fname}}</h1>
<h4>Your are successfullay logged in</h4>
<a href="/signout" class="btn btn-outline-primary " tabindex="-1" role="button" aria-disabled="true">Sign Out</a>

{% else %}
<h4>sorry! try agin</h4>
{% endif %}

{% endblock body %}
 ```
