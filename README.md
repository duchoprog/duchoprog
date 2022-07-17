
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style type="text/css" media="screen">

        body{
            background-color: gold;
            font-family: Arial, Helvetica, sans-serif;
        }

        .wrapper{
            background-color: crimson;
            display:flex;
            margin:1rem;
            padding:1rem;
            min-height: 80vh;  
            flex-direction: row;  
            justify-content: space-around;        
        }

        .wrapper>div{
            background-color: rgb(89, 37, 183);
            flex:1;
            margin:2rem;                     
        }
        .one{
            padding:2rem;
            line-height:3em;
        }

        .one>div:first-child{
            margin-bottom: 2rem;
            text-align: center;
            height: 4rem;
            
        }
        .two{
            flex:2 !important;
            background-color: darkgreen !important;
        }
  /* ----------------- */
  @-webkit-keyframes mask-move {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(210px);
  }
}
@keyframes mask-move {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(210px);
  }
}
@-webkit-keyframes mask-inner-move {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-210px);
  }
}
@keyframes mask-inner-move {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-210px);
  }
}
*,
*:before,
*:after {
  box-sizing: border-box;
}



.focus {
  font-size: 3rem;
  color: white;
  letter-spacing: 0.2rem;
  line-height: 1;
  position: relative;
  width: 179px;
}
.focus:before {
  content: " duchoprog";
  filter: blur(3px);
}
.focus:after {
  content: "";
  position: absolute;
  width: 50px;
  height: calc(100% + 8px);
  top: -4px;
  left: 0;
  border-top: 2px solid;
  border-bottom: 2px solid;
  -webkit-animation: mask-move 2s linear infinite alternate;
          animation: mask-move 2s linear infinite alternate;
}
.focus--mask {
  overflow: hidden;
  position: absolute;
  width: 50px;
  height: 100%;
  top: 0;
  left: 0;
  background: rgb(89, 37, 183);
  -webkit-animation: mask-move 2s linear infinite alternate;
          animation: mask-move 2s linear infinite alternate;
}
.focus--mask-inner {
  -webkit-animation: mask-inner-move 2s linear infinite alternate;
          animation: mask-inner-move 2s linear infinite alternate;
}



  /* ----------------- */
.know{
    padding:0.1rem;
    border-radius: 0.5rem;
    font-family: 'Courier New', Courier, monospace;
}
.know:nth-child(3n){
    background-color:red ;
}
.know:nth-child(3n-2){
    background-color:green ;
}
.know:nth-child(3n-1){
    background-color:yellow ;
}

       


        </style>
</head>
<body>
    <div class="wrapper">
        <div class="one">
            <div class="focus"> 
                <div class="focus--mask">
                  <div class="focus--mask-inner"> duchoprog</div>
                </div>
              </div>

            <div>
                <span class="know">HTML5</span>
                <span class="know">CSS</span>
                <span class="know">Javascript</span>
                <span class="know">React</span>
                <span class="know">Vue</span>
                <span class="know">Node.js</span>
                <span class="know">Express</span>
                <span class="know">SQL</span>
                <span class="know">Sequelize</span>
                <span class="know">Java</span>
                <span class="know">// Look</span>
                <span class="know">at</span>
                <span class="know">all</span>
                <span class="know">this</span>
                <span class="know">room</span>
                <span class="know">to</span>
                <span class="know">learn</span>
                <span class="know">new</span>
                <span class="know">stuff!</span>
            </div>
        </div>
        <div class="two"></div>
        

    </div>
    
</body>

