
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #111111;
}
</style>
</head>
<body>
  
<div id="result"></div>

<script>
if(typeof(EventSource) !== "undefined") {
  var source = new EventSource("demo_sse.php");
  source.onmessage = function(event) {
    document.getElementById("result").innerHTML += event.data + "<br>";
  };
} else {
  document.getElementById("result").innerHTML = "Sorry, your browser does not support server-sent events...";
}
</script>

<h1>WELCOME TO HELLO WORLD</h1>
<p>from the begining e hard oo:</p>

<ul>
  <li><a href="https://jennis775.github.io/hello-world/">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>
<a href="https://imgbb.com/"><img src="https://i.ibb.co/CWJ0c3P/Naruto-Uzumaki.png" alt="Naruto-Uzumaki" width="700" height="600" border="0"></a>

</body>
</html>
