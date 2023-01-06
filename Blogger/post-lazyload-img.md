```
<b:if cond='data:view.isPost'>
<script>//<![CDATA[
var psBody = document.querySelector('.postBody');
var lzImgT = psBody.getElementsByTagName('img');
var imgBs = 'data:image/png;base64,R0lGODlhAQABAAD/ACwAAAAAAQABAAACADs=';
for(var i = 0; i < lzImgT.length; i++) {
	var currentSrc = lzImgT[i].getAttribute('src');
	if(currentSrc != imgBs){
		lzImgT[i].setAttribute('src',imgBs);
		lzImgT[i].setAttribute('data-src',currentSrc);
        lzImgT[i].className += ' lazy';}}
//]]>
</script>
</b:if>
```
