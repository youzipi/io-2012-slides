title: Slide Title
class: image

![Mobile vs desktop users](images/google_developers_icon_128.png)

---

title: Agenda
class: big

Things we'll cover:

- Bullet1
- Bullet2
- Bullet3

---

title: Today
class: nobackground fill

![Many kinds of devices.](images/google_developers_icon_128.png)

<footer class="source">source: place source info here</footer>

---

h1: Big Title Slide
class: title-slide

---

title: Code Example

Media Queries are sweet:

<pre class="prettyprint" data-lang="css">
@media screen and (max-width: 640px) {
  #sidebar { display: none; }
}
</pre>

---

title: Once more, with JavaScript

<pre class="prettyprint" data-lang="javascript">
function isSmall() {
  return window.matchMedia("(min-device-width: ???)").matches;
}

function hasTouch() {
  return Modernizr.touch;
}

function detectFormFactor() {
  var device = DESKTOP;
  if (hasTouch()) {
    device = isSmall() ? PHONE : TABLET;
  }
  return device;
}
</pre>
