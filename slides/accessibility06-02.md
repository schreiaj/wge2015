###Focus on the element that's being changed ("outlet")
<pre><code class="javascript">
Ember.Route.reopen({
  focus(morph) {
    var elem = morph.firstNode;

    try {
      if (!elem.getAttribute('tabindex')) {
        if (isInteractive(elem)) {
          elem.setAttribute('tabindex', 0);
        } else {
          elem.setAttribute('tabindex', -1);
        }
      }

      elem.focus();
    } catch (e) {}
  }
</code></pre>
