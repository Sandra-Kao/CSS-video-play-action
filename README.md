# CSS-video-play-action
Please see Codepen:

https://codepen.io/K-SY/pen/mdWOBYy

```css
:root {
  --color-gray-darker: #787878;
  --gray-darkest: #323233;
  --vivid-blue-darker: #006498;
  --vivid-blue-lightest: #daeef9;

  --color-white: #ffffff;
  --color-black: #000000;
  --color-black-50: rgba(0, 0, 0, 0.5);

  --color-blue-light: #48ace1;
  --color-blue: #008cd6;
  --color-blue-darker: #006498;

  --color-gray-lighter: #e2e2e2;
  --color-gray-light: #d5d5d5;
  --color-gray-base: #c5c5c5;
  --color-gray-darker: #787878;

  --color-primary-base: #6b44cc;
}

* {
  margin: 0;
  padding: 0;
}

.overview-block {
  padding: 50px 0px;
}

.overview-block__title {
  font-size: 32px;
  font-weight: bold;
  margin-bottom: 12px;
  line-height: 1.75;
  color: var(--color-dark);
}

.overview-block__content {
  margin-bottom: 24px;
  display: flex;
}

.overview-block__content--discription {
  font-size: 16px;
  color: var(--color-grey-darker);
  float: left;
  margin-right: 20px;
}

.overview-block__wrapper {
  position: relative;
  width: 500px;
  height: 300px;
  background-repeat: no-repeat;
  background-image: url(https://cdn.pixabay.com/photo/2015/03/26/09/47/sky-690293__340.jpg);
}

.overview-block__img {
  border-radius: 4px;
}

.overview-block__play {
  width: 56px;
  height: 56px;
  border: 0px;
  border-radius: 100px;
  color: var(--color-white);
  background-color: var(--color-white);
  position: absolute;
  transform: translate(-50%, -50%);
  top: 50%;
  left: 50%;
}

.overview-block__play::before {
  content: "";
  display: inline-block;
  height: 100%;
  width: 100%;
  border: 0px;
  border-radius: 100px;
  position: absolute;
  background-color: var(--color-white);
  top: 0;
  right: 0;
  animation: halo 2s infinite;
}

.overview-block__play:hover::before {
  animation: halo 2s infinite;
}

.overview-block__play-action {
  width: 56px;
  height: 56px;
  border: 0px;
  border-radius: 100px;
  background-color: var(--color-primary-base);
  position: absolute;
  transform: translate(-50%, -50%);
  top: 50%;
  left: 50%;
}
.overview-block__play-action::after {
  content: "";
  border: 0;
  border-top: 12px solid transparent;
  border-bottom: 12px solid transparent;
  border-left: 15px solid white;
  position: absolute;
  transform: translate(-50%, -50%);
  top: 50%;
  left: 53%;
}
.overview-block__play-action:hover {
  cursor: pointer;
}
@keyframes halo {
  0% {
    opacity: 0.8;
    transform: scale(1);
  }
  100% {
    opacity: 0;
    transform: scale(2);
  }
}
```
