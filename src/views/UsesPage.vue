<template>
  <div class="wrapper">
    <h1>/uses</h1>
    <p>
      Here you can find some info, about what I use on everyday basis - software, hardware and some
      personal gear 😄.
    </p>
    <p>Heavily inspired by <a href="https://uses.tech/">uses.tech</a></p>
    <h2 id="hardware">#hardware</h2>
    <img
      src="https://images.ctfassets.net/5jzpzmwjn9yr/7GGC5xhl9nu57BG6WbTRmP/92dd82d87c1c33f78215b39c474df5b2/computer.jpg"
      alt="my setup"
    />
    <ul>
      <li>
        MacBook Pro 13 2020 - Intel Core i5, 16GB RAM, 512SSD - Currently my main laptop, I got from AppUnite
      </li>
      <li>
        MacBook Pro 13 2017 - no touchbar, Intel Core i5, 8GB RAM, 256SSD - My private laptop
      </li>
      <li>LG 29-WK500 21:9 2560x1080px monitor</li>
      <li>CalDigit USB-C dock</li>
      <li>Apple Magic Keyboard + Apple Magic Mouse</li>
      <li>Griffin Elevator laptop stand</li>
      <li>
        Lenovo S340 with Ryzen 3 3200U, 4GB RAM and 128SSD - My linux machine, which I also use at
        school
      </li>
    </ul>
    <h2 id="software">#software</h2>
    Code editing
    <ul>
      <li>WebStorm - My main IDE</li>
      <li>
        Vim - I try to force myself using it, but I'm not that good at using it. At least I have it
        set up
      </li>
      <li>Xcode - My second language is currently Swift</li>
    </ul>
    Terminal
    <ul>
      <li>iTerm 2</li>
      <li>oh-my-zsh</li>
      <li>spaceship-prompt</li>
    </ul>
    Other apps I use very often
    <ul>
      <li>Chrome</li>
      <li>Spotify</li>
      <li>Figma</li>
      <li>Postman</li>
      <li>XMind</li>
      <li>Rectangle - an amazing macOS app for managing windows</li>
    </ul>
    <h2 id="gear">#gear</h2>
    Recording
    <ul>
      <li>
        Behringer C1U - My microphone for recording the
        <a href="https://require.pl">Require Podcast</a>
      </li>
      <li>Behrginger UM2 audio interface</li>
      <li>
        Sony α58 + Sony 18-55mm F3.5-5.6 Lens + Sony 50mm F1.8 Lens + Tamron 70-300mm Lens - My
        camera for video projects
      </li>
      <li>
        Rode VideoMicro - Amazing on-camera microphone, with which I've recorded my first podcast
        episodes
      </li>
    </ul>
    Personal stuff
    <ul>
      <li>iPhone XR 64GB (PRODUCT)<sup>RED</sup></li>
      <li>Focus JAM 6.9 Mountain Bike</li>
    </ul>
    <h2 id="setup">#setup</h2>
    <details>
      <summary>VSCode Setup</summary>
      <ul>
        <li>Font: JetBrains Mono, 14</li>
        <li>Theme: Material Deep Ocean</li>
        <li>
          Nice plugins I have:
          <ul>
            <li>Vetur - best Vue support plugin</li>
            <li>Snipsnap - amazing plugin for code snippets</li>
            <li>React PropTypes Generate - nice helper at everyday work</li>
            <li>Polacode - beautiful code screenshots</li>
            <li>Markdown Preview Github Styling - how this isn't natively implemented yet?</li>
            <li>Go - Go</li>
            <li>Discord Presence - discord swag</li>
            <li>Colorize - better looking CSS colors preview in editor</li>
            <li>Bracket Pair Colorizer 2 - Nice extension, that helps you read the code</li>
            <li>Backticks - automatically convert the string to backticks when needed in JS</li>
          </ul>
        </li>
      </ul>
    </details>
    <details>
      <summary>Terminal Setup</summary>
      <ul>
        <li>Font: JetBrains Mono, 14</li>
        <li>Theme: Nord</li>
        <li>Emulator: iTerm 2</li>
        <li>
          ZSH Setup:
          <ul>
            <li>oh-my-zsh</li>
            <li>zsh-autosuggestions</li>
            <li>zsh-syntax-highlighting</li>
            <li>Pure prompt</li>
            <li>nvm</li>
          </ul>
        </li>
      </ul>
    </details>
    <details>
      <summary>Linux Setup</summary>
      <p>
        Available on my GitHub -
        <a href="https://github.com/AdamSiekierski/dotfiles-arch">dotfiles-arch</a>
      </p>
    </details>
  </div>
</template>
<style lang="scss" scoped>
@use "../styles/mixins.scss" as mixins;

.wrapper {
  padding: 50px 25px;
  min-height: 100vh;
  max-width: 800px;
  margin: 0 auto;
}

a {
  @include mixins.themed() using ($theme) {
    color: map-get($theme, "fg");
  }
}

img {
  width: 100%;
}
</style>
