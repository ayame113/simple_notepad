# simple_notepad
Notepad that runs on your browser

```
data:text/html,<html><head><title>memo</title><script>window.addEventListener('beforeunload',event=>{event.preventDefault();event.returnValue=''})</script></head><body style="margin:0;"><textarea autofocus placeholder="hello world" style="width:100%;height:100%;font-size:2em;padding:0.5em;" oninput="document.title=this.value||'memo'"></textarea></body></html>
```

```html
<html>
  <head>
    <title>memo</title>
    <script>
      window.addEventListener('beforeunload', (event) => {
        event.preventDefault();
        event.returnValue = '';
      })
    </script>
  </head>
  <body style="margin:0;">
    <textarea
      autofocus
      placeholder="hello world"
      style="width:100%;height:100%;font-size:2em;padding:0.5em;"
      oninput="document.title=this.value||'memo'"
    ></textarea>
  </body>
</html>
```
