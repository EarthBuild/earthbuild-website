<script>
import { browser } from '$app/environment';
 
let isMobile = false;

if (browser) {
 function detectMobile() {
   const userAgent = navigator.userAgent;
   isMobile = userAgent.match(/Android/i) || userAgent.match(/webOS/i) || userAgent.match(/iPhone/i) || userAgent.match(/iPad/i) || userAgent.match(/iPod/i) || userAgent.match(/BlackBerry/i) || userAgent.match(/Windows Phone/i);
 }

 detectMobile()
}

export { isMobile };
</script>