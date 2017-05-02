# infoBox
 jQuery plugin to create information boxes
<br>
Developed by Arun Thomas
<br>
www.ajarunthomas.com
<br>
<br>
<a href="http://www.ajarunthomas.com/jquery/infoBox/demo/" target="_blank" style="text-decoration:none">Demo</a>
<a download href="http://www.ajarunthomas.com/files/infoBox.js" target="_blank" style="text-decoration:none">Download</a>
<br><br>
<a href="http://www.ajarunthomas.com/jquery/infoBox/" target="_blank" style="text-decoration:none">Website</a>
##USAGE
###Step 1 : Include js
If you want to have an information sign to show the information box pop-up at the end of a paragraph, then include an anchor tag at the end of the paragraph. This anchor tag content will be data showing inside the information box. Once the plugin is initialized, this anchor tag will have an information sign and when mouse placed over this sign will show an information box pop-up with our intially entered anchor tag content
```
<script src="https://code.jquery.com/jquery-1.12.0.min.js"></script>
<script type="text/javascript" src="js/infoBox.js"></script>
```
###Step 2 : Include the HTML content
```
<p>This will the paragraph content
    <a id="sampledata">This will be the information box content</a>
</p>
```
###Step 3 : Initialize the plugin
```
$(document).ready(function(){
    $('#sampledata').infoBox();
});
```
Default Settings: Width of information pop-up box will be 200, position will be below the information sign, text color will be white and background color will be black
### more options
You can customize your information boxes with more options
```
$(document).ready(function(){
    $('#sampledata').infoBox({
        "width":300,    //width of information box pop-up
        "position":"above", //position whether above or below the information sign
        "text_color":"white",   //color of the text 
        "bg_color":"grey"   //background color
    }); 
});
```
