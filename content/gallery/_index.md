---
title: Gallery
---

## Group Photo

<section class="gallery-feature">
  <figure class="gallery-hero-card">
    <img id="gallery-hero-image" src="/img/group/2026_fall.jpg" alt="Kingsbury Lab Fall 2026 group photo">
    <figcaption id="gallery-hero-caption">Fall 2026 Group Photo</figcaption>
  </figure>
  <div class="gallery-thumbnail-carousel">
    <button class="gallery-carousel-arrow gallery-carousel-prev" type="button" aria-label="Show previous group photo" title="Previous photo">
      <i class="fas fa-chevron-left" aria-hidden="true"></i>
    </button>
    <div class="gallery-thumbnail-strip" aria-label="Group photo thumbnails">
      <button class="gallery-thumb is-active" type="button" data-src="/img/group/2026_fall.jpg" data-alt="Kingsbury Lab Fall 2026 group photo" data-caption="Fall 2026 group photo" data-position="50% 80%">
        <img src="/img/group/2026_fall.jpg" alt="Fall 2026 group photo thumbnail">
      </button>
      <button class="gallery-thumb" type="button" data-src="/img/group/2025_fall.jpg" data-alt="Kingsbury Lab Fall 2025 group photo" data-caption="Fall 2025 group photo" data-position="50% 50%">
        <img src="/img/group/2025_fall.jpg" alt="Fall 2025 group photo thumbnail">
      </button>
      <button class="gallery-thumb" type="button" data-src="/img/group/2025_spring.jpg" data-alt="Kingsbury Lab Spring 2025 group photo at AEESP" data-caption="Spring 2025 at AEESP" data-position="50% 50%">
        <img src="/img/group/2025_spring.jpg" alt="Spring 2025 group photo thumbnail">
      </button>
      <button class="gallery-thumb" type="button" data-src="/img/group/2024_fall.jpg" data-alt="Kingsbury Lab Fall 2024 group photo" data-caption="Fall 2024 group photo" data-position="50% 50%">
        <img src="/img/group/2024_fall.jpg" alt="Fall 2024 group photo thumbnail">
      </button>
      <button class="gallery-thumb" type="button" data-src="/img/group/2024_spring.jpg" data-alt="Kingsbury Lab Spring 2024 group photo" data-caption="Spring 2024 group photo" data-position="50% 50%">
        <img src="/img/group/2024_spring.jpg" alt="Spring 2024 group photo thumbnail">
      </button>
    </div>
    <button class="gallery-carousel-arrow gallery-carousel-next" type="button" aria-label="Show next group photo" title="Next photo">
      <i class="fas fa-chevron-right" aria-hidden="true"></i>
    </button>
  </div>
</section>

<script>
const galleryFeature = document.querySelector('.gallery-feature');
const thumbnailStrip = galleryFeature.querySelector('.gallery-thumbnail-strip');
const previousButton = galleryFeature.querySelector('.gallery-carousel-prev');
const nextButton = galleryFeature.querySelector('.gallery-carousel-next');

function showGalleryPhoto(button) {
  const hero = document.getElementById('gallery-hero-image');
  const caption = document.getElementById('gallery-hero-caption');
  hero.src = button.dataset.src;
  hero.alt = button.dataset.alt;
  hero.style.objectPosition = button.dataset.position || '50% 50%';
  caption.textContent = button.dataset.caption;
  galleryFeature.querySelectorAll('.gallery-thumb').forEach((thumb) => thumb.classList.remove('is-active'));
  button.classList.add('is-active');
}

galleryFeature.querySelectorAll('.gallery-thumb').forEach((button) => {
  button.addEventListener('click', () => showGalleryPhoto(button));
});

function updateGalleryArrows() {
  const maxScroll = thumbnailStrip.scrollWidth - thumbnailStrip.clientWidth;
  previousButton.disabled = thumbnailStrip.scrollLeft <= 1;
  nextButton.disabled = thumbnailStrip.scrollLeft >= maxScroll - 1;
}

function scrollGallery(direction) {
  const firstThumbnail = thumbnailStrip.querySelector('.gallery-thumb');
  const gap = parseFloat(getComputedStyle(thumbnailStrip).columnGap) || 0;
  thumbnailStrip.scrollBy({
    left: direction * (firstThumbnail.offsetWidth + gap),
    behavior: 'smooth'
  });
}

previousButton.addEventListener('click', () => scrollGallery(-1));
nextButton.addEventListener('click', () => scrollGallery(1));
thumbnailStrip.addEventListener('scroll', updateGalleryArrows, { passive: true });
window.addEventListener('resize', updateGalleryArrows);
showGalleryPhoto(galleryFeature.querySelector('.gallery-thumb.is-active'));
updateGalleryArrows();
</script>

## Group Events
