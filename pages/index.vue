<template>
  <section class="section">
    <div class="container">
    <div class="columns is-centered">
      <div class="column is-6">
        <div class="card">
            <div class="card-image">
              <figure class="image is-4by3">
                <img src="~assets/photo.png" alt="Где фотка, ёпта?">
              </figure>
            </div>
            <div class="card-content">
              <RansomNote class="title" text='Привет!'/>
              <RansomNote class="title" text='Я Вова Серёгин'/>
              <p>Я — «немного».</p>
              <p>Немного программирую на python (django) и javascript (vue.js). Буквы сверху — работа моего <a href="https://github.com/heaviss/ransomnote">ransomnote</a>.</p>
              <br>
              <p>Немного сочиняю музыку, учусь играть на гитаре и губной гармошке.</p>
              <br>
              <p>Немного пишу (в <a href="https://t.me/rdpms">телеграм-канал</a>, занял 9 место на <a href="https://challenge.glvrd.ru/mtv.html">вызове Главреда</a>).</p>
              <br>
              <p>Много читаю, потому что люблю (45 книг в 2016, <a href="telegra.ph/thisage--26-02-19">31 в 2017</a>). Читаю про разработку, дизайн, редактуру, устройство людей, рациональное мышление и сочинение музыки. И фантастику.</p>
              <br>
              <p>Веду с Верой Иноземцевой <a href="https://t.me/listen2it">канал «Слушай чё»</a>, где она читает вслух клёвые статьи.</p>
              <br>
              <p>Сейчас работаю безопасником в ЦФТ.</p>
            </div>
            <footer class="card-footer">
              <p class="card-footer-item">
                <span>
                  <a href="https://t.me/heavis">Telegram</a>
                </span>
              </p>
              <p class="card-footer-item">
                <span>
                  <a href="https://github.com/heaviss/">Github</a>
                </span>
              </p>
            </footer>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import RansomNote from 'ransomnote';
export default {
  components: {
    RansomNote
  },
}
</script>

<style lang="scss">
.title
{
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
}

.links
{
  padding-top: 15px;
}
</style>
