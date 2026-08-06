---
title: Gallery
---

## Group Photo

<section class="gallery-feature">
  <figure class="gallery-hero-card">
    <img id="gallery-hero-image" src="/img/group/2025_fall.jpg" alt="Kingsbury Lab Fall 2025 group photo">
    <figcaption id="gallery-hero-caption">Fall 2025 Group Photo</figcaption>
  </figure>
  <div class="gallery-thumbnail-strip" aria-label="Group photo thumbnails">
    <button class="gallery-thumb is-active" type="button" data-src="/img/group/2025_fall.jpg" data-alt="Kingsbury Lab Fall 2025 group photo" data-caption="Fall 2025">
      <img src="/img/group/2025_fall.jpg" alt="Fall 2025 group photo thumbnail">
    </button>
    <button class="gallery-thumb" type="button" data-src="/img/group/2025_spring.jpg" data-alt="Kingsbury Lab Spring 2025 group photo at AEESP" data-caption="Spring 2025">
      <img src="/img/group/2025_spring.jpg" alt="Spring 2025 group photo thumbnail">
    </button>
    <button class="gallery-thumb" type="button" data-src="/img/group/2024_fall.jpg" data-alt="Kingsbury Lab Fall 2024 group photo" data-caption="Fall 2024">
      <img src="/img/group/2024_fall.jpg" alt="Fall 2024 group photo thumbnail">
    </button>
    <button class="gallery-thumb" type="button" data-src="/img/group/2024_spring.jpg" data-alt="Kingsbury Lab Spring 2024 group photo" data-caption="Spring 2024">
      <img src="/img/group/2024_spring.jpg" alt="Spring 2024 group photo thumbnail">
    </button>
  </div>
</section>

<script>
document.querySelectorAll('.gallery-thumb').forEach((button) => {
  button.addEventListener('click', () => {
    const hero = document.getElementById('gallery-hero-image');
    const caption = document.getElementById('gallery-hero-caption');
    hero.src = button.dataset.src;
    hero.alt = button.dataset.alt;
    caption.textContent = button.dataset.caption;
    document.querySelectorAll('.gallery-thumb').forEach((thumb) => thumb.classList.remove('is-active'));
    button.classList.add('is-active');
  });
});
</script>

## Group Events
