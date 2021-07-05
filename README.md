# google-analytics-template
Simple template to kickstart your google analytics projects.

'''
<!DOCTYPE html>
<html lang="en">

<head>
 <meta charset="UTF-8">
 <meta http-equiv="X-UA-Compatible" content="IE=edge">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Your page title</title>
 <!-- Global site tag (gtag.js) - Google Analytics -->
 <script async src="https://www.googletagmanager.com/gtag/js?id=G-Z98VWMMS1C"></script>
 <script>
  window.dataLayer = window.dataLayer || [];

  function gtag() {
   dataLayer.push(arguments);
  }
  gtag('js', new Date());
  gtag('config', 'G-Z98VWMMS1C');
 </script>
</head>

<body>
 <script type="text/javascript">

  $(yourElement).on(function() {
   sendGaEvent('Your Event')
  })

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
'''
