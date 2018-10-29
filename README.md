# lcd-xml
function sleep(milliseconds) {
    var start = new Date().getTime();
    for (var i = 0; i < 1e7; i++) {
      if ((new Date().getTime() - start) > milliseconds){
        break;
      }
    }
  }
  try
  {
    for(var i = 0;i<12;i++){
        pageGoTo(currentVideo+1);
        sleep(2000);
   }
  }
  catch(e)
  {
      pageGoTo(currentVideo-1)
  }
