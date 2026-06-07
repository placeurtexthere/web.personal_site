---
title: System Settings
---
<h1>System Settings</h1>
<p>Customize environmental parameters, background gradient color vectors, and liquid glass glow aesthetics.</p>

<!-- Cursor Glow Module -->
<div class="form-group" style="margin-top: 25px;">
  <label>Cursor Glow Control</label>
  <div class="control-widget" style="margin-top: 10px;">
    <button class="widget-btn" id="glow-toggle" onclick="toggleOption('cursor-glow')">
      <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><circle cx="12" cy="12" r="10"/><circle cx="12" cy="12" r="4"/></svg>
      Toggle Glow
    </button>
  </div>
  
  <div style="margin-top: 15px; display: grid; grid-template-columns: 1fr 1fr; gap: 20px;">
    <div>
      <label for="intensity-input" style="font-size: 11px;">Glow Intensity</label>
      <input type="range" id="intensity-input" min="0.05" max="0.8" step="0.05" style="width:100%; height: 6px; cursor: pointer;" oninput="updateSetting('glow-intensity', this.value)">
    </div>
    <div>
      <label for="diameter-input" style="font-size: 11px;">Glow Diameter (px)</label>
      <input type="range" id="diameter-input" min="40" max="400" step="10" style="width:100%; height: 6px; cursor: pointer;" oninput="updateSetting('glow-diameter', this.value)">
    </div>
  </div>
</div>

<!-- Wallpaper Gradient Customizer -->
<div class="form-group" style="margin-top: 35px; border-top: 1px solid rgba(255,255,255,0.08); padding-top: 25px;">
  <label>Workspace Wallpaper Canvas</label>
  <p style="font-size: 12px; color: var(--text-secondary); margin-bottom: 15px;">Configure the static three-color gradient matrix and specify the color sweep angle.</p>
  
  <div style="display: grid; grid-template-columns: repeat(4, 1fr); gap: 15px;">
    <div>
      <label for="color1-input" style="font-size: 11px;">Color 1</label>
      <input type="color" id="color1-input" style="width:100%; height:32px; border:1px solid rgba(255,255,255,0.12); border-radius:8px; cursor:pointer; background:none;" onchange="updateSetting('bg-color-1', this.value)">
    </div>
    <div>
      <label for="color2-input" style="font-size: 11px;">Color 2</label>
      <input type="color" id="color2-input" style="width:100%; height:32px; border:1px solid rgba(255,255,255,0.12); border-radius:8px; cursor:pointer; background:none;" onchange="updateSetting('bg-color-2', this.value)">
    </div>
    <div>
      <label for="color3-input" style="font-size: 11px;">Color 3</label>
      <input type="color" id="color3-input" style="width:100%; height:32px; border:1px solid rgba(255,255,255,0.12); border-radius:8px; cursor:pointer; background:none;" onchange="updateSetting('bg-color-3', this.value)">
    </div>
    <div>
      <label for="angle-input" style="font-size: 11px;">Angle (deg)</label>
      <input type="range" id="angle-input" min="0" max="360" step="5" style="width:100%; cursor: pointer;" oninput="updateSetting('bg-angle', this.value)">
    </div>
  </div>
</div>

<!-- Theme Selection Module -->
<div class="form-group" style="margin-top: 35px; border-top: 1px solid rgba(255,255,255,0.08); padding-top: 25px;">
  <label>Interface Theme Mode</label>
  <div class="control-widget" style="margin-top: 10px;">
    <button class="widget-btn" id="dark-theme-toggle" onclick="toggleOption('dark-mode')">
      Dark Mode
    </button>
    <button class="widget-btn" id="light-theme-toggle" onclick="toggleOption('light-mode')">
      Light Mode
    </button>
  </div>
</div>