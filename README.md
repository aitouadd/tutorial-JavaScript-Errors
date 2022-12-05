# tutorial-JavaScript-Errors

# Throw, and Try...Catch...Finally
The ***try*** statement defines a code block to run (to try).

The ***catch*** statement defines a code block to handle any error.

The ***finally*** statement defines a code block to run regardless of the result.

The ***throw*** statement defines a custom error.


 #  Syntax:
     
                            try
                               {
                                   // code that may throw an error
                               }
                               catch(ex)
                               {
                                   // code to be executed if an error occurs
                               }
                               finally{
                                   // code to be executed regardless of an error occurs or not
                               }
# Example :

              <!DOCTYPE html>
              <html>
              <body>

              <h2>JavaScript try catch</h2>

              <p>Please input a number between 5 and 10:</p>

              <input id="demo" type="text">
              <button type="button" onclick="myFunction()">Test Input</button>
              <p id="p01"></p>

              <script>
              function myFunction() {
                const message = document.getElementById("p01");
                message.innerHTML = "";
                let x = document.getElementById("demo").value;
                try { 
                  if(x == "")  throw "empty";
                  if(isNaN(x)) throw "not a number";
                  x = Number(x);
                  if(x < 5)  throw "too low";
                  if(x > 10)   throw "too high";
                }
                catch(err) {
                  message.innerHTML = "Input is " + err;
                }
              }
              </script>

              </body>
              </html>





Click this link to see how the code works : https://dreamy-banoffee-072fe4.netlify.app


next.. The Error Object

   
   
      
  
