# stopwatch-js

Simple Stopwatch/Timer/Countdown using HTML+JS 

<a href="https://codepen.io/fox24/pen/xxEKPXB"><b> DEMO </b></a>

<b> Setting up </b>

1. Fork and clone the repository
2. open Stopwatch.html in any browser 

<b> Contribution </b>

1. Follow the instruction in Setting up
2. Create issues and wait for it to be reviewed


<b> HTML </b>


```
<div class="wrapper">
   <h2>Stopwatch</h2>
        <p><span id="seconds">00</span>
        <span id="b">:</span>
        <span id="tens">00</span></p>
        <button id="button-start">Start</button>
        <button id="button-stop">Stop</button>
        <button id="button-reset">Reset</button>
 </div> 
 ```
 
 <b> JAVASCRIPT </b>
 
START
```
buttonStart.onclick = function() {
      
       clearInterval(Interval);
       Interval = setInterval(startTimer, 10);
    }
```

STOP
```
buttonStop.onclick = function() {
         clearInterval(Interval);
    }
```

RESET
```
buttonReset.onclick = function() {
       clearInterval(Interval);
      tens = "00";
        seconds = "00";
      appendTens.innerHTML = tens;
        appendSeconds.innerHTML = seconds;
    }
```
