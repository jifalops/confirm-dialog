[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/jifalops/confirm-dialog)

# confirm-dialog
A simple paper-dialog wrapper.

## Installation
```
bower install --save confirm-dialog
```

 <!--## Usage-->



## Demo
<!--
```
<custom-element-demo height="400">
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="confirm-dialog.html">
    <next-code-block></next-code-block>
    <script>
      var dialog = document.getElementById('dialog');
      var heading = document.getElementById('heading');
      var body = document.getElementById('body');
      var confirm = document.getElementById('confirm');
      var cancel = document.getElementById('cancel');
      var delay = document.getElementById('delay');
      var modal = document.getElementById('modal');
      var withBackdrop = document.getElementById('withBackdrop');
      var feedback = document.getElementById('feedback');

      var htmlContent = document.getElementById('htmlContent');
      var div = document.createElement('div');
      Polymer.dom(dialog).appendChild(div);

      dialog.addEventListener('result', function(e) {
        feedback.innerText += ', on-result: ' + e.detail;
      });

      function show() {
        div.innerHTML = htmlContent.value;
        dialog.heading = heading.value;
        dialog.body = body.value;
        dialog.confirm = confirm.value;
        dialog.cancel = cancel.value;
        dialog.delay = Number(delay.value);
        dialog.modal = modal.checked;
        dialog.withBackdrop = withBackdrop.checked;
        dialog.onResult = function(result) { feedback.innerText = "onResult("+result+")"; };
        dialog.show();
      }
      function showWithProperties() {
        div.innerHTML = htmlContent.value;
        dialog.show({
          heading: heading.value,
          body: body.value,
          confirm: confirm.value,
          cancel: cancel.value,
          delay: Number(delay.value),
          modal: modal.checked,
          withBackdrop: withBackdrop.checked,
          onResult: function(result) { feedback.innerText = "onResult("+result+")"; }
        });
      }
    </script>
  </template>
</custom-element-demo>
```
-->

```html
<confirm-dialog id="dialog"></confirm-dialog>
<input id="heading" placeholder="heading" value="Heading"/><br/>
<input id="body" placeholder="body" value="Are you sure?"/><br/>
<input id="htmlContent" placeholder="html content" value="<i>Content Slot</i>"/><br/>
<input id="confirm" placeholder="confirm button" value="Confirm"/><br/>
<input id="cancel" placeholder="cancel button" value="Cancel"/><br/>
<input id="delay" placeholder="delay (ms)" value="1000"/><br/>
<label><input id="modal" type="checkbox"/>Modal</label><br/>
<label><input id="withBackdrop" type="checkbox" checked/>With backdrop</label><br/>
<button onclick="show()">Show</button>&nbsp;
<button onclick="showWithProperties()">Show with properties</button><br/>
Last Event: <span id="feedback"></span>
```

Full demo:
[webcomponents.org](https://www.webcomponents.org/element/jifalops/confirm-dialog/demo/demo/index.html)
| [github](https://jifalops.github.io/confirm-dialog/components/confirm-dialog/demo/).

API: [webcomponents.org](https://www.webcomponents.org/element/jifalops/confirm-dialog/confirm-dialog)
| [github](https://jifalops.github.io/confirm-dialog).

## Contributing

1. Fork it on Github.
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## License

[MIT](https://opensource.org/licenses/MIT)
