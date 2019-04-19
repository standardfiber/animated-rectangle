======

<div class="heading">
  Animated Photo
</div>
<div class="container">
  <div class="box">
    <img src="http://www.standardfiber.com/images/product/conforters-poly-inset.jpg" alt="Nice Photo">
    <i class="fas fa-camera-retro"></i>
  </div>
</div>


======

body {
  margin: 0;
}

.heading {
  background-color: orange;
  font-size: 42px;
  font-family: "Raleway", sans-serif;
  text-align: center;
  padding: 10px 10px;
  position: relative;
  top: 0;
}

.container {
  background-color: silver;
  display: flex;
  justify-content: center;
  position: relative;
  top: 20px;
}

div.box {
  position: relative;
  top: 20px;
  height: 240px;
  width: 320px;
  background-color: green;
  box-shadow: 10px 10px 35px -15px rgba(0, 0, 0, 0.75);
}

div.box img {
  position: absolute;
  top: 0;
  height: 240px;
  width: 320px;
}

div.box i {
  color: white;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: scale(4);
}

div.box:hover img {
  opacity: 0.4;
  filter: grayscale(100%);
}

div.box * {
  transition: all 0.35s ease-in-out;
}

div.box i {
  transform: scale(0);
}

div.box:hover i {
  transform: scale(4);
  transition: transform 0.35s ease-in;
}
