<script>
  import '../app.css';

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