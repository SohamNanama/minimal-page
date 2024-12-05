
<!DOCTYPE html>
<html>

<head>
  <!--
    If you are serving your web app in a path other than the root, change the
    href value below to reflect the base path you are serving from.

    The path provided below has to start and end with a slash "/" in order for
    it to work correctly.

    Fore more details:
    * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/base
  -->
  <base href="/">
  
  <meta charset="UTF-8">
  <meta content="IE=Edge" http-equiv="X-UA-Compatible">
  <meta name="description" content="A Selft taught flutter developer, technical writer and open source contributor.">

  <!-- iOS meta tags & icons -->
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black">
  <meta name="apple-mobile-web-app-title" content="folio">
  <link rel="apple-touch-icon" href="icons/Icon-192.png">

  <!-- Favicon -->
  <link rel="icon" type="image/png" href="favicon.png" />

  <title>Monang Champaneri</title>
  <link rel="manifest" href="manifest.json">

  <style>
    .lds-ripple {
      display: inline-block;
      position: relative;
      width: 80px;
      height: 80px;
    }

    .lds-ripple div {
      background-color: #e64230;
      position: absolute;
      border: 4px solid #fff;
      opacity: 1;
      border-radius: 50%;
      animation: lds-ripple 1s cubic-bezier(0, 0.2, 0.8, 1) infinite;
    }

    .lds-ripple div:nth-child(2) {
      animation-delay: -0.5s;
    }

    @keyframes lds-ripple {
      0% {
        top: 36px;
        left: 36px;
        width: 0;
        height: 0;
        opacity: 1;
      }

      100% {
        top: 0px;
        left: 0px;
        width: 72px;
        height: 72px;
        opacity: 0;
      }
    }

    .container {
      height: 100%;
    }

    .center {
      margin: 0;
      position: absolute;
      top: 50%;
      left: 50%;
      -ms-transform: translate(-50%, -50%);
      transform: translate(-50%, -50%);
    }
  </style>

</head>

<body>


  <div class="container">
    <div class="center">
      <div class="lds-ripple">
        <div></div>
        <div></div>
      </div>
    </div>
  </div>
  <!-- This script installs service_worker.js to provide PWA functionality to
       application. For more information, see:
       https://developers.google.com/web/fundamentals/primers/service-workers -->
  <script>
    if ('serviceWorker' in navigator) {
      window.addEventListener('flutter-first-frame', function () {
        navigator.serviceWorker.register('flutter_service_worker.js?v=1936427080');
      });
    }
  </script>
  <script src="main.dart.js" type="application/javascript"></script>
</body>

</html>
