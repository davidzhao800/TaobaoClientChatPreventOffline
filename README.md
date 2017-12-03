
# Setup
请使用Chrome 打开developer tools，切换至console， 将以下code粘贴进去 按ENTER


# 开始防掉线

var jq = document.createElement('script');
jq.src = "https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js";
document.getElementsByTagName('head')[0].appendChild(jq);

var dt = new Date();
var intervalID = setInterval(function(){$("#chat-input").val("[防掉线]" + dt.toUTCString() + "by davidzhao800");$("#btn-send").click();}, 24000);

# 结束防掉线

clearInterval(intervalID);