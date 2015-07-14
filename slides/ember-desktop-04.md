# Code things!
NW.js has APIs for native UI controls.
```
const fileMenu = new gui.MenuItem({
  label: 'Save',
  key: 's',
  modifiers: env.ctrlKey,

  click() {
    this.sendAction('fileSave');
  }
});
```
