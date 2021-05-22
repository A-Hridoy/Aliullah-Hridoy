<!DCOTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>Digital Clock</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="clock">
        <div class="hour">
            <div class="hr" id="hr"></div>
        <div>
        <div class="min">
            <div class="mn" id="mn"></div>
        </div>
        <div class="sec">
            <div class="sc" id="sc"></div>
        </div>
    </div>
    <script type="text/javascript">
      const deg = 6;
      const hr = document.qureyselector('#hr');
      const mn = document.qureyselector('#mn');
      const sc = document.qureyselector('#sc');
setInterval(()=> {
      let day = new Date();
      let hh = day.getHours() * 30;
      let mn = day.getMinutes() * deg;
      let ss = day.getSeconds() * deg;

      hr.style.transform= 'rotateZ(${(hh)+(mm/12)}deg)';
      mn.style.transform= 'rotateZ(${mm}deg)';
      hr.style.transform= 'rotateZ(${ss}deg)';
      })
    </script>
</body>
</html>
