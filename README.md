# google-analytics-template
Simple template to kickstart your google analytics projects.

```html
<!DOCTYPE html>
<html lang="en">

<head>
 <meta charset="UTF-8">
 <meta http-equiv="X-UA-Compatible" content="IE=edge">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Google Analytics Example</title>
 <script
  src="https://code.jquery.com/jquery-3.6.0.min.js"
  integrity="sha256-/xUj+3OJU5yExlq6GSYGSHk7tPXikynS7ogEvDej/m4="
  crossorigin="anonymous"></script>
<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-MSPR2488QB"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-MSPR2488QB');
</script>
</head>

<body>
 <button>Click to Send an Event!</button>

 <script type="text/javascript">

  $('button').on('click', () => {
   sendGaEvent('Event Button Clicked!');
  });

  // Send Event Template
  function sendGaEvent(e) {
   gtag('event', e, {
    'event_category': 'Example Button',
    'event_label': 'Example page'
   });
  }
 </script>
</body>

</html>
```
