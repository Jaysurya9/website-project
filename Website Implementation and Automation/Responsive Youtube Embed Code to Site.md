# Add a Responsive Youtube Embed Code to Site

<b>Responsive Youtube Embed Code:</b><br>
This a Script for CSS Inline<br>
Note: Modify src='https://www.youtube.com/embed/<add watch value here>' with actual youtube url. For Example: src='https://www.youtube.com/embed/QKZXPYmD3hM'

    <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%">
      <iframe style="position: absolute; top: 0; left: 0; width: 100%; height: 100%" src='https://www.youtube.com/embed/<add watch value here>' frameborder='0' allowfullscreen></iframe>
    </div>
  
<h3>Alternatives for adding CSS</h3>

<b>Add CSS Styling</b>

    <style>
      .embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } 
      .embed-container iframe, .embed-container object, .embed-container embed 
      { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }
    </style>

<b>Add HTML body</b>

    <div class='embed-container'>
      <iframe src='https://www.youtube.com/embed/<add watch value here>' frameborder='0' allowfullscreen></iframe>
    </div>


# Generate Responsive Youtube Embed Code Online
  
<img src="Images/Embed Responsively.png" alt="Images/Embed Responsively">
  
Click Here to Generate: https://embedresponsively.com/






    

