# learnJavaScript
A repository for lessons and practice and collaboration with JavaScipt
// here is a sample of using JavaScript within the HTML  ( not recommended)
<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta charset="utf-8">
    <title>
        Apply JavaScript example</title>
    document.addEventListener("DOMContentLoaded", function() {
        function createParagraph() {
          let para = document.createElement('p');
          para.textContent = 'You clicked the button!';
          document.body.appendChild(para);
        }
      
        const buttons = document.querySelectorAll('button');
      
        for(let i = 0; i < buttons.length ; i++) {
          buttons[i].addEventListener('click', createParagraph);
        }
      });
  </head>
  <body>
    <button>Click me</button>
  </body>
</html>
