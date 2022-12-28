<style>
 :global(html) {
  background-image: url(https://cdn.discordapp.com/attachments/812383975611432960/1057395352728244264/image.png);
 }

 :global(body) {
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  font-size: 60px;
  color: white;
  display: flex;
  justify-content: center;
  margin-top: 10%;
 }

 .hover_scale {
  transition: all .15s ease;
 }

 .hover_scale:hover {
  transform: scale(1.05);
 }

 .logo {
  text-decoration: none;
  color: white;
 }

 .card_left {
  transition: all .15s ease;
  width: 261px;
  height: 95px;

  background: rgba(53, 53, 53, 0.5);
  border-radius: 10px;
  position: absolute;
  left: 90px;
  top: 255px;
  align-items: center;
  display: flex;
 }

 .card_left:hover {
  transform: scale(1.05);
  cursor: pointer;
 }

 .card_right {
  transition: all .15s ease;
  width: 261px;
  height: 95px;

  background: rgba(53, 53, 53, 0.5);
  border-radius: 10px;
  position: absolute;
  right: 90px;
  top: 255px;
  align-items: center;
  display: flex;
 }

 .card_right:hover {
  transform: scale(1.05);
  cursor: pointer;
 }

 a {
  text-decoration: none;
  color: white;
 }
</style>

<script>
 function copyLink() {
   navigator.clipboard.writeText('earthbuild.de');
 }
</script>

<div>
 <div class="card_left" on:click={copyLink}>
  <div style="font-size: 24px;font-weight:700;left:20px;position:relative;">EARTHBUILD.DE</div>
  <div style="font-size: 14px;font-weight:700;color:blue;position:absolute;top:60px;left:19px;">Klicke zum kopieren</div>
 </div>
 <div class="hover_scale">
  <a href="https://earthbuild.de/" class="logo">
   <h1>Earthbuild</h1>
  </a>
 </div>
 <a href="https://discord.gg/fmxNNE3xnH">
  <div class="card_right">
    <div style="font-size: 24px;font-weight:700;left:20px;position:relative;">DISCORD</div>
  <div style="font-size: 14px;font-weight:700;color:blue;position:absolute;top:60px;left:19px;">Klicke zum joinen</div>
  </div>
 </a>
</div>