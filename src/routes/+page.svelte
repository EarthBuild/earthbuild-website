<script>
  import '../app.css';

  function isMobileDevice() {
  return (window.innerWidth <= 600 && window.innerHeight <= 800);
};

 var isMobile = isMobileDevice();

 function copyLink() {
   navigator.clipboard.writeText('earthbuild.de');
 }
</script>

<div>
 {#if !isMobile}
 <div class="card_left" on:click={copyLink}>
  <div style="font-size: 24px;font-weight:700;left:20px;position:relative;">EARTHBUILD.DE</div>
  <div style="font-size: 14px;font-weight:700;color:blue;position:absolute;top:60px;left:19px;">Klicke zum kopieren</div>
 </div>
 {/if}
 <div class="logo">
  <a href="https://earthbuild.de/">
   <img alt="Earthbuild Logo" src="https://cdn.discordapp.com/attachments/812383975611432960/1060555560916893837/earthbuild-removebg-preview.png">
  </a>
 </div>
 <a href="https://discord.gg/fmxNNE3xnH">
  <div class="card_right">
    <div style="font-size: 24px;font-weight:700;left:20px;position:relative;">DISCORD</div>
  <div style="font-size: 14px;font-weight:700;color:blue;position:absolute;top:60px;left:19px;">Klicke zum joinen</div>
  </div>
 </a>
</div>