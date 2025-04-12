<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Redirecting...</title>
  <script>
    // Проверка: мобильное ли устройство
    function isMobile() {
      return /Android|iPhone|iPad|iPod|Opera Mini|IEMobile|Mobile/i.test(navigator.userAgent);
    }

    window.onload = function () {
      const offers = [
        "https://grzvkg.trueamouronline.com/?utm_source=da57dc555e50572d&ban=tiktok&j1=1&s1=212364&s2=2121035", // оффер 1
        "https://mb9pmr0.vipsthelovehaven.com/lw4h4aw?s1=testTT", // оффер 2
        "https://mb9pmr0.meethotlove.com/lwyrlwm?s1=testTT2", // оффер 3
        "https://prev.affomelody.com/VgeE8p"  // оффер 4
      ];

      const desktopRedirect = "https://www.instagram.com/men.click_here0?igsh=d2tleGZ1MzE1eGV4"; // для десктопа

      if (isMobile()) {
        // случайный оффер из 4 (равномерно)
        const randomOffer = offers[Math.floor(Math.random() * offers.length)];
        window.location.href = randomOffer;
      } else {
        // редирект для ПК
        window.location.href = desktopRedirect;
      }
    };
  </script>
</head>
<body>
  <p>Переход на оффер...</p>
</body>
</html>
