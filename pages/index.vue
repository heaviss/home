<template>
  <article class="homepage">
    <RansomNote class="homepage__hi ransomenote" text="Привет!" />
    <img class="homepage__photo" src="~assets/photo.png" alt="Где фотка, ёпта?">
    <RansomNote class="homepage__name ransomenote" text="Я Вова Серёгин" />
    <section class="homepage__about">
      <p>Программирую на python (django) и javascript (vue.js). Буквы сверху — работа моего <a href="https://github.com/heaviss/ransomnote">ransomnote</a>.</p>
      <p>Люблю читать (45 книг в 2016, <a href="https://telegra.ph/thisage--26-02-19">31 в 2017</a>). Читаю про разработку, дизайн, редактуру, устройство людей, рациональное мышление и сочинение музыки. И фантастику.</p>
      <p>Люблю музыку, учусь играть на гитаре и губной гармошке.</p>
      <p>Веду блог в телеграме: https://t.me/rdpms. 8 читателей, У — успех.</p>
      <p>Мечтаю дожить до 200, пытаюсь придумать, как.</p>
      <p>Работал безопасником в ЦФТ, сейчас — программирую и борюсь с синдромом самозванца в ГдеМатериале.</p>
    </section>

    <section class="homepage__contacts">
      <p class="card-footer-item">
        <a href="https://t.me/heavis">Telegram</a>
      </p>
      <p class="card-footer-item">
        <a href="https://github.com/heaviss/">Github</a>
      </p>
    </section>
  </article>
</template>

<script>
import RansomNote from 'ransomnote';
export default {
  components: {
    RansomNote
  },
}
</script>

<style>
.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
}

.links {
  padding-top: 15px;
}

.homepage {
  font-size: 1em;

  width: 100vw;
  height: 100vh;
}

@media (width > 1024px) {
  .homepage {
    display: grid;
    grid-template-columns: repeat(12, 1fr);
    grid-auto-rows: 1fr;
  }
}

.ransomenote {
  font-size: 1.5em;
}

@media (width > 1024px) {
  .ransomenote {
    font-size: 2em;
  }
}

.homepage__hi {
  grid-column: 3 / 5;
  grid-row: 3 / 4;
}

.homepage__photo {
  grid-column: 4 / 8;
  grid-row: 2 / 8;
  max-width: 100%;
}

.homepage__name {
  grid-column: 7 / 9;
  grid-row: 5 / 6;
}

.homepage__about {
  grid-column: 4 / 8;
  grid-row: 9 / 13;
}

.homepage__about p {
  margin-bottom: 1em;
}

.homepage__contacts {
  grid-column: 4 / 8;
  grid-row: 14 / 15;
}
</style>
