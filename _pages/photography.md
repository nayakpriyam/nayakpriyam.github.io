---
layout: archive
title: "Photography"
permalink: /photography/
author_profile: true
---

# My Photography

<style>
.gallery {
  display: flex;
  flex-wrap: wrap;
  gap: 24px;
  justify-content: center;
}
.gallery-item {
  width: 300px;
  margin-bottom: 24px;
  background: #f9f9f9;
  border-radius: 10px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.08);
  overflow: hidden;
  text-align: center;
  display: flex;
  flex-direction: column;
  cursor: pointer;
}
.gallery-item img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  display: block;
  transition: opacity 0.2s;
}
.gallery-item:hover img {
  opacity: 0.85;
}
.caption {
  padding: 10px;
  font-size: 1em;
  color: #555;
  background: #fafafa;
}

/* Lightbox styles */
#lightbox-overlay {
  display: none;
  position: fixed;
  z-index: 9999;
  left: 0; top: 0; right: 0; bottom: 0;
  background: rgba(0,0,0,0.85);
  justify-content: center;
  align-items: center;
}
#lightbox-overlay.active {
  display: flex;
}
#lightbox-img {
  max-width: 90vw;
  max-height: 80vh;
  border-radius: 10px;
  box-shadow: 0 4px 24px rgba(0,0,0,0.2);
}
#lightbox-caption {
  color: #fff;
  text-align: center;
  margin-top: 15px;
  font-size: 1.1em;
}
#lightbox-close {
  position: absolute;
  top: 30px;
  right: 40px;
  font-size: 2.5em;
  color: #fff;
  cursor: pointer;
  font-weight: bold;
  z-index: 10000;
  background: none;
  border: none;
}
</style>

<!-- Lightbox popup markup -->
<div id="lightbox-overlay">
  <button id="lightbox-close" title="Close">&times;</button>
  <div style="text-align:center;">
    <img id="lightbox-img" src="" alt="">
    <div id="lightbox-caption"></div>
  </div>
</div>

<div class="gallery">
  <div class="gallery-item" onclick="showLightbox('/images/2735841B-73E4-40AD-B33C-E9B28C7D34B5.jpg','CSMT Station at midnight')">
    <img src="/images/2735841B-73E4-40AD-B33C-E9B28C7D34B5.jpg" alt="CSMT Station at midnight">
    <div class="caption">CSMT Station at midnight</div>
  </div>
  <div class="gallery-item" onclick="showLightbox('/images/IMG_0616.JPG','Early morning at Gateway of India, Mumbai')">
    <img src="/images/IMG_0616.JPG" alt="Early morning at Gateway of India, Mumbai">
    <div class="caption">Early morning at Gateway of India, Mumbai</div>
  </div>
  <div class="gallery-item" onclick="showLightbox('/images/dudhsagar-2.jpg','Dudhsagar Falls, Goa')">
    <img src="/images/dudhsagar-2.JPG" alt="Dudhsagar Falls, Goa">
    <div class="caption">Dudhsagar Falls, Goa</div>
  </div>
  <div class="gallery-item" onclick="showLightbox('/images/IMG_0590.JPG','Mumbai Municipal Corporation (BMC) headquarters')">
    <img src="/images/IMG_0590.JPG" alt="Mumbai Municipal Corporation (BMC) headquarters">
    <div class="caption">Mumbai Municipal Corporation (BMC) headquarters</div>
  </div>
  <div class="gallery-item" onclick="showLightbox('/images/IMG_8991.JPG','View from Aguada Fort, Goa')">
    <img src="/images/IMG_8991.jpeg" alt="View from Aguada Fort, Goa">
    <div class="caption">View from Aguada Fort, Goa</div>
  </div>
  <div class="gallery-item" onclick="showLightbox('/images/IMG_20190322_171100.jpg','Dona Paula Beach, Panaji, Goa')">
    <img src="/images/IMG_20190322_171100.jpg" alt="Dona Paula Beach, Panaji, Goa">
    <div class="caption">Dona Paula Beach, Panaji, Goa</div>
  </div>
  <div class="gallery-item" onclick="showLightbox('/images/IMG_5343.HEIC','Parade at Wagah Border')">
    <img src="/images/IMG_5343.HEIC" alt="Parade at Wagah Border">
    <div class="caption">Parade at Wagah Border</div>
  </div>
  <div class="gallery-item" onclick="showLightbox('/images/IMG_5319.HEIC','Golden Temple, Amritsar')">
    <img src="/images/IMG_5319.HEIC" alt="Golden Temple, Amritsar">
    <div class="caption">Golden Temple, Amritsar</div>
  </div>
  <div class="gallery-item" onclick="showLightbox('/images/IMG_0772.JPG','Sunset at Alibag')">
    <img src="/images/IMG_0772.JPG" alt="Sunset at Alibag">
    <div class="caption">Sunset at Alibag</div>
  </div>
  <div class="gallery-item" onclick="showLightbox('/images/IMG_3052.JPG','Murdeshwar, Karnataka')">
    <img src="/images/IMG_3052.JPG" alt="Murdeshwar, Karnataka">
    <div class="caption">Murdeshwar, Karnataka</div>
  </div>
  <div class="gallery-item" onclick="showLightbox('/images/IMG_3056.JPG','Murdeshwar, Karnataka')">
    <img src="/images/IMG_3056.JPG" alt="Murdeshwar, Karnataka">
    <div class="caption">Murdeshwar, Karnataka</div>
  </div>
</div>

<script>
function showLightbox(imgSrc, captionText) {
  document.getElementById('lightbox-img').src = imgSrc;
  document.getElementById('lightbox-img').alt = captionText;
  document.getElementById('lightbox-caption').textContent = captionText;
  document.getElementById('lightbox-overlay').classList.add('active');
}
document.getElementById('lightbox-close').onclick = function() {
  document.getElementById('lightbox-overlay').classList.remove('active');
  document.getElementById('lightbox-img').src = '';
};
// Optional: close lightbox when clicking outside the image/caption
document.getElementById('lightbox-overlay').onclick = function(e) {
  if(e.target === this) {
    this.classList.remove('active');
    document.getElementById('lightbox-img').src = '';
  }
};
</script>