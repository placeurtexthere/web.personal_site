---
title: Inquire
---
<h1>Spatial Inquiry Form</h1>
<p>To submit details, input information below. Inputs are rendered with adaptive, semi-transparent backgrounds to blend with underlying wallpapers.</p>

<form onsubmit="event.preventDefault(); alert('Transmission completed.');" style="padding-bottom: 60px;">
  <div class="form-group">
    <label for="name">Identity</label>
    <input type="text" id="name" class="glass-field" required placeholder="Name">
  </div>
  <div class="form-group" style="margin-top: 15px;">
    <label for="email">Digital Address</label>
    <input type="email" id="email" class="glass-field" required placeholder="email@address.com">
  </div>
  <button class="widget-btn" type="submit" style="margin-top: 20px; font-weight:600;">Transmit Data</button>
</form>