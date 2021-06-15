<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="preconnect" href="https://fonts.gstatic.com" />
    <link
      href="https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,300;0,400;0,700;0,900;1,300;1,400;1,700;1,900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
    <title>Document</title>
  </head>
  <body>
    <!-- Navbar -->
    <header>
      <nav class="navbar">
        <div class="navbar__brand">
          <img src="./assets/logo.png" alt="logo" class="navbar__logo" />
        </div>
        <div class="navbar__nav__items">
          <div class="nav__item">
            <button class="button__primary hide__mobile">Order Food</button>
            <button
              class="button__primary hamburger__menu mobile__only"
              id="hamburgermenu"
            >
              <div></div>
              <div></div>
              <div></div>
            </button>
          </div>
        </div>
      </nav>
      <div class="mobile__navbar__items mobile__only hamburger__menu__close">
        <ul>
          <li class="nav__item">Products</li>
          <li class="nav__item">Restaurants</li>
          <li class="nav__item">Pricing</li>
          <li class="nav__item">About Us</li>
        </ul>

        <div class="nav__item">
          <button class="button__primary">Order Food</button>
        </div>
      </div>
    </header>
    <main class="container">
      <!-- Hero Section -->
      <section class="hero__container">
        <div class="hero__image__container">
          <img class="hero__image" src="./assets/hero.jpg" alt="hero image" />
          <img
            src="./assets/svg/heroShape.svg"
            alt="hero image shape"
            class="hero__image__shape"
          />
          <img
            src="./assets/svg/herobgpattren.svg"
            alt="hero image shape"
            class="hero__image__pattren"
          />
        </div>
        <div class="hero__description">
          <h1 class="hero__text">
            Order food from favourite restaurants near you.
          </h1>
          <button class="button__primary">Order now</button>
        </div>
      </section>

      <!--Video Footage-->
      <section class="video__footage__container">
        <div class="video__footage">
          <iframe
            src="https://player.vimeo.com/video/323795266"
            frameborder="0"
            allow="autoplay; fullscreen; picture-in-picture"
            allowfullscreen
            class="chef__video"
          ></iframe>
        </div>
        <div class="video__footage__text">
          <p>
            Your food will be prepared safely with an experienced chef, without
            compromising on the quality and hygiene.
          </p>
        </div>
      </section>

      <!-- Explore Menu -->
      <section class="explore__menu__container">
        <h1 class="explore__menu__text">Explore Our Menu</h1>
        <div class="explore__menu__gradient__bg"></div>
        <div class="explore__menu__lists">
          <!-- Burger -->
          <div class="food__menu__card">
            <img src="./assets/burger.jpg" alt="burger" class="food__image" />
            <div class="food__menu__card__description">
              <h3 class="food__title">Burgers</h3>
              <p class="food__restaurants">
                Burger King, Mcdonalds, Burger Place
                <span style="color: red"> +3</span>
              </p>
            </div>
          </div>
          <!-- Pizza -->
          <div class="food__menu__card" id="pizza__card">
            <img src="./assets/pizza.jpg" alt="pizza" class="food__image" />
            <div class="food__menu__card__description">
              <h3 class="food__title">Pizza</h3>
              <p class="food__restaurants">
                Pizza Hut, Domino's Pizza
                <span style="color: red"> +3</span>
              </p>
            </div>
          </div>
          <!-- Ice Cream -->
          <div class="food__menu__card">
            <img
              src="./assets/iceCream.jpg"
              alt="ice cream"
              class="food__image"
            />
            <div class="food__menu__card__description">
              <h3 class="food__title">Ice Creams</h3>
              <p class="food__restaurants">
                Baskin Robins, Ibaco
                <span style="color: red"> +3</span>
              </p>
            </div>
          </div>
        </div>
        <div class="explore__menu__view__more">
          <button class="button__primary">View More</button>
        </div>
      </section>

      <!-- Restaurants -->
      <section class="restaurants__container">
        <div class="restaurant__text">
          <h4 class="restaurants__description">Order From 100s of restaurants</h4>
        </div>
        <div class="restaurants__flex">
          <div class="restaurants__flex__row__one">
            <div class="restaurant__1">
              <img
                class="restaurant__1__image"
                src="./assets/restaurant1.jpg"
                alt="restaurant__1"
              />
            </div>
            <div class="restaurant__2">
              <img
                class="restaurant__2__image"
                src="./assets/restaurant2.jpg"
                alt="restaurant__2"
              />
            </div>
          </div>
          <div class="restaurants__flex__row__two">
            <div class="restaurant__3">
              <img
                class="restaurant__3__image"
                src="./assets/restaurant3.jpg"
                alt="restaurant__3"
              />
            </div>
            <div class="restaurant__4">
              <img
                class="restaurant__4__image"
                src="./assets/restaurant4.jpg"
                alt="restaurant__4"
              />
            </div>
          </div>
        </div>
      </section>
      <section class="email__subscribe__container">
        <div class="update">
          <h1 class="text__1">Stay Updated</h1>
          <div class="email__field">
            <div>
              <input type="email" placeholder="xyz@email.com" class="email__input">
            </div>
            <button class="button__primary">Get Updates</button>
          </div>
        </div>
      </section>

      <!--Quote-->
      <section class="quote__container">
        <div class="quote_image_overlay"></div>
        <h3 class="quote_image_text">
          When a man's stomach is full it makes no difference whether he is rich
          or poor.
        </h3>
      </section>
     </main>
    <footer>
      <img src="./assets/logo.png" alt="logo">
      <ul>
        <li>Pricing</li>
        <li>Terms and condition</li>
        <li>Partnership</li>
        <li>Career</li>
        <li>Contact</li>
      </ul>
    </footer>
    <script>
      const hamburgermenu = document.getElementById("hamburgermenu");
      const mobileNavDropDown = document.querySelector(
        ".mobile__navbar__items"
      );
      window.addEventListener("click", () => {
        if (mobileNavDropDown.classList.contains("hamburger__menu__close"))
          return mobileNavDropDown.classList.remove("hamburger__menu__close");
        return mobileNavDropDown.classList.add("hamburger__menu__close");
      });
    </script>
  </body>
</html>
