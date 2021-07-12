# Task-2-comine-code is :

<!DOCTYPE html>

<html lang="en">

<head>

 <title>combine pages</title>

 <meta charset="utf-8">

 <meta name="viewport" content="width=device-width, initial-scale=1">

 <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">

 <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>

 <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>

 <link rel="stylesheet" href="style.css">

 <script src="jquery-3.6.0.min.js"></script>

<style>

 

*{

 margin: 0%;

 padding: 0%;

 box-sizing: border-box;

}



html,body{

 display: grid;

 height: max-content;

 place-items: center;

}



.alice-blue{

 color: aliceblue;

}



.center-content{

 display: flex;

 height: max-content;

 align-items: center;

}

.outer-content{

 position: relative;

 margin-left: 0px;

 margin-right: 5rem;

 background-color: red;

}

.custom-btn{

 height: 7rem;

 width: 22rem;

}

.circle{

 height: 20rem;

 width: 20rem;

 border-radius: 50%;

}

.outer-content button, .outer-content span{

 position: absolute;

 top: 50%;

 left: 50%;

 transform: translate(-50%, -50%);

}

.outer-content button{

 background-color: #52006A;

 color: white;

 outline: none;

 border: none;

 font-size: 2rem;

 z-index: 9;

 letter-spacing: 0.1rem;

 text-transform: uppercase;

 cursor: pointer;

}

.custom-btn button{

 height: 6rem;

 width: 21rem;

}

.circle button{

 height: 18rem;

 width: 18rem;

 border-radius: 50%;

}

.outer-content span{

 height: max-content;

 width: 100%;

 background: inherit;

}

.outer-content:hover span:nth-child(1){

 filter: blur(7px);

}

.outer-content:hover span:nth-child(2){

 filter: blur(14px);

}

.outer-content:hover{

 background: linear-gradient(#14ffe9, #ffeb3b, #ff00e0);

 animation: rotate 1.5s linear infinite;

}

@keyframes rotate {

 0%{

 filter: hue-rotate(0deg);

 }

 100%{

 filter: hue-rotate(360deg);

 }

}

@media (max-width: 500px){

 .center-content{

 flex-wrap: wrap;

 flex-direction: column;

 }

 .outer-content{

 margin: 50px 0;

 }



}



</style>







</head>







<body>





  -->



 

<h1 class="alice-blue" class="alice-blue"> لوحة التحكم بالذراع</h1>

-->



<p>المحرك الاول</p>



 

 

 

 <div class="value left">0</div>

 <div class="value right">180</div>

 





<div class="range">





<div class="sliderValue">

 <span>180</span>

</div>

<div class="field">

 <div class="value left">0</div>

 <input type="range" min="0" max="180" value="90" >

 <div class="value right">180</div>

</div>

</div>

 -->



<p>المحرك الثاني</p>



<div class="range">

<div class="sliderValue">

 <span>180</span>

</div>

<div class="field">

 <div class="value left">

 0</div>

 <input type="range" min="0" max="180" value="90" >

 <div class="value right">

 180</div>

</div>

</div>





<p>المحرك الثالث</p>



<div class="range">

<div class="sliderValue">

 <span>180</span>

</div>

<div class="field">

 <div class="value left">

 0</div>

 <input type="range" min="0" max="180" value="90" >

 <div class="value right">

 180</div>

</div>

</div>

-->



<p>المحرك الرابع</p>



<div class="range">

<div class="sliderValue">

 <span>180</span>

</div>

<div class="field">

 <div class="value left">

 0</div>

 <input type="range" min="0" max="180" value="90" >

 <div class="value right">

 180</div>

</div>

</div>




<p>المحرك الخامس</p>



<div class="range">

<div class="sliderValue">

 <span>180</span>

</div>

<div class="field">

 <div class="value left">

 0</div>

 <input type="range" min="0" max="180" value="90" >

 <div class="value right">

 180</div>

</div>

</div>



->



<p>المحرك السادس</p>



<div class="range">

<div class="sliderValue">

 <span>180</span>

</div>

<div class="field">

 <div class="value left">

 0</div>

 <input type="range" min="0" max="180" value="90" >

 <div class="value right">

 180</div>

</div>

</div>

<br>

<button type="button" class="btn"> حفظ</button>

<br>

<button type="button" class="btn"> تشغيل</button>


<script>

$(document).ready(function () {



 $('input[type="range"]').on('input', function(){

 var bubble = $(this).parent().parent().find('.sliderValue span');

 bubble.text($(this).val());

 bubble.addClass('show');

 bubble.css('left', $(this).val() / 2 + '%');

 });

 

 $('input[type="range"]').on('blur', function(){

 $(this).parent().parent().find('.sliderValue span').removeClass('show');

 });



});

</script>







<br>

<br>

<br>

<br>

<br>

<br>









<h1 class="alice-blue">الاتجاهات لقاعدة الروبوت </h1>



<br>



<br>

<br>

 <div class="center-content">

 

 <span></span>

 

 <table style="width:40%">

 <tr>

 <th> </th>

 <th> </th> 

 <th> </th>

 </tr>

 <tr>

<td></td>

 <td> <div class="center-content">

 <div class="outer-content custom-btn">

 <button>للاعلى</button>

 <span></span>

 <span></span>

 </div> </td>

 <td> </td>

 </tr> </div>

 

 <br>

 

 <tr>

 <td></td> <div class="outer-content custom-btn">

 <button>لليسار</button>

 <span></span>

 <span></span>

 </div>

 </div>

 <br>

 <br> <br> <br> <br> <br>

 

 

 </td>

 <td> 

 <br><br><br><br>

 

 

 <div class="outer-content circle">

 <button>توقف</button>

 <span></span>

 <span></span>

 </div>

 </td>

 

 <td>

 

 <br>

 <br>

 <br>

 <br>

 <div class="outer-content custom-btn">

 <button>لليمين</button>

 <span></span>

 <span></span>

 </div> 

 </td>

 </tr> </div>

 

 

 

 <tr>

 

 

 <td></td>

 <td> 

 <br><br><br><br>

 

 <div class="outer-content custom-btn">

 <button>للخلف</button>

 <span></span>

 <span></span>

 </div>

 <td> 

 </td>

 </tr>

 



</body>

</html>

