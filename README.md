<html>
  <head>
    <style>
      #color-block {
        width: 1920px;
        height: 1080px;
        display: inline-block;
      }
    </style>
  </head>
  <body>
    <div id="color-block"></div>
    <script>
      const colorBlock = document.getElementById("color-block");
      const colors = ["red", "blue", "green", "yellow", "purple"];
      let index = 0;

      setInterval(function () {
        colorBlock.style.backgroundColor = colors[index];
        index = (index + 1) % colors.length;
      }, 2000);
    </script>
  </body>
</html>
