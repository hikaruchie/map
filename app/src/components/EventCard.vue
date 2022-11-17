<template>
  <!-- TODO: イベント詳細画面のデザインは Figma に寄せる -->
  <div id="contet">
    <div class="sample">
      <ul>
        <li class="card-group">
          <div class="card">
            <a
              class="card-link"
              target="_blank"
              href="https://infomotion.co.jp/sample-event"
            >
              <div class="card-title">第1回目 黒カレーフェスティバル</div>

              <div class="card-img">
                <img
                  src="https://infomotion.co.jp/wp-content/uploads/2020/04/curry.jpg"
                  class="card-img-src"
                  height="69"
                />
              </div>

              <div class="card-info">
                <div class="card-info-box">
                  <i class="fa-regular fa-calendar-days card-info-box-logo"></i>
                  <div class="card-info-box-text">
                    2022年9月21日(水)～11月6日(日)
                  </div>
                </div>

                <div class="card-info-box">
                  <i class="fa-regular fa-clock card-info-box-logo"></i>
                  <div class="card-info-box-text">10:00-19:00</div>
                </div>

                <div class="card-info-box">
                  <i class="fa-solid fa-location-dot card-info-box-logo"></i>
                  <div class="card-info-box-text">Impact HUB Tokyo</div>
                </div>

                <div class="card-info-category">
                  グルメ / ファミリー / その他
                </div>
              </div>
            </a>
          </div>

          <div class="card">
            <a
              class="card-link"
              target="_blank"
              href="https://infomotion.co.jp/sample-event"
            >
              <div class="card-title">第1回目 黒カレーフェスティバル</div>

              <div class="card-img">
                <img
                  src="https://infomotion.co.jp/wp-content/uploads/2020/04/curry.jpg"
                  class="card-img-src"
                  height="69"
                />
              </div>

              <div class="card-info">
                <div class="card-info-box">
                  <i class="fa-regular fa-calendar-days card-info-box-logo"></i>
                  <div class="card-info-box-text">
                    2022年9月21日(水)～11月6日(日)
                  </div>
                </div>

                <div class="card-info-box">
                  <i class="fa-regular fa-clock card-info-box-logo"></i>
                  <div class="card-info-box-text">10:00-19:00</div>
                </div>

                <div class="card-info-box">
                  <i class="fa-solid fa-location-dot card-info-box-logo"></i>
                  <div class="card-info-box-text">Impact HUB Tokyo</div>
                </div>

                <div class="card-info-category">
                  グルメ / ファミリー / その他
                </div>
              </div>
            </a>
          </div>

          <div class="card">
            <a
              class="card-link"
              target="_blank"
              href="https://infomotion.co.jp/sample-event"
            >
              <div class="card-title">第1回目 黒カレーフェスティバル</div>

              <div class="card-img">
                <img
                  src="https://infomotion.co.jp/wp-content/uploads/2020/04/curry.jpg"
                  class="card-img-src"
                  height="69"
                />
              </div>

              <div class="card-info">
                <div class="card-info-box">
                  <i class="fa-regular fa-calendar-days card-info-box-logo"></i>
                  <div class="card-info-box-text">
                    2022年9月21日(水)～11月6日(日)
                  </div>
                </div>

                <div class="card-info-box">
                  <i class="fa-regular fa-clock card-info-box-logo"></i>
                  <div class="card-info-box-text">10:00-19:00</div>
                </div>

                <div class="card-info-box">
                  <i class="fa-solid fa-location-dot card-info-box-logo"></i>
                  <div class="card-info-box-text">Impact HUB Tokyo</div>
                </div>

                <div class="card-info-category">
                  グルメ / ファミリー / その他
                </div>
              </div>
            </a>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.sample ul {
  display: flex;
  max-width: 1600px; /* 最大幅 */
  min-width: 240px; /* 最小幅 */
  overflow-x: scroll;
  margin: 0;
  padding: 0;
}

.sample li {
  min-width: 40%;
  margin: 50px;
  padding: 0;
  list-style: none;
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: flex-start;
}

.card-group {
  margin-left: auto;
  margin-right: auto;
  max-width: 640px;
  width: 90%;
  height: auto;
}

.card-group > :nth-child(n) {
  margin-left: 20px;
}

.card {
  box-shadow: rgb(143 172 162 / 40%) 0px 8px 20px;
  border-radius: 2px;
  color: rgb(40, 40, 40);
  padding: 12px 16px;
  background-color: white;
  transition-duration: 1s;
}

.card:hover {
  box-shadow: rgb(143 172 162 / 40%) 0px 8px 20px;
  border-radius: 2px;
  color: rgb(40, 40, 40);
  padding: 12px 16px;
  background-color: white;
  transform: translateY(-20px) translateX(-5px);
  transition: 0.4s ease-out;
}

.card-title {
  font-size: 14px;
  line-height: 22px;
  letter-spacing: 0.48px;
  font-weight: bold;
  text-overflow: ellipsis;
  white-space: nowrap;
  overflow: hidden;
  margin-bottom: 4px;
}

.card-img {
}

.card-img-src {
}

.card-info {
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  -webkit-flex-direction: column;
  -ms-flex-direction: column;
  flex-direction: column;
  overflow: hidden;
  padding: 4px 0;
  height: 69px;
}

.eWBWcX {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: contain;
}

.card-info-box {
  display: flex;
  -webkit-box-align: center;
  align-items: center;
  overflow: hidden;
  height: 20px;
  margin-bottom: 4px;
}

.card-info-box-logo {
  width: 16px;
  height: 16px;
  margin-right: 7px;
}

.card-info-box-text {
  font-size: 12px;
  line-height: 14px;
  letter-spacing: 0.39px;
  text-overflow: ellipsis;
  white-space: nowrap;
  overflow: hidden;
}

.card-info-category {
  font-size: 12px;
  line-height: 18px;
  letter-spacing: 0.39px;
  text-overflow: ellipsis;
  overflow: hidden;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
}
.card-link {
}
</style>
