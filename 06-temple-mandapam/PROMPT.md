# Prompt to regenerate this invitation

Copy everything below the line into Claude Code (or any AI coding assistant), and put the two images in an `img/` folder next to it first.

---

Build a mobile-first, single-file engagement invitation website (`index.html`, inline CSS and vanilla JS, Google Fonts allowed, no frameworks). It will be shared as a link on WhatsApp and opened on phones, so it must load fast and feel luxurious and smoothly animated.

**Details**
- Engagement of **Amitha** (bride, always named first) & **Harsha** (groom). Use the name "Harsha" only, never a surname.
- Bride's parents: Mrs. Renuka & Mr. Keshav. Groom's parents: Mrs. Lakshmi Nagamani & Mr. Ravindra Kumar.
- Sunday, 15 November 2026, 9:00 AM onwards (IST).
- Venue: SVR Convention Hall, Ponnur Rd, Lalpuram, Sangadigunta, Guntur, Andhra Pradesh 522003. Map link: https://maps.app.goo.gl/n8947P4qcDS9F5pp7
- Hashtag: #AmithaWedsHarsha. Language: English.
- **The date must not appear anywhere before the scratch card** (not on the cover, not in the link preview text).

**Look and feel**
- Palette: ivory, soft peach and blush, terracotta, rich cocoa-brown titles (keep headings dark enough to read clearly), champagne rose-gold accents (no yellow gold, no purple).
- Fonts: Parisienne for the couple's names (clear capital A), Cinzel for small caps labels, Cinzel Decorative for section titles, Cormorant Garamond for body text, Great Vibes for small script accents.
- Subtle paper texture on the background. Elegant, realistic, never cartoonish.

**Sequence**
1. **Cover:** two ivory satin doors meeting in the middle with a thin rose-gold seam. Pearl-and-lace borders run down the outer edges. "Amitha & Harsha" in embossed rose-gold script near the top. In the centre, a jewelled rose-gold locket on the seam: scalloped rose-gold frame with tiny bead highlights, a ring of pearls, a deep terracotta enamel centre with "A&H" in bright champagne script, crystals set at the four points, a pearl and crystal drop above and below, a soft breathing glow and sparkle glints. "TAP TO OPEN" pulsing at the bottom. No hanging garlands.
2. **On tap** (no auto-open, because browsers only allow sound after a tap), the doors swing open in 3D and background music `music.mp3` starts at 0:15 of the track with a soft 2-second fade-in and loops back to 0:15 (a small ♪ button bottom-right toggles it; hide the button if the file is missing).
3. **Ganesha:** `img/ganesha.webp` is a full painted scene (Ganesha on a flower-and-marigold swing under a carved arch with hanging lanterns). Show it full-screen with a slow cinematic zoom-out, flickering glows on the lanterns and rising gold sparkles, with soft ivory fades at the top and bottom for the text. Show "|| SHREE GANESHAYA NAMAH ||" at the top in solid dark cocoa with a soft light halo (fully legible, no box behind it). After a moment, the Vakratunda shloka fades in at the bottom. No tap needed: it moves on to the next page automatically about 8 seconds after the doors open.
4. **Couple:** "With the blessings of our elders", then "Amitha & Harsha" written on with a left-to-right wipe and a rose-gold shimmer. Below it, `img/couple.jpg` in an arched rose-gold frame, with glowing twinkles on the lanterns in the art. Then "ARE GETTING ENGAGED" and each name with "Daughter of / Son of" and the parents' names. Pastel petals and little flowers drift down.
5. **Welcome message:** blessings of Lord Ganesha and elders, honoured to welcome you.
6. **Scratch to Reveal:** a heart covered in peach and terracotta flowers that the guest rubs off with a finger to reveal "15 November 2026 · Sunday · 9:00 AM onwards". **If the guest doesn't scratch within 2 seconds of the heart coming into view, it scratches itself automatically.** On reveal: confetti burst, the title changes to "Our Forever Begins", and "Save the Date" (Google Calendar link) plus "Add to another calendar" (.ics download) buttons appear.
7. **Countdown** "Counting Down to Forever" (days, hours, minutes, seconds). Show "Today's the day!" on the day and a thank-you message afterwards.
8. **Venue** with the address, an embedded Google Map and a "Get Directions" button.
9. **Closing:** "Your presence and blessings will make our day complete", "With love, the families of Amitha & Harsha", the hashtag, and a small Ganesha medallion.

**Technical**
- Fade sections in on scroll. Respect `prefers-reduced-motion`.
- **Auto-scroll:** 2 seconds after the inner page appears, if the guest hasn't scrolled, gently scroll down (about 55 px/s). Pause at the scratch heart until it's revealed, then continue to the end. As soon as the guest touches, scrolls or uses the keyboard, stop auto-scrolling for good.
- Cap canvas pixel ratio at 2. Use WebP images. Keep total size small.
- Include Open Graph tags (title "Amitha & Harsha · Engagement Invitation", image `SITE_URL/preview.jpg` 1200×630: the couple art in an arched rose-gold frame beside "The Engagement of Amitha & Harsha" and "Tap to open your invitation", no date) and a comment to replace `SITE_URL` after deploying.
- Test at 360–414px phone widths.
