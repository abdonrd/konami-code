[![Build status][travis-image]][travis-url]
[![Published on webcomponents.org][webcomponents-image]][webcomponents-url]

## \<konami-code\>

Web Component (with Polymer) to listen the Konami Code (↑↑↓↓←→←→BA).

Example:
<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="konami-code.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<konami-code></konami-code>
<p>Type the Konami Code to launch the easter egg.</p>

<script>
  var konamiCode = document.querySelector('konami-code');
  konamiCode.addEventListener('code-completed', function(event) {
    alert('Easter egg!');
  });
</script>

<!--
You also can use the Polymer annotated event listener setup:
<konami-code on-code-completed="_launchEasterEgg"></konami-code>
-->
```

[travis-image]: https://travis-ci.org/abdonrd/konami-code.svg?branch=master
[travis-url]: https://travis-ci.org/abdonrd/konami-code
[webcomponents-image]: https://img.shields.io/badge/webcomponents.org-published-blue.svg
[webcomponents-url]: https://beta.webcomponents.org/element/abdonrd/konami-code
