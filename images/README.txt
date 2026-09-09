JHIDE — animated prototype : image folder
=========================================

VERSIONS
  index.html                         current — v1.2 (colour hero)
  versions/index-v1.1-monochrome.html v1.1 — fully black & white
  Both open the same way. To show v1.1, just open that file.

COLOUR RULES (v1.2)
  class="tint"  photo stays in full colour, always
  class="mono"  photo is black & white, turns colour on hover —
                and automatically on the active process step

  In full colour : hero pair (flatlay + needle), material close-up
  Black & white  : product cards, process steps, material inset
  Swap one class for the other on any <img> to change a photo.

FILES IN USE
  collection-flatlay.jpg      hero (large, COLOUR) + Belt No. 05 card
  needle-and-thread.jpg       hero (small inset, COLOUR)
  machine-needle-detail.jpg   material section (large, COLOUR)
  leather-hide-grain.jpg      process 01 + Swatch Set card
  thread-spools-crate.jpg     process 02 + Thread & Care Kit card
  stitching-by-hand.jpg       process 03
  bifold-wallet-in-hand.jpg   process 04 + Bifold No. 01 card
  card-holder-tan.jpg         Card Holder No. 02 card
  atelier-sewing-machine.jpg  material inset + Bespoke card

TO REPLACE A PHOTO
  Easiest: save your new photo over the existing filename above.
  Otherwise: edit the PRODUCTS list at the bottom of index.html
  for product cards, or the <img src="..."> tags in the hero /
  process / material sections.

SUGGESTED CROPS
  Products & process : 4:5 portrait, ~1200x1500px
  Hero large         : 4:5 portrait
  Material inset     : 1:1 square
