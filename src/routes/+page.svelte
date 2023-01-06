<script>
  import { webVitals } from '../vitals';
  import { page } from '$app/stores';
  import { inject } from '@vercel/analytics';

  // Load the stylesheet
  import '../app.css';

  // Inject vercel analytics
  inject();

  // More vercel analytics
  let analyticsId = import.meta.env.VERCEL_ANALYTICS_ID;

  $: if (analyticsId) {
    webVitals({
      path: $page.url.pathname,
      params: $page.params,
      analyticsId
    })
  }

 function copyLink() {
   navigator.clipboard.writeText('earthbuild.de');
 }
</script>

<div>
 <div class="card_left" on:click={copyLink}>
  <div style="font-size: 24px;font-weight:700;left:20px;position:relative;">EARTHBUILD.DE</div>
  <div style="font-size: 14px;font-weight:700;color:blue;position:absolute;top:60px;left:19px;">Klicke zum kopieren</div>
 </div>
 <div class="logo">
  <a href="https://earthbuild.de/">
   <img alt="Earthbuild Logo" src="/favicon.png">
  </a>
 </div>
 <a href="https://discord.gg/fmxNNE3xnH">
  <div class="card_right">
    <div style="font-size: 24px;font-weight:700;left:20px;position:relative;">DISCORD</div>
  <div style="font-size: 14px;font-weight:700;color:blue;position:absolute;top:60px;left:19px;">Klicke zum joinen</div>
  </div>
 </a>
</div>