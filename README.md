# danielFrancisOlivieri.github.io

<!DOCTYPE html>
<html>
<title>Coyle</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.0/jquery.min.js"></script>
<script src="http://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js"></script>
<script src="http://ajax.googleapis.com/ajax/libs/angularjs/1.4.8/angular.min.js"></script>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<script src="http://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
<link rel="stylesheet" href="http://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">

<link rel="stylesheet" href="http://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
<link rel="stylesheet" href="http://www.w3schools.com/lib/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Lato">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Montserrat">
<link rel="stylesheet" href="http://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.6.3/css/font-awesome.min.css">
<head>

</head>

<style>
.onoffswitch {
    position: relative; width: 90px;
    -webkit-user-select:none; -moz-user-select:none; -ms-user-select: none;
	margin: auto;
	text-align: left;
	position: relative;
margin-top: 15px;
}

.onoffswitch-checkbox {
    display: none;
}
.onoffswitch-label {
    display: block; overflow: hidden; cursor: pointer;
    border: 2px solid #999999; border-radius: 20px;
}
.onoffswitch-inner {
    display: block; width: 200%; margin-left: -100%;
    transition: margin 0.3s ease-in 0s;
}
.onoffswitch-inner:before, .onoffswitch-inner:after {
    display: block; float: left; width: 50%; height: 30px; padding: 0; line-height: 30px;
    font-size: 14px; color: white; font-family: Trebuchet, Arial, sans-serif; font-weight: bold;
    box-sizing: border-box;
}
.onoffswitch-inner:before {
    content: "|";
    padding-left: 15px;
    background-color: #34A7C1; color: #FFFFFF;
}

.onoffswitch-inner:after {
    content: "O";
    padding-right: 15px;
    background-color: #EEEEEE; color: #999999;
    text-align: right;
}

.onoffswitch-switch {
    display: block; width: 32px; margin: 0.5px;
    background: #FFFFFF;
    position: absolute; top: 0; bottom: 0;
    right: 56px;
    border: 2px solid #999999; border-radius: 20px;
    transition: all 0.3s ease-in 0s;
}
.onoffswitch-checkbox:checked + .onoffswitch-label .onoffswitch-inner {
    margin-left: 0;
}
.onoffswitch-checkbox:checked + .onoffswitch-label .onoffswitch-switch {
    right: 0px;
}

.switchLabel {
padding: 30px;
postion: relative;
display: block;
text-align: center;
font-family: "Lato";
}


body,h1, h3,h4,h5,h6 {font-family: Courier New;
align: center;
}
body {

  background-color: #f44336;
}
.fa-pencil-square-o,.fa-code {font-size:260px}
#btndiv {
display: block;
border-color: black;
margin-top: 15px;
}
button, #modal1 {
position: relative;
display: block;
 border-radius: 23%;
 text-align: center;

clear: left;
  margin: auto;
    width: 8%;
    border: 3px solid #179ee0;
    padding: 10px;
}
p {
display: inline-block;
font-family: Courier New;
font-size: 18px;
}
.synDiv, #traits, #story{
border: dashed;
padding: 20px;
border-color: black;
text-align: left;
display: block;
  margin: auto;
    width: 50%;
align: center;
}
textarea {
display: none;
}
#radioButtons {
display: block;
}
.words {
text-decoration: none;
display: inline-block;
}
.disappear{
display: none;
}
#switch2 {
margin-top: 15px;
}
.footnotes, .MoD{
visibility: hidden;
display: inline-block;
}
#endnotes {
visibility: hidden;
}
.quote {
color: #f44336;
}

.collapse {

}
.labels {
border: none;
background-color: #f44336;
}


 .carousel-inner > .item > img,
 .carousel-inner > .item > a > img {
     width: 70%;
     margin: auto;
 }
 .affix {
      top: 0;
      width: 100%;
  }

  .affix + .container-fluid {
      padding-top: 70px;
  }


</style>
<body>





<!-- Header -->
<div class="w3-container w3-red w3-center w3-padding-128">
  <h1 id = "#title" class="w3-margin w3-jumbo"> <span title = "Many thanks to W3 schools, Kyle Stetz, and the people who made the icons" class="label label-primary"> Charcter Assembly </span> </h1>
  <br>
  <h3 data-toggle="tooltip" data-placement="bottom" title="Randall Munroe called, he wants his mouseover text back." > Start Figuring that Character Out </h3>

<div  ng-app="myApp" ng-controller="myChar">
<div class="synDiv" >
<div>
Name? <input class = "labels" type="text" ng-model="name" placeholder="Luke Skywalker">
</div><br>
<div>
Gender? <input class = "labels" type="text" ng-model="gender" placeholder="Male"><br>
</div>
<br>
<div>
Age? <input class = "labels" type="text" ng-model="age" placeholder="20"><br>
</div>
<br>
<div>
What power do they have? <input class = "labels" type="text" ng-model="power" placeholder="the force"><br>
</div>
<br>
<div>
What do they fear? <input class = "labels" type="text" ng-model="fear" placeholder="Darth Vader"><br>
</div>
<br>
<div>
What do they wear? <input class = "labels" type="text" ng-model="wear" placeholder="orange jumpsuit"><br>
</div>
<br>
<div>
What's in their pocket? <input class = "labels" type="text" ng-model="pocket" placeholder="a lightsaber"><br>
</div>
<br>
<div>
What do they dislike? <input class = "labels" type="text" ng-model="dislike" placeholder="not having a hand"><br>
</div>
<br>
<div>
What do they like? <input class = "labels" type="text" ng-model="like" placeholder="spaceships"><br>
</div>
<br>
<div>
What are they obssessed with? <input class = "labels" type="text" ng-model="obsession" placeholder="his dad"><br>
</div>
<br>
<div>
What trait do they hate in themself? <input class = "labels" type="text" ng-model="hate" placeholder="can't save 'em all"><br>
</div>
<br>
<div>
What phrase do they overuse? <input class = "labels" type="text" ng-model="catchphrase" placeholder="may the force be with you"><br>
</div>
<br>
<div>
What is their central thesis? <input class = "labels" type="text" ng-model="thesis" placeholder="it's good to be good"><br>
</div>
<br>

</div>

<br>
  <div class="container-fluid bg-1 text-center" id = "circle">
  <h3  class="w3-margin w3-jumbo"> <span title = "Many thanks to W3 schools, Kyle Stetz, and the people who made the icons" class="label label-primary"> Story Assembly </span></h3>
  <br>
  <img src="https://notjustamoviepodcast.files.wordpress.com/2014/08/story-circle.png" id = "circleImg" class="img-responsive" style="display:inline" alt="Bird" width="500" height="500"> </img>
<br>
<br>

</div>
<br>

<div class="synDiv">
  <div>
  Title: <input class = "labels" type="text" ng-model="title" placeholder="Star Wars">
  </div><br>
<div>
You: <input class = "labels" type="text" ng-model="you" placeholder="moisture farmer">
</div><br>
<div>
Need: <input class = "labels" type="text" ng-model="need" placeholder="to be independent"><br>
</div>
<br>
<div>
 Go: <input class = "labels" type="text" ng-model="go" placeholder="to Mos Eisley"><br>
</div>
<br>
<div>
Search: <input class = "labels" type="text" ng-model="search" placeholder="for Leia"><br>
</div>
<br>
<div>
Find: <input class = "labels" type="text" ng-model="find" placeholder="the force"><br>
</div>
<br>
<div>
Take: <input class = "labels" type="text" ng-model="take" placeholder="a medal"><br>
</div>
<br>
<div>
Return: <input class = "labels" type="text" ng-model="return" placeholder="to being a civilian"><br>
</div>
<br>
<div>
Change: <input class = "labels" type="text" ng-model="change" placeholder="become a jedi"><br>
</div>
<br>
</div>
<br>

<button type="button" class="btn btn-info" data-toggle="collapse" data-target="#demo" style = "background-color: #179ee0 "> <span class="label label-danger"> Summary </span> </button>
<br>
<br>
  <div id="demo" class="collapse">
<div id = "traits" style = "text-align: left">
  <textarea id="summary" class="form-control" col = "13" rows="50" id="comment" placeholder="Gatsby believed in the green light..." value ="copied" >
{{name}}

{{gender}}

{{age}}

{{power}}

{{fear}}

{{rfgu}}

{{wear}}

{{pocket}}

{{dislike}}

{{like}}

{{obsession}}

{{hate}}

{{catchphrase}}

{{thesis}}

{{title}}

{{you}}

{{need}}

{{go}}

{{search}}

{{find}}

{{take}}

{{return}}

{{change}}
</textarea>
<br>

<br>
</div>
</div>
<br>

<button type="button" class="btn btn-info" data-toggle="collapse" data-target="#demo2" style = "background-color: #179ee0 "> <span class="label label-danger"> Story </span> </button>
<br>
<br>
  <div id="demo2" class="collapse">
<div id = "story" style = "text-align: left" >
<p> {{name}} begins as a {{age}} year old who has the power of {{power}}. {{name}} is {{you}} but is not satisfied. He gets up in the morning because {{rfgu}}. But then he needs {{need}} a he goes to
{{go}}. There he searches for {{search}}. He eventually finds {{find}} and takes {{take}}. He returns and {{change}}. </p>

  <br>
 <label for="comment">Comment:</label>
<textarea class="form-control" rows="5" id="comment" placeholder="Gatsby believed in the green light..."></textarea>
</div>
</div>
</div>
</div>


<script>
var app = angular.module('myApp', []);
app.controller('myChar', function($scope) {

    $scope.name= "Luke Skywalker";
    $scope.gender= "Male";
    $scope.age = "20";
    $scope.power ="the force";
    $scope.fear = "the void";
    $scope.rfgu = "to become a pilot";


        $scope.wear= "orange jumpsuit";
        $scope.pocket= "a lightsaber";
        $scope.dislike = "not having a hand";
        $scope.like ="spaceships";
        $scope.obsession = "the force";
        $scope.hate = "can't save 'em all'";
        $scope.catchphrase = "may the force be with you";
        $scope.thesis = "it's good to be good";

$scope.title= "Star Wars";
    $scope.you= "moisture farmer";
    $scope.need= "to be independent";
    $scope.go = "to Mos Eisely";
    $scope.search ="for Leia";
    $scope.find = "the force";
    $scope.take = "a medal";
    $scope.return = "to being a civilian";
    $scope.change = "become a jedi";


});
</script>


</div>


<!-- Modal -->

<div class="container">

  <!-- Trigger the modal with a button -->
  <button type="button" class="btn btn-info btn-lg" data-toggle="modal" data-target="#myModal" id = "modal1" >Modal</button>

  <!-- Modal -->
  <div class="modal fade" id="myModal" role="dialog">
    <div class="modal-dialog">

      <!-- Modal content-->
      <div class="modal-content">
        <div class="modal-header">
          <button type="button" class="close" data-dismiss="modal">&times;</button>
          <h4 class="modal-title">Alternate Form</h4>
        </div>
        <div class="modal-body">
            <label for="comment">It doesn't have to be good</label>
         <textarea class="form-control" rows="5" id="comment" placeholder="In my younger and more vulnerable years..."></textarea>
              <br>
        <!--  <img src= "https://www.iconexperience.com/_img/g_collection_png/standard/512x512/robot.png"> </img> -->
        </div>
        <div class="modal-footer">
        <!--  <button type="button" class="close" data-dismiss="modal">&times;</button> -->
        </div>
      </div>

    </div>
  </div>

</div>

<!-- Footer -->
<footer class="w3-container w3-padding-64 w3-center w3-opacity">
  <div class="w3-xlarge w3-padding-32">
   <a href="#" class="w3-hover-text-indigo"><i class="fa fa-cubes"></i></a>
   <a href="#" class="w3-hover-text-red"><i class="fa fa-database"></i></a>
   <a href="#" class="w3-hover-text-light-blue"><i class="fa fa-plug"></i></a>
   <a href="#" class="w3-hover-text-grey"><i class="fa fa-tasks"></i></a>
   <a href="#" class="w3-hover-text-indigo"><i class="fa fa-tint"></i></a>
 </div>
 <div >
     <h1 class = "w3-text-red" class = "quote" > <strong>  "Computers are like old testament God, lots of rules and no mercy." </strong> </h1>
 	<h3 style="align: left" class = "w3-text-red" class = "quote"> <strong> - Joseph Campbell </strong> </h3>
 </div>
 <h4 id = "endnotes" style = "display: block;" title="If you think that I'm pretentious for adding this, just be glad I didn't name it 'Endnotes and Errata'"> Endnotes </h4>
 <p class = "footnotes" id = "footnote1">1. And this really did define their personality. It would often cause like </p> <p> <a class="words" id="dfwAdj1"> <a></p> <p class = "footnotes"> nightmares. Some say that this is what caused their obsession with </p> <p><a class="words" id="dfwNoun1"></a></p><p class = "footnotes">.</p> <br>
  <p class = "footnotes" id = "footnote2">2. Other people would perfer to use the adjective </p> <p><a class="words" id="dfwAdj2"> </a></p> <p class = "footnotes">instead.</p> <br>
    <p class= "MoD" class = "footnotes" id = "footnote3">3. And they drank like mulled wine and honied lamb as they did it. </p> <br>
</footer>
<script>
// Used to toggle the menu on small screens when clicking on the menu button

/*
    Copy text from any appropriate field to the clipboard
  By Craig Buckler, @craigbuckler
  use it, abuse it, do whatever you like with it!
*/
(function() {

    'use strict';

  // click events
  document.body.addEventListener('click', copy, true);

    // event handler
    function copy(e) {

    // find target element
    var
      t = e.target,
      c = t.dataset.copytarget,
      inp = (c ? document.querySelector(c) : null);

    // is element selectable?
    if (inp && inp.select) {

      // select text
      inp.select();

      try {
        // copy text
        document.execCommand('copy');
        inp.blur();

        // copied animation
        t.classList.add('copied');
        setTimeout(function() { t.classList.remove('copied'); }, 1500);
      }
      catch (err) {
        alert('please press Ctrl/Cmd+C to copy');
      }

    }

    }

})();

function myFunction() {
    var x = document.getElementById("navDemo");
    if (x.className.indexOf("w3-show") == -1) {
        x.className += " w3-show";
    } else {
        x.className = x.className.replace(" w3-show", "");
    }
}

$(document).ready(function(){
    $('[data-toggle="tooltip"]').tooltip();
});
</script>
</body>
</html>
