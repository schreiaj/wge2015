###Call it when we handle the transition
<pre><code class="javascript">
enter(transition) {
    var route = this;

    if (transition.pivotHandler && this.routeName == transition.pivotHandler.routeName + '.index') {
      transition.pivot = transition.pivotHandler.routeName;
      route = transition.pivotHandler;
      this._focus(route, transition);
    }

    if (!transition.pivot) {
      transition.pivot = this.routeName;
      this._focus(route, transition)
    }

    return this._super(...arguments);
  }
</code></pre>