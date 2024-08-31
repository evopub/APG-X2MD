# APG-X2MD

**Bookmarklet to copy all tweets of a X threads as Markdown : <https://gouillou.com/scripts/apg-x2md.html>**

Generated as a bookmarklet with Claude.ai, but didn't work until being minified and re-bookmarkletified in Visual Studio Code.

## Use

1. Save this bookmarklet as a Bookmark (aka: Signet, Marque-Page, etc.) in your browser : [APG-X2MD](javascript:(()%3D%3E%7B!function(e)%7Bconst%20t%3Ddocument.createElement(%22textarea%22)%3Bt.value%3De%2Cdocument.body.appendChild(t)%2Ct.select()%3Btry%7Bdocument.execCommand(%22copy%22)%7Dcatch(e)%7Bconsole.error(%22Unable%20to%20copy%22%2Ce)%2Calert(%22Unable%20to%20copy!%22)%7Ddocument.body.removeChild(t)%7D(function()%7Bconst%20e%3Ddocument.querySelectorAll('%5Bdata-testid%3D%22tweet%22%5D')%3Blet%20t%3D%22%22%3Bif(e.length%3E0)%7Bconst%20n%3De%5B0%5D%2Co%3Dwindow.location.href.split(%22%3F%22)%5B0%5D%2Cr%3Dn.querySelector(%22time%22)%2Cc%3Dr%3Fr.getAttribute(%22datetime%22)%3A%22Unknown%20Date%22%2Ca%3Dn.querySelector('%5Bdata-testid%3D%22User-Name%22%5D')%2Cl%3Da%3Fa.textContent.split(%22%5Cn%22)%5B0%5D.trim()%3A%22Unknown%20Author%22%3Bt%2B%3D%60%23%20X%20Thread%20by%20%24%7Bl%7D%5Cn%5Cn%60%2Ct%2B%3D%60First%20tweet%3A%20%24%7Bc%7D%5CnURL%3A%20%3C%24%7Bo%7D%3E%5Cn%5Cn%60%7Dreturn%20e.forEach((e%3D%3E%7Bconst%20n%3De.querySelector('%5Bdata-testid%3D%22tweetText%22%5D')%3Bn%26%26(t%2B%3D%60%24%7Bn.innerText%7D%5Cn%60)%2Ce.querySelectorAll('img%5Balt%3D%22Image%22%5D%2C%20video').forEach(((e%2Cn)%3D%3E%7Bif(%22IMG%22%3D%3D%3De.tagName)%7Bconst%20o%3De.src%3Bt%2B%3D%60!%5BImage%20%24%7Bn%2B1%7D%5D(%24%7Bo%7D)%5Cn%60%7Delse%20if(%22VIDEO%22%3D%3D%3De.tagName)%7Bconst%20o%3De.src%7C%7C(e.querySelector(%22source%22)%3Fe.querySelector(%22source%22).src%3A%22%22)%3Bo%26%26(t%2B%3D%60%5BVideo%20%24%7Bn%2B1%7D%5D(%24%7Bo%7D)%5Cn%60)%7D%7D))%2Ct%2B%3D%22%5Cn%22%7D))%2Ct%7D())%2Cfunction(e)%7Bconst%20t%3Ddocument.createElement(%22textarea%22)%3Bt.value%3De%2Cdocument.body.appendChild(t)%2Ct.select()%3Btry%7Bdocument.execCommand(%22copy%22)%7Dcatch(e)%7Balert(%22Unable%20to%20copy!%22)%7Ddocument.body.removeChild(t)%7D(function()%7Bconst%20e%3Ddocument.querySelectorAll('%5Bdata-testid%3D%22tweet%22%5D')%3Blet%20t%3D%22%22%3Bif(e.length%3E0)%7Bconst%20n%3De%5B0%5D%2Co%3Dwindow.location.href.split(%22%3F%22)%5B0%5D%2Cr%3Dn.querySelector(%22time%22)%2Cc%3Dr%3Fr.getAttribute(%22datetime%22)%3A%22Unknown%20Date%22%2Ca%3Dn.querySelector('%5Bdata-testid%3D%22User-Name%22%5D')%2Cl%3Da%3Fa.textContent.split(%22%5Cn%22)%5B0%5D.trim()%3A%22Unknown%20Author%22%3Bt%2B%3D%60%23%20X%20Thread%20by%20%24%7Bl%7D%5Cn%5Cn%60%2Ct%2B%3D%60First%20tweet%3A%20%24%7Bc%7D%5CnURL%3A%20%3C%24%7Bo%7D%3E%5Cn%5Cn%60%7Dreturn%20e.forEach((e%3D%3E%7Bconst%20n%3De.querySelector('%5Bdata-testid%3D%22tweetText%22%5D')%3Bn%26%26(t%2B%3D%60%24%7Bn.innerText%7D%5Cn%60)%2Ce.querySelectorAll('img%5Balt%3D%22Image%22%5D%2C%20video').forEach(((e%2Cn)%3D%3E%7Bif(%22IMG%22%3D%3D%3De.tagName)%7Bconst%20o%3De.src%3Bt%2B%3D%60!%5BImage%20%24%7Bn%2B1%7D%5D(%24%7Bo%7D)%5Cn%60%7Delse%20if(%22VIDEO%22%3D%3D%3De.tagName)%7Bconst%20o%3De.src%7C%7C(e.querySelector(%22source%22)%3Fe.querySelector(%22source%22).src%3A%22%22)%3Bo%26%26(t%2B%3D%60%5BVideo%20%24%7Bn%2B1%7D%5D(%24%7Bo%7D)%5Cn%60)%7D%7D))%2Ct%2B%3D%22%5Cn%22%7D))%2Ct%7D())%3B%7D)()%3B)
  ```javascript
javascript:(()%3D%3E%7B!function(e)%7Bconst%20t%3Ddocument.createElement(%22textarea%22)%3Bt.value%3De%2Cdocument.body.appendChild(t)%2Ct.select()%3Btry%7Bdocument.execCommand(%22copy%22)%7Dcatch(e)%7Bconsole.error(%22Unable%20to%20copy%22%2Ce)%2Calert(%22Unable%20to%20copy!%22)%7Ddocument.body.removeChild(t)%7D(function()%7Bconst%20e%3Ddocument.querySelectorAll('%5Bdata-testid%3D%22tweet%22%5D')%3Blet%20t%3D%22%22%3Bif(e.length%3E0)%7Bconst%20n%3De%5B0%5D%2Co%3Dwindow.location.href.split(%22%3F%22)%5B0%5D%2Cr%3Dn.querySelector(%22time%22)%2Cc%3Dr%3Fr.getAttribute(%22datetime%22)%3A%22Unknown%20Date%22%2Ca%3Dn.querySelector('%5Bdata-testid%3D%22User-Name%22%5D')%2Cl%3Da%3Fa.textContent.split(%22%5Cn%22)%5B0%5D.trim()%3A%22Unknown%20Author%22%3Bt%2B%3D%60%23%20X%20Thread%20by%20%24%7Bl%7D%5Cn%5Cn%60%2Ct%2B%3D%60First%20tweet%3A%20%24%7Bc%7D%5CnURL%3A%20%3C%24%7Bo%7D%3E%5Cn%5Cn%60%7Dreturn%20e.forEach((e%3D%3E%7Bconst%20n%3De.querySelector('%5Bdata-testid%3D%22tweetText%22%5D')%3Bn%26%26(t%2B%3D%60%24%7Bn.innerText%7D%5Cn%60)%2Ce.querySelectorAll('img%5Balt%3D%22Image%22%5D%2C%20video').forEach(((e%2Cn)%3D%3E%7Bif(%22IMG%22%3D%3D%3De.tagName)%7Bconst%20o%3De.src%3Bt%2B%3D%60!%5BImage%20%24%7Bn%2B1%7D%5D(%24%7Bo%7D)%5Cn%60%7Delse%20if(%22VIDEO%22%3D%3D%3De.tagName)%7Bconst%20o%3De.src%7C%7C(e.querySelector(%22source%22)%3Fe.querySelector(%22source%22).src%3A%22%22)%3Bo%26%26(t%2B%3D%60%5BVideo%20%24%7Bn%2B1%7D%5D(%24%7Bo%7D)%5Cn%60)%7D%7D))%2Ct%2B%3D%22%5Cn%22%7D))%2Ct%7D())%2Cfunction(e)%7Bconst%20t%3Ddocument.createElement(%22textarea%22)%3Bt.value%3De%2Cdocument.body.appendChild(t)%2Ct.select()%3Btry%7Bdocument.execCommand(%22copy%22)%7Dcatch(e)%7Balert(%22Unable%20to%20copy!%22)%7Ddocument.body.removeChild(t)%7D(function()%7Bconst%20e%3Ddocument.querySelectorAll('%5Bdata-testid%3D%22tweet%22%5D')%3Blet%20t%3D%22%22%3Bif(e.length%3E0)%7Bconst%20n%3De%5B0%5D%2Co%3Dwindow.location.href.split(%22%3F%22)%5B0%5D%2Cr%3Dn.querySelector(%22time%22)%2Cc%3Dr%3Fr.getAttribute(%22datetime%22)%3A%22Unknown%20Date%22%2Ca%3Dn.querySelector('%5Bdata-testid%3D%22User-Name%22%5D')%2Cl%3Da%3Fa.textContent.split(%22%5Cn%22)%5B0%5D.trim()%3A%22Unknown%20Author%22%3Bt%2B%3D%60%23%20X%20Thread%20by%20%24%7Bl%7D%5Cn%5Cn%60%2Ct%2B%3D%60First%20tweet%3A%20%24%7Bc%7D%5CnURL%3A%20%3C%24%7Bo%7D%3E%5Cn%5Cn%60%7Dreturn%20e.forEach((e%3D%3E%7Bconst%20n%3De.querySelector('%5Bdata-testid%3D%22tweetText%22%5D')%3Bn%26%26(t%2B%3D%60%24%7Bn.innerText%7D%5Cn%60)%2Ce.querySelectorAll('img%5Balt%3D%22Image%22%5D%2C%20video').forEach(((e%2Cn)%3D%3E%7Bif(%22IMG%22%3D%3D%3De.tagName)%7Bconst%20o%3De.src%3Bt%2B%3D%60!%5BImage%20%24%7Bn%2B1%7D%5D(%24%7Bo%7D)%5Cn%60%7Delse%20if(%22VIDEO%22%3D%3D%3De.tagName)%7Bconst%20o%3De.src%7C%7C(e.querySelector(%22source%22)%3Fe.querySelector(%22source%22).src%3A%22%22)%3Bo%26%26(t%2B%3D%60%5BVideo%20%24%7Bn%2B1%7D%5D(%24%7Bo%7D)%5Cn%60)%7D%7D))%2Ct%2B%3D%22%5Cn%22%7D))%2Ct%7D())%3B%7D)()%3B
```
2. On a X thread, go to the bottom of the thread, and click on the bookmarklet. That's all: all the tweets are in the clipboard. 


**Important: this bookmarklet only copy the tweets already displayed, so *before* using it, go to the bottom of the thread (it is sometimes necessary to copy the thread in multiple times)!**


## Code

### Source 

```javascript
javascript:(function() {
    function extractThreadContent() {
        const tweets = document.querySelectorAll('[data-testid="tweet"]');
        let markdown = '';
        if (tweets.length > 0) {
            const firstTweet = tweets[0];
            const tweetUrl = window.location.href.split('?')[0];
            const dateElement = firstTweet.querySelector('time');
            const dateStr = dateElement ? dateElement.getAttribute('datetime') : 'Unknown Date';
            const userNameElement = firstTweet.querySelector('[data-testid="User-Name"]');
            const tweetAuthor = userNameElement ? userNameElement.textContent.split('\n')[0].trim() : 'Unknown Author';
            markdown += `# X Thread by ${tweetAuthor}\n\n`;
            markdown += `First tweet: ${dateStr}\nURL: <${tweetUrl}>\n\n`;
        }
        tweets.forEach((tweet) => {
            const tweetContent = tweet.querySelector('[data-testid="tweetText"]');
            if (tweetContent) {
                markdown += `${tweetContent.innerText}\n`;
            }
            // Handle media attachments
            const mediaElements = tweet.querySelectorAll('img[alt="Image"], video');
            mediaElements.forEach((media, index) => {
                if (media.tagName === 'IMG') {
                    const imgSrc = media.src;
                    markdown += `![Image ${index + 1}](${imgSrc})\n`;
                } else if (media.tagName === 'VIDEO') {
                    const videoSrc = media.src || (media.querySelector('source') ? media.querySelector('source').src : '');
                    if (videoSrc) {
                        markdown += `[Video ${index + 1}](${videoSrc})\n`;
                    }
                }
            });
            markdown += `\n`;
        });  
        return markdown;
    }
    function copyToClipboard(text) {
        const textArea = document.createElement('textarea');
        textArea.value = text;
        document.body.appendChild(textArea);
        textArea.select();
        
        try {
            const successful = document.execCommand('copy');
            const msg = successful ? 'successful' : 'unsuccessful';
        } catch (err) {
			console.error('Unable to copy', err);
			alert('Unable to copy!');

        }
        
        document.body.removeChild(textArea);
    }

    const threadContent = extractThreadContent();
    copyToClipboard(threadContent);
})();
```

### Minified

```javascript
!function(e){const t=document.createElement("textarea");t.value=e,document.body.appendChild(t),t.select();try{document.execCommand("copy")}catch(e){alert("Unable to copy!")}document.body.removeChild(t)}(function(){const e=document.querySelectorAll('[data-testid="tweet"]');let t="";if(e.length>0){const n=e[0],o=window.location.href.split("?")[0],r=n.querySelector("time"),c=r?r.getAttribute("datetime"):"Unknown Date",a=n.querySelector('[data-testid="User-Name"]'),l=a?a.textContent.split("\n")[0].trim():"Unknown Author";t+=`# X Thread by ${l}\n\n`,t+=`First tweet: ${c}\nURL: <${o}>\n\n`}return e.forEach((e=>{const n=e.querySelector('[data-testid="tweetText"]');n&&(t+=`${n.innerText}\n`),e.querySelectorAll('img[alt="Image"], video').forEach(((e,n)=>{if("IMG"===e.tagName){const o=e.src;t+=`![Image ${n+1}](${o})\n`}else if("VIDEO"===e.tagName){const o=e.src||(e.querySelector("source")?e.querySelector("source").src:"");o&&(t+=`[Video ${n+1}](${o})\n`)}})),t+="\n"})),t}());
```

### Bookmarkletified

```javascript
javascript:(()%3D%3E%7B!function(e)%7Bconst%20t%3Ddocument.createElement(%22textarea%22)%3Bt.value%3De%2Cdocument.body.appendChild(t)%2Ct.select()%3Btry%7Bdocument.execCommand(%22copy%22)%7Dcatch(e)%7Bconsole.error(%22Unable%20to%20copy%22%2Ce)%2Calert(%22Unable%20to%20copy!%22)%7Ddocument.body.removeChild(t)%7D(function()%7Bconst%20e%3Ddocument.querySelectorAll('%5Bdata-testid%3D%22tweet%22%5D')%3Blet%20t%3D%22%22%3Bif(e.length%3E0)%7Bconst%20n%3De%5B0%5D%2Co%3Dwindow.location.href.split(%22%3F%22)%5B0%5D%2Cr%3Dn.querySelector(%22time%22)%2Cc%3Dr%3Fr.getAttribute(%22datetime%22)%3A%22Unknown%20Date%22%2Ca%3Dn.querySelector('%5Bdata-testid%3D%22User-Name%22%5D')%2Cl%3Da%3Fa.textContent.split(%22%5Cn%22)%5B0%5D.trim()%3A%22Unknown%20Author%22%3Bt%2B%3D%60%23%20X%20Thread%20by%20%24%7Bl%7D%5Cn%5Cn%60%2Ct%2B%3D%60First%20tweet%3A%20%24%7Bc%7D%5CnURL%3A%20%3C%24%7Bo%7D%3E%5Cn%5Cn%60%7Dreturn%20e.forEach((e%3D%3E%7Bconst%20n%3De.querySelector('%5Bdata-testid%3D%22tweetText%22%5D')%3Bn%26%26(t%2B%3D%60%24%7Bn.innerText%7D%5Cn%60)%2Ce.querySelectorAll('img%5Balt%3D%22Image%22%5D%2C%20video').forEach(((e%2Cn)%3D%3E%7Bif(%22IMG%22%3D%3D%3De.tagName)%7Bconst%20o%3De.src%3Bt%2B%3D%60!%5BImage%20%24%7Bn%2B1%7D%5D(%24%7Bo%7D)%5Cn%60%7Delse%20if(%22VIDEO%22%3D%3D%3De.tagName)%7Bconst%20o%3De.src%7C%7C(e.querySelector(%22source%22)%3Fe.querySelector(%22source%22).src%3A%22%22)%3Bo%26%26(t%2B%3D%60%5BVideo%20%24%7Bn%2B1%7D%5D(%24%7Bo%7D)%5Cn%60)%7D%7D))%2Ct%2B%3D%22%5Cn%22%7D))%2Ct%7D())%2Cfunction(e)%7Bconst%20t%3Ddocument.createElement(%22textarea%22)%3Bt.value%3De%2Cdocument.body.appendChild(t)%2Ct.select()%3Btry%7Bdocument.execCommand(%22copy%22)%7Dcatch(e)%7Balert(%22Unable%20to%20copy!%22)%7Ddocument.body.removeChild(t)%7D(function()%7Bconst%20e%3Ddocument.querySelectorAll('%5Bdata-testid%3D%22tweet%22%5D')%3Blet%20t%3D%22%22%3Bif(e.length%3E0)%7Bconst%20n%3De%5B0%5D%2Co%3Dwindow.location.href.split(%22%3F%22)%5B0%5D%2Cr%3Dn.querySelector(%22time%22)%2Cc%3Dr%3Fr.getAttribute(%22datetime%22)%3A%22Unknown%20Date%22%2Ca%3Dn.querySelector('%5Bdata-testid%3D%22User-Name%22%5D')%2Cl%3Da%3Fa.textContent.split(%22%5Cn%22)%5B0%5D.trim()%3A%22Unknown%20Author%22%3Bt%2B%3D%60%23%20X%20Thread%20by%20%24%7Bl%7D%5Cn%5Cn%60%2Ct%2B%3D%60First%20tweet%3A%20%24%7Bc%7D%5CnURL%3A%20%3C%24%7Bo%7D%3E%5Cn%5Cn%60%7Dreturn%20e.forEach((e%3D%3E%7Bconst%20n%3De.querySelector('%5Bdata-testid%3D%22tweetText%22%5D')%3Bn%26%26(t%2B%3D%60%24%7Bn.innerText%7D%5Cn%60)%2Ce.querySelectorAll('img%5Balt%3D%22Image%22%5D%2C%20video').forEach(((e%2Cn)%3D%3E%7Bif(%22IMG%22%3D%3D%3De.tagName)%7Bconst%20o%3De.src%3Bt%2B%3D%60!%5BImage%20%24%7Bn%2B1%7D%5D(%24%7Bo%7D)%5Cn%60%7Delse%20if(%22VIDEO%22%3D%3D%3De.tagName)%7Bconst%20o%3De.src%7C%7C(e.querySelector(%22source%22)%3Fe.querySelector(%22source%22).src%3A%22%22)%3Bo%26%26(t%2B%3D%60%5BVideo%20%24%7Bn%2B1%7D%5D(%24%7Bo%7D)%5Cn%60)%7D%7D))%2Ct%2B%3D%22%5Cn%22%7D))%2Ct%7D())%3B%7D)()%3B
```









