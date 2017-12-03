


var jq = document.createElement('script');
jq.src = "https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js";
document.getElementsByTagName('head')[0].appendChild(jq);

var dt = new Date();
var intervalID = setInterval(function(){$("#chat-input").val("[防掉线]" + dt.toUTCString() + "by davidzhao800");$("#btn-send").click();}, 24000);


clearInterval(intervalID);