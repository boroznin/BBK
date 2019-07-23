var OwlRecentWorks=function(){return{initOwlRecentWorksV1:function(){jQuery(document).ready(function(){var owl=jQuery(".owl-recent-works-v1");owl.owlCarousel({items:[5],itemsDesktop:[1000,4],itemsDesktopSmall:[900,3],itemsTablet:[600,2],itemsMobile:[479,1],slideSpeed:1000});jQuery(".next-v2").click(function(){owl.trigger('owl.next');})
jQuery(".prev-v2").click(function(){owl.trigger('owl.prev');})});},};}();var Behaviour={list:new Array,register:function(sheet){Behaviour.list.push(sheet);},start:function(){Behaviour.addLoadEvent(function(){Behaviour.apply();});},apply:function(){for(h=0;sheet=Behaviour.list[h];h++){for(selector in sheet){list=document.getElementsBySelector(selector);if(!list){continue;}
for(i=0;element=list[i];i++){sheet[selector](element);}}}},addLoadEvent:function(func){var oldonload=window.onload;if(typeof window.onload!='function'){window.onload=func;}else{window.onload=function(){oldonload();func();}}}}
Behaviour.start();function getAllChildren(e){return e.all?e.all:e.getElementsByTagName('*');}
document.getElementsBySelector=function(selector){if(!document.getElementsByTagName){return new Array();}
var tokens=selector.split(' ');var currentContext=new Array(document);for(var i=0;i<tokens.length;i++){token=tokens[i].replace(/^\s+/,'').replace(/\s+$/,'');;if(token.indexOf('#')>-1){var bits=token.split('#');var tagName=bits[0];var id=bits[1];var element=document.getElementById(id);if(tagName&&element.nodeName.toLowerCase()!=tagName){return new Array();}
currentContext=new Array(element);continue;}
if(token.indexOf('.')>-1){var bits=token.split('.');var tagName=bits[0];var className=bits[1];if(!tagName){tagName='*';}
var found=new Array;var foundCount=0;for(var h=0;h<currentContext.length;h++){var elements;if(tagName=='*'){elements=getAllChildren(currentContext[h]);}else{elements=currentContext[h].getElementsByTagName(tagName);}
for(var j=0;j<elements.length;j++){found[foundCount++]=elements[j];}}
currentContext=new Array;var currentContextIndex=0;for(var k=0;k<found.length;k++){if(found[k].className&&found[k].className.match(new RegExp('\\b'+className+'\\b'))){currentContext[currentContextIndex++]=found[k];}}
continue;}
if(token.match(/^(\w*)\[(\w+)([=~\|\^\$\*]?)=?"?([^\]"]*)"?\]$/)){var tagName=RegExp.$1;var attrName=RegExp.$2;var attrOperator=RegExp.$3;var attrValue=RegExp.$4;if(!tagName){tagName='*';}
var found=new Array;var foundCount=0;for(var h=0;h<currentContext.length;h++){var elements;if(tagName=='*'){elements=getAllChildren(currentContext[h]);}else{elements=currentContext[h].getElementsByTagName(tagName);}
for(var j=0;j<elements.length;j++){found[foundCount++]=elements[j];}}
currentContext=new Array;var currentContextIndex=0;var checkFunction;switch(attrOperator){case '=':checkFunction=function(e){return(e.getAttribute(attrName)==attrValue);};break;case '~':checkFunction=function(e){return(e.getAttribute(attrName).match(new RegExp('\\b'+attrValue+'\\b')));};break;case '|':checkFunction=function(e){return(e.getAttribute(attrName).match(new RegExp('^'+attrValue+'-?')));};break;case '^':checkFunction=function(e){return(e.getAttribute(attrName).indexOf(attrValue)==0);};break;case '$':checkFunction=function(e){return(e.getAttribute(attrName).lastIndexOf(attrValue)==e.getAttribute(attrName).length-attrValue.length);};break;case '*':checkFunction=function(e){return(e.getAttribute(attrName).indexOf(attrValue)>-1);};break;default:checkFunction=function(e){return e.getAttribute(attrName);};}
currentContext=new Array;var currentContextIndex=0;for(var k=0;k<found.length;k++){if(checkFunction(found[k])){currentContext[currentContextIndex++]=found[k];}}
continue;}
if(!currentContext[0]){return;}
tagName=token;var found=new Array;var foundCount=0;for(var h=0;h<currentContext.length;h++){var elements=currentContext[h].getElementsByTagName(tagName);for(var j=0;j<elements.length;j++){found[foundCount++]=elements[j];}}
currentContext=found;}
return currentContext;}
var xmlhttp
if(!xmlhttp&&typeof XMLHttpRequest!='undefined'){try{xmlhttp=new XMLHttpRequest();}catch(e){xmlhttp=false}}
function myXMLHttpRequest(){var xmlhttplocal;try{xmlhttplocal=new ActiveXObject("Msxml2.XMLHTTP")}catch(e){try{xmlhttplocal=new ActiveXObject("Microsoft.XMLHTTP")}catch(E){xmlhttplocal=false;}}
if(!xmlhttplocal&&typeof XMLHttpRequest!='undefined'){try{var xmlhttplocal=new XMLHttpRequest();}catch(e){var xmlhttplocal=false;alert('couldn\'t create xmlhttp object');}}
return(xmlhttplocal);}
function snd1Reqq(id_num,gal){var theUL=document.getElementById('unit_ul'+id_num);theUL.innerHTML='<i class="fa fa-spinner fa-spin fa-2x"></i>';xmlhttp.open('get','/ratings_1_base/rpc.php?q='+id_num+'&gallery='+gal);xmlhttp.setRequestHeader('X-Requested-With','XMLHttpRequest');xmlhttp.onreadystatechange=handleResponse;xmlhttp.send(null);}
function snd1ReqqGal(id_num,gal){var theUL=document.getElementById('unit_ul'+id_num);theUL.innerHTML='<i class="fa fa-spinner fa-spin"></i>';xmlhttp.open('get','/ratings_1_base/rpc_gal.php?q='+id_num+'&gallery='+gal);xmlhttp.setRequestHeader('X-Requested-With','XMLHttpRequest');xmlhttp.onreadystatechange=handleResponse;xmlhttp.send(null);}
function handleResponse(){if(xmlhttp.readyState==4){if(xmlhttp.status==200){var response=xmlhttp.responseText;var update=new Array();if(response.indexOf('|')!=-1){update=response.split('|');changeText(update[0],update[1]);}}}}
function changeText(div2show,text){var IE=(document.all)?1:0;var DOM=0;if(parseInt(navigator.appVersion)>=5){DOM=1};if(DOM){var viewer=document.getElementById(div2show);viewer.innerHTML=text;}else if(IE){document.all[div2show].innerHTML=text;}}
function disru(){var b1=document.getElementById("b1");var b2=document.getElementById("b2");var b3=document.getElementById("b3");var b4=document.getElementById("b4");var dig=document.getElementById("digit");var code=document.getElementById("code");var dipb1=document.getElementById("dipb1");var month=document.getElementById("ctype");if(month.value==1){b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=true;b2.style.visibility="hidden";b2.style.display="none";b3.disabled=false;b3.style.visibility="visible";b3.style.display="inline-block";b4.disabled=false;b4.style.visibility="visible";b4.style.display="inline-block";code.disabled=true;code.style.visibility="hidden";code.style.display="none";dipb1.disabled=true;dipb1.style.visibility="hidden";dipb1.style.display="none";}
if((month.value==12)||(month.value==15)){b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";b3.disabled=false;b3.style.visibility="visible";b3.style.display="inline-block";b4.disabled=true;b4.style.visibility="hidden";b4.style.display="none";code.disabled=true;code.style.visibility="hidden";code.style.display="none";dipb1.disabled=true;dipb1.style.visibility="hidden";dipb1.style.display="none";}
if((month.value==16)||(month.value==17)||(month.value==2)||(month.value==19)||(month.value==6)){b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";b3.disabled=true;b3.style.visibility="hidden";b3.style.display="none";b4.disabled=true;b4.style.visibility="hidden";b4.style.display="none";code.disabled=true;code.style.visibility="hidden";code.style.display="none";dipb1.disabled=true;dipb1.style.visibility="hidden";dipb1.style.display="none";}
if((month.value==3)||(month.value==4)||(month.value==5)||(month.value==7)||(month.value==8)){b1.disabled=true;b1.style.visibility="hidden";b1.style.display="none";b2.disabled=true;b2.style.visibility="hidden";b2.style.display="none";b3.disabled=false;b3.style.visibility="visible";b3.style.display="inline-block";b4.disabled=false;b4.style.visibility="visible";b4.style.display="inline-block";code.disabled=true;code.style.visibility="hidden";code.style.display="none";dipb1.disabled=true;dipb1.style.visibility="hidden";dipb1.style.display="none";}
if(month.value==20){b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=true;b2.style.visibility="hidden";b2.style.display="none";b3.disabled=true;b3.style.visibility="hidden";b3.style.display="none";b4.disabled=true;b4.style.visibility="hidden";b4.style.display="none";code.disabled=true;code.style.visibility="hidden";code.style.display="none";dipb1.disabled=true;dipb1.style.visibility="hidden";dipb1.style.display="none";}
if((month.value==21)||(month.value==22)){b1.disabled=true;b1.style.visibility="hidden";b1.style.display="none";b2.disabled=true;b2.style.visibility="hidden";b2.style.display="none";b3.disabled=false;b3.style.visibility="visible";b3.style.display="inline-block";b4.disabled=true;b4.style.visibility="hidden";b4.style.display="none";code.disabled=true;code.style.visibility="hidden";code.style.display="none";dipb1.disabled=true;dipb1.style.visibility="hidden";dipb1.style.display="none";}
if(month.value==9){b1.disabled=true;b1.style.visibility="hidden";b1.style.display="none";b2.disabled=true;b2.style.visibility="hidden";b2.style.display="none";b3.disabled=true;b3.style.visibility="hidden";b3.style.display="none";b4.disabled=true;b4.style.visibility="hidden";b4.style.display="none";code.disabled=false;code.style.visibility="visible";code.style.display="inline-block";dipb1.disabled=false;dipb1.style.visibility="visible";dipb1.style.display="inline-block";}}
function dis1(){var b1=document.getElementById("b1");var b2=document.getElementById("b2");var b3=document.getElementById("b3");var b4=document.getElementById("b4");var month=document.getElementById("type");if(month.value==0)
{b1.disabled=false;b2.disabled=false;b3.disabled=false;b4.disabled=false;}
if((month.value==1)||(month.value==2)||(month.value==6)||(month.value==19))
{b1.disabled=false;b2.disabled=false;b3.disabled=true;b4.disabled=true;}
if((month.value==3)||(month.value==4)||(month.value==5)||(month.value==7)||(month.value==8))
{b1.disabled=true;b2.disabled=true;b3.disabled=false;b4.disabled=false;}
if((month.value==12)||(month.value==15))
{b1.disabled=false;b2.disabled=false;b3.disabled=false;b4.disabled=true;}
if(month.value==20)
{b1.disabled=true;b2.disabled=false;b3.disabled=true;b4.disabled=true;}
if((month.value==21)||(month.value==22))
{b1.disabled=true;b2.disabled=true;b3.disabled=false;b4.disabled=true;}}
function disde(){var b1=document.getElementById("b1");var b2=document.getElementById("b2");var season=document.getElementById("season");var transdate=document.getElementById("transdate");var month=document.getElementById("ctype");if(month.value==7){season.disabled=false;season.style.visibility="visible";season.style.display="inline-block";}else{season.disabled=true;season.style.visibility="hidden";season.style.display="none";}
if((month.value==1)||(month.value==5)||(month.value==7)){b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=true;b2.style.visibility="hidden";b2.style.display="none";transdate.disabled=true;transdate.style.visibility="hidden";transdate.style.display="none";}
if(month.value==2){b1.disabled=true;b1.style.visibility="hidden";b1.style.display="none";b2.disabled=true;b2.style.visibility="hidden";b2.style.display="none";transdate.disabled=false;transdate.style.visibility="visible";transdate.style.display="inline-block";}
if(month.value==3){b1.disabled=true;b1.style.visibility="hidden";b1.style.display="none";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";b2.value="";transdate.disabled=false;transdate.style.visibility="visible";transdate.style.display="inline-block";}
if((month.value==6)||(month.value==11)){b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=true;b2.style.visibility="visible";b2.style.display="inline-block";transdate.disabled=true;transdate.style.visibility="hidden";transdate.style.display="none";if(month.value==6){b2.value="H";}
if(month.value==11){b2.value="E";}}
if((month.value==8)||(month.value==9)||(month.value==10)){b1.disabled=true;b1.style.visibility="hidden";b1.style.display="none";b2.disabled=true;b2.style.visibility="hidden";b2.style.display="none";transdate.disabled=true;transdate.style.visibility="hidden";transdate.style.display="none";}}
function disfr(){var b1=document.getElementById("b1");var b2=document.getElementById("b2");var b3=document.getElementById("b3");var season=document.getElementById("season");var dig1=document.getElementById("digit1");var dig2=document.getElementById("digit2");var reg1=document.getElementById("region1");var reg2=document.getElementById("region2");var month=document.getElementById("ctype");if(month.value==3){season.disabled=false;season.style.visibility="visible";season.style.display="inline-block";}else{season.disabled=true;season.style.visibility="hidden";season.style.display="none";}
if(month.value==8){dig1.disabled=false;dig1.style.visibility="visible";dig1.style.display="inline-block";b3.disabled=false;b3.style.visibility="visible";b3.style.display="inline-block";b2.disabled=true;b2.style.visibility="hidden";b2.style.display="none";b1.disabled=true;b1.style.visibility="hidden";b1.style.display="none";dig2.disabled=true;dig2.style.visibility="hidden";dig2.style.display="none";reg2.disabled=false;reg2.style.visibility="visible";reg2.style.display="inline-block";reg1.disabled=true;reg1.style.visibility="hidden";reg1.style.display="none";}else{dig1.disabled=true;dig1.style.visibility="hidden";dig1.style.display="none";b3.disabled=true;b3.style.visibility="hidden";b3.style.display="none";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";dig2.disabled=false;dig2.style.visibility="visible";dig2.style.display="inline-block";reg2.disabled=true;reg2.style.visibility="hidden";reg2.style.display="none";}
if(month.value==2){b1.disabled=true;b1.style.visibility="visible";b1.style.display="inline-block";b1.value="WW";reg1.disabled=false;reg1.style.visibility="visible";reg1.style.display="inline-block";}
if((month.value==1)||(month.value==7)){b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b1.value="";reg1.disabled=false;reg1.style.visibility="visible";reg1.style.display="inline-block";}
if((month.value==3)||(month.value==4)){b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b1.value="";reg1.disabled=true;reg1.style.visibility="hidden";reg1.style.display="none";}
if(month.value==6){b1.disabled=true;b1.style.visibility="visible";b1.style.display="inline-block";b1.value="W";reg1.disabled=false;reg1.style.visibility="visible";reg1.style.display="inline-block";}}
function dises(){var let=document.getElementById("let");var dig1=document.getElementById("digit1");var dig2=document.getElementById("digit2");var reg=document.getElementById("region");var month=document.getElementById("ctype");if(month.value==7){let.disabled=true;let.style.visibility="hidden";let.style.display="none";}else{let.disabled=false;let.style.visibility="visible";let.style.display="inline-block";}
if(month.value==1){reg.disabled=true;reg.style.visibility="hidden";reg.style.display="none";}else{reg.disabled=false;reg.style.visibility="visible";reg.style.display="inline-block";}
if((month.value==1)||(month.value==3)||(month.value==5)){dig1.disabled=false;dig1.style.visibility="visible";dig1.style.display="inline-block";dig2.disabled=true;dig2.style.visibility="hidden";dig2.style.display="none";}else{dig1.disabled=true;dig1.style.visibility="hidden";dig1.style.display="none";dig2.disabled=false;dig2.style.visibility="visible";dig2.style.display="inline-block";}}
function disit2(){var nm1=document.getElementById("nomerpl");var nm2=document.getElementById("nomerpl1");var fon=document.getElementById("fon");var month=document.getElementById("ctype");if(month.value==5)
{if(fon.value==7){nm1.disabled=false;nm1.style.visibility="visible";nm1.style.display="inline-block";nm2.disabled=true;nm2.style.visibility="hidden";nm2.style.display="none";}
else{nm1.disabled=true;nm1.style.visibility="hidden";nm1.style.display="none";nm2.disabled=false;nm2.style.visibility="visible";nm2.style.display="inline-block";}}}
function disch(){var b1=document.getElementById("b1");var reg=document.getElementById("region");var fon=document.getElementById("fon");var month=document.getElementById("ctype");if(month.value==10)
{reg.disabled=true;reg.style.visibility="visible";reg.style.display="inline-block";reg.value="M";}
else
{reg.disabled=false;reg.style.visibility="visible";reg.style.display="inline-block";}
if((month.value==8)||(month.value==9))
{b1.style.visibility="visible";b1.style.display="inline-block";if(month.value==8){b1.value="Z";}
if(month.value==9){b1.value="U";}}
else
{b1.style.visibility="hidden";b1.style.display="none";}
if((month.value==2)||(month.value==3)||(month.value==4))
{fon.disabled=true;fon.style.visibility="hidden";fon.style.display="none";}
else
{fon.disabled=false;fon.style.visibility="visible";fon.style.display="inline-block";}}
function dissuresult(){var b1=document.getElementById("b1");var b2=document.getElementById("b2");var reg1=document.getElementById("region1");var reg2=document.getElementById("region2");var month=document.getElementById("tip");if((month.value==1)||(month.value==5)){b1.disabled=true;b1.style.visibility="hidden";b1.style.display="none";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";reg1.disabled=true;reg1.style.visibility="hidden";reg1.style.display="none";reg2.disabled=false;reg2.style.visibility="visible";reg2.style.display="inline-block";}
if((month.value==3)||(month.value==4)){b1.disabled=true;b1.style.visibility="hidden";b1.style.display="none";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";reg1.disabled=false;reg1.style.visibility="visible";reg1.style.display="inline-block";reg2.disabled=true;reg2.style.visibility="hidden";reg2.style.display="none";}
if(month.value==2){b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=true;b2.style.visibility="hidden";b2.style.display="none";reg1.disabled=false;reg1.style.visibility="visible";reg1.style.display="inline-block";reg2.disabled=true;reg2.style.visibility="hidden";reg2.style.display="none";}
if(month.value==6){b1.disabled=true;b1.style.visibility="hidden";b1.style.display="none";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";reg1.disabled=false;reg1.style.visibility="visible";reg1.style.display="inline-block";reg2.disabled=true;reg2.style.visibility="hidden";reg2.style.display="none";}}
function diskzresult(){var b1=document.getElementById("b1");var b2=document.getElementById("b2");var b3=document.getElementById("b3");var reg1=document.getElementById("region1");var reg2=document.getElementById("region2");var month=document.getElementById("tip");if((month.value==5)||(month.value==6)||(month.value==9)){if(month.value==9)
{b1.disabled=true;b1.value="K";b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=true;b2.value="P";b2.style.visibility="visible";b2.style.display="inline-block";b3.disabled=true;b3.style.visibility="hidden";b3.style.display="none";}
if(month.value==5)
{b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";b3.disabled=false;b3.style.visibility="visible";b3.style.display="inline-block";}
if(month.value==6)
{b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";b3.disabled=true;b3.style.visibility="hidden";b3.style.display="none";}
reg1.disabled=true;reg1.style.visibility="hidden";reg1.style.display="none";reg2.disabled=false;reg2.style.visibility="visible";reg2.style.display="inline-block";}
if(month.value==12)
{b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";b3.disabled=false;b3.style.visibility="visible";b3.style.display="inline-block";reg1.disabled=true;reg1.style.visibility="hidden";reg1.style.display="none";reg2.disabled=true;reg2.style.visibility="hidden";reg2.style.display="none";}
if((month.value==1)||(month.value==2)||(month.value==10)){if(month.value==10)
{b1.disabled=true;b1.value="K";b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=true;b2.value="P";b2.style.visibility="visible";b2.style.display="inline-block";b3.disabled=true;b3.style.visibility="hidden";b3.style.display="none";}
if(month.value==2)
{b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";b3.disabled=false;b3.style.visibility="visible";b3.style.display="inline-block";}
if(month.value==1)
{b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";b3.disabled=true;b3.style.visibility="hidden";b3.style.display="none";}
reg1.disabled=false;reg1.style.visibility="visible";reg1.style.display="inline-block";reg2.disabled=true;reg2.style.visibility="hidden";reg2.style.display="none";}}
function disfrresult(){var b1=document.getElementById("b1");var b2=document.getElementById("b2");var month=document.getElementById("tip");if(month.value==2){b1.disabled=true;b1.style.visibility="visible";b1.style.display="inline-block";b1.value="W";b2.disabled=true;b2.style.visibility="visible";b2.style.display="inline-block";b2.value="W";}
if(month.value==6){b1.disabled=true;b1.style.visibility="visible";b1.style.display="inline-block";b1.value="W";b2.disabled=true;b2.style.visibility="hidden";b2.style.display="none";}
if((month.value==1)||(month.value==3)||(month.value==4)||(month.value==7)){b1.disabled=false;b1.style.visibility="visible";b1.style.display="inline-block";b1.value="A";b2.disabled=false;b2.style.visibility="visible";b2.style.display="inline-block";b2.value="A";}}
function searchru(){var nomer=document.getElementById("nomer");var month=document.getElementById("ctype");if(month.value==1){nomer.placeholder="A 001 AA 77";}
if(month.value==11){nomer.placeholder="A 001 AA";}
if((month.value==16)||(month.value==19)){nomer.placeholder="AA 001 77";}
if((month.value==2)||(month.value==17)||(month.value==6)){nomer.placeholder="AA 0001 77";}
if((month.value==12)||(month.value==15)){nomer.placeholder="AA 001 A 77";}
if((month.value==3)||(month.value==4)||(month.value==7)||(month.value==8)){nomer.placeholder="0001 AA 77";}
if(month.value==20){nomer.placeholder="A 0001 77";}
if(month.value==21){nomer.placeholder="001 A 77";}
if(month.value==22){nomer.placeholder="0001 A 77";}
if(month.value==31){nomer.placeholder="001 CD 1 77";}
if(month.value==32){nomer.placeholder="001 D/T 001 77";}}
function searchua(){var nomer=document.getElementById("nomer");var month=document.getElementById("ctype");if(month.value<5){nomer.placeholder="AA 0001 AA";}
if(month.value==5){nomer.placeholder="11 AA 0001";}
if(month.value==6){nomer.placeholder="T1 AA 0001";}
if(month.value==7){nomer.placeholder="11 0001";}
if(month.value==8){nomer.placeholder="0001 А1";}
if((month.value==11)||(month.value==12)){nomer.placeholder="01 001-01 AA";}
if((month.value==13)||(month.value==14)){nomer.placeholder="00001 AA";}
if(month.value==15){nomer.placeholder="AA 00001";}
if(month.value==20){nomer.placeholder="";}}
function searchsu(){var nomer=document.getElementById("nomer");var month=document.getElementById("ctype");if((month.value==1)||(month.value==3)||(month.value==4)||(month.value==5)){nomer.placeholder="0001 АБВ";}
if(month.value==2){nomer.placeholder="а 0001 АБ";}
if(month.value==6){nomer.placeholder="АБВ 0001";}
if(month.value==7){nomer.placeholder="11 0001";}
if(month.value==8){nomer.placeholder="0001 А1";}
if((month.value==11)||(month.value==12)||(month.value==14)||(month.value==15)||(month.value==16)||(month.value==17)){nomer.placeholder="0001 АБ";}
if((month.value==13)||(month.value==18)){nomer.placeholder="АБ 0001";}}
function searchby(){var nomer=document.getElementById("nomer");var month=document.getElementById("ctype");if((month.value==1)||(month.value==6)){nomer.placeholder="0001 AA-1";}
if(month.value==2){nomer.placeholder="AA 0001-1";}
if(month.value==5){nomer.placeholder="A 0001 A-1";}
if(month.value==7){nomer.placeholder="AA-1 0001";}
if(month.value==12){nomer.placeholder="1AA T 0001";}
if(month.value==13){nomer.placeholder="0001 AAA";}
if(month.value==14){nomer.placeholder="0001 AA";}
if(month.value==15){nomer.placeholder="AA 0001";}}
function searchde(){var nomer=document.getElementById("nomer");var month=document.getElementById("ctype");if((month.value==1)||(month.value==5)){nomer.placeholder="B AB 001";}
if(month.value==2){nomer.placeholder="AB 04001 (21.10.15)";}
if(month.value==3){nomer.placeholder="AB 001 A (21.10.15)";}
if(month.value==6){nomer.placeholder="B AB 001 H";}
if(month.value==7){nomer.placeholder="B AB 001 (04/10)";}
if(month.value==8){nomer.placeholder="AB 06001";}
if(month.value==9){nomer.placeholder="AB 07001";}
if(month.value==10){nomer.placeholder="AB 0001";}
if(month.value==11){nomer.placeholder="B AB 001 E";}}
function searchfr(){var nomer=document.getElementById("nomer");var month=document.getElementById("ctype");if((month.value==1)||(month.value==7)){nomer.placeholder="AB-001-CD 75";}
if(month.value==2){nomer.placeholder="WW-001-CD 75";}
if(month.value==3){nomer.placeholder="AB-001-CD (02/15)";}
if(month.value==4){nomer.placeholder="AB-001-CD";}
if(month.value==6){nomer.placeholder="W-001-CD 75";}
if(month.value==8){nomer.placeholder="1234 AB 75";}}
function searches(){var nomer=document.getElementById("nomer");var month=document.getElementById("ctype");if(month.value==1){nomer.placeholder="0001 ABC";}
if(month.value==3){nomer.placeholder="H 0001 ABC";}
if(month.value==4){nomer.placeholder="ABC 0001 (AB)";}
if(month.value==5){nomer.placeholder="A 0001 A(A)";}
if(month.value==7){nomer.placeholder="A-00001";}}
function searchkz(){var nomer=document.getElementById("nomer");var month=document.getElementById("ctype");if(month.value==1){nomer.placeholder="A 001 AA";}
if(month.value==2){nomer.placeholder="A 001 AAA";}
if((month.value==3)||(month.value==4)){nomer.placeholder="0001 AA";}
if(month.value==10){nomer.placeholder="A 001 KP";}
if(month.value==12){nomer.placeholder="001 AA(A)";}
if(month.value==5){nomer.placeholder="001 AAA 01";}
if((month.value==6)||(month.value==9)){nomer.placeholder="001 AA 01";}
if(month.value==7){nomer.placeholder="AAA 01 01";}
if(month.value==8){nomer.placeholder="01 AA 01";}
if(month.value==13){nomer.placeholder="F 0001 01";}
if(month.value==14){nomer.placeholder="H 0001 01";}}
(function(){var a=document.querySelector('#aside1'),b=null,P=0;window.addEventListener('scroll',Ascroll,false);document.body.addEventListener('scroll',Ascroll,false);function Ascroll(){if(b==null){var Sa=getComputedStyle(a,''),s='';for(var i=0;i<Sa.length;i++){if(Sa[i].indexOf('overflow')==0||Sa[i].indexOf('padding')==0||Sa[i].indexOf('border')==0||Sa[i].indexOf('outline')==0||Sa[i].indexOf('box-shadow')==0||Sa[i].indexOf('background')==0){s+=Sa[i]+': '+Sa.getPropertyValue(Sa[i])+'; '}}
b=document.createElement('div');b.style.cssText=s+' box-sizing: border-box; width: '+a.offsetWidth+'px;';a.insertBefore(b,a.firstChild);var l=a.childNodes.length;for(var i=1;i<l;i++){b.appendChild(a.childNodes[1]);}
a.style.height=b.getBoundingClientRect().height+'px';a.style.padding='0';a.style.border='0';}
var Ra=a.getBoundingClientRect(),R=Math.round(Ra.top+b.getBoundingClientRect().height-document.querySelector('footer').getBoundingClientRect().top+0);if((Ra.top-P)<=0){if((Ra.top-P)<=R){b.className='stop';b.style.top=-R+'px';}else{b.className='sticky';b.style.top=P+'px';}}else{b.className='';b.style.top='';}
window.addEventListener('resize',function(){a.children[0].style.width=getComputedStyle(a,'').width},false);}})()