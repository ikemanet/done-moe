---
layout: page
comments: true
title: Tell me 麻烦问一下
type: messages
featured: messages.jpg
featured_position: center
---

## 老马有问必答时间

你可以问我``一个``问题，任何问题都行，只要你问我就会回答你 🥳。  
You can ask me ``one`` question of whatever, I promise I will answer it 😉.

![轻松熊](/assets/img/posts/rilakkuma.jpg)

<script>
    var nowDate = new Date();
    var nowYear = nowDate.getUTCFullYear();
    var nowMonth = nowDate.getUTCMonth()+1;
    if (nowMonth < 10) nowMonth = "0"+nowMonth;
    var nowDay = nowDate.getUTCDate();
    if (nowDay < 10) nowDay = "0"+nowDay;
    var nowHour = nowDate.getUTCHours();
    if (nowHour < 10) nowHour = "0"+nowHour;
    var nowMinute = nowDate.getUTCMinutes();
    if (nowMinute < 10) nowMinute = "0"+nowMinute;
    var nowSecond = nowDate.getUTCSeconds();
    if (nowSecond < 10) nowSecond = "0"+nowSecond;
    
    
    var nowDateStr = nowYear + '-' + nowMonth + '-' + nowDay + 'T' + nowHour + ':' + nowMinute + ':' + nowSecond + '.000Z';
    console.log("ike.today: new date is " + nowDateStr)
    localStorage.setItem("ike.today.q2a.lasttime", nowDateStr);
</script>