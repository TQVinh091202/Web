*,
*::after,
*::before {
  margin: 0;
  padding: 0;
  box-sizing: inherit; }

html {
  font-size: 62.5%; }
  @media (max-width: 75em) {
    html {
      font-size: 56.25%; } }
  @media (max-width: 56.25em) {
    html {
      font-size: 50%; } }

body {
  box-sizing: border-box;
  padding: 3rem; }
  @media (max-width: 56.25em) {
    body {
      padding: 0; } }

@keyframes moveInLeft {
  0% {
    opacity: 0;
    transform: translateX(-10rem); }
  80% {
    transform: translate(1rem); }
  100% {
    opacity: 1;
    transform: translateX(0); } }

@keyframes moveInRight {
  0% {
    opacity: 0;
    transform: translateX(10rem); }
  80% {
    transform: translate(-1rem); }
  100% {
    opacity: 1;
    transform: translateX(0); } }

@keyframes moveInBottom {
  0% {
    opacity: 0;
    transform: translateY(3rem); }
  100% {
    opacity: 1;
    transform: translateY(0); } }

body {
  font-family: "Lato", sans-serif;
  font-weight: 400;
  line-height: 1.7;
  color: #777;
  overflow-x: hidden; }

.heading-primary {
  color: #fff;
  text-transform: uppercase;
  backface-visibility: hidden;
  margin-bottom: 6rem; }
  .heading-primary--main {
    display: block;
    font-size: 6.2rem;
    font-weight: 400;
    letter-spacing: 1.5rem;
    animation-name: moveInLeft;
    animation-duration: 1s;
    animation-timing-function: ease-out; }
    @media (max-width: 37.5em) {
      .heading-primary--main {
        letter-spacing: 1rem;
        font-size: 5rem; } }
  .heading-primary--sub {
    display: block;
    font-size: 2rem;
    font-weight: 700;
    letter-spacing: 1.8rem;
    animation: moveInRight 1s ease-out; }
    @media (max-width: 37.5em) {
      .heading-primary--sub {
        letter-spacing: .5rem; } }

.heading-secondary {
  font-size: 3.5rem;
  text-transform: uppercase;
  font-weight: 700;
  display: inline-block;
  background-image: linear-gradient(to right, #8e9efc, #1c3eff);
  -webkit-background-clip: text;
  color: transparent;
  transition: all .2s;
  letter-spacing: .2rem;
  cursor: pointer; }
  @media (max-width: 56.25em) {
    .heading-secondary {
      font-size: 3rem; } }
  @media (max-width: 37.5em) {
    .heading-secondary {
      font-size: 2.5rem; } }
  .heading-secondary:hover {
    transform: skewY(5deg) scale(1.1);
    text-shadow: 0.5rem 1rem 2rem rgba(0, 0, 0, 0.2); }

.heading-tertiary {
  font-size: 1.6rem;
  font-weight: 700;
  text-transform: uppercase; }

.paragraph {
  font-size: 1.6rem; }
  .paragraph:not(:last-child) {
    margin-bottom: 3rem; }

.u-center-text {
  text-align: center !important; }

.u-margin-bottom-big {
  margin-bottom: 8rem !important; }

.u-margin-bottom-medium {
  margin-bottom: 4rem !important; }

.u-margin-bottom-small {
  margin-bottom: 1.5rem !important; }

.u-margin-top-big {
  margin-top: 8rem !important; }

.btn, .btn:link, .btn:visited {
  text-transform: uppercase;
  text-decoration: none;
  padding: 1.5rem 4rem;
  display: inline-block;
  border-radius: 10rem;
  transition: all .2s;
  position: relative;
  font-size: 1.6rem;
  border: none;
  cursor: pointer; }

.btn:hover {
  transform: translateY(-0.3rem);
  box-shadow: 0 1rem 2rem rgba(0, 0, 0, 0.2); }
  .btn:hover::after {
    transform: scaleX(1.4) scaleY(1.6);
    opacity: 0; }

.btn:active, .btn:focus {
  outline: none;
  transform: translateY(-0.1rem);
  box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.2); }

.btn::after {
  content: "";
  display: inline-block;
  height: 100%;
  width: 100%;
  border-radius: 10rem;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
  transition: all .4s; }

.btn--white {
  background-color: #fff;
  color: #777; }
  .btn--white::after {
    background-color: #fff; }

.btn--blue {
  background-color: #5a73fc;
  color: #fff; }
  .btn--blue::after {
    background-color: #5a73fc; }

.btn--animated {
  animation: moveInBottom .5s ease-out .75s;
  animation-fill-mode: backwards; }

.btn-text:link, .btn-text:visited {
  color: #5a73fc;
  display: inline-block;
  text-decoration: none;
  border-bottom: 1px solid #5a73fc;
  padding: .3rem;
  font-size: 1.6rem;
  transition: all .2s; }

.btn-text:hover {
  background-color: #5a73fc;
  color: #fff;
  box-shadow: 0 1rem 2rem rgba(0, 0, 0, 0.15);
  transform: translateY(-0.2rem); }

.btn-text:active {
  box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15);
  transform: translateY(0); }

.composition {
  position: relative; }
  .composition__photo {
    width: 50%;
    box-shadow: 0 1.5rem 4rem rgba(0, 0, 0, 0.4);
    border-radius: .2rem;
    position: absolute;
    z-index: 10;
    transition: all .2s;
    outline-offset: 1rem; }
    @media (max-width: 56.25em) {
      .composition__photo {
        float: left;
        position: relative;
        width: 33.3333%;
        box-shadow: 0 1.5rem 3rem rgba(0, 0, 0, 0.2);
        margin-bottom: 2rem; } }
    .composition__photo--p1 {
      left: 0;
      top: -2rem; }
      @media (max-width: 56.25em) {
        .composition__photo--p1 {
          top: 0;
          transform: scale(1.1); } }
    .composition__photo--p2 {
      right: 2rem;
      top: 2rem; }
      @media (max-width: 56.25em) {
        .composition__photo--p2 {
          top: -1rem;
          right: 0;
          transform: scale(1.2);
          z-index: 12; } }
    .composition__photo--p3 {
      left: 10%;
      top: 10rem; }
      @media (max-width: 56.25em) {
        .composition__photo--p3 {
          top: 0;
          left: 0;
          transform: scale(1.1); } }
    .composition__photo:hover {
      outline: 1.5rem solid #5a73fc;
      transform: scale(1.05);
      box-shadow: 0 2.5rem 4rem rgba(0, 0, 0, 0.5);
      z-index: 20; }
    .composition__photo:hover .composition__photo__photo:not(:hover) {
      transform: scale(0.9); }

.skill-box {
  background-color: rgba(255, 255, 255, 0.8);
  font-size: 1.5rem;
  padding: 2.5rem 2.5rem 5rem 2.5rem;
  text-align: center;
  border-radius: 5rem;
  box-shadow: 0 1.5rem 4rem rgba(0, 0, 0, 0.15);
  transition: all .3s; }
  .skill-box__icon {
    font-size: 6rem;
    margin-bottom: 1.5rem;
    display: inline-block;
    background-image: linear-gradient(to right, #8e9efc, #1c3eff);
    -webkit-background-clip: text;
    color: transparent; }
  .skill-box:hover {
    cursor: pointer;
    transform: translateY(-1.5rem) scale(1.03); }

.card {
  perspective: 150rem;
  -moz-perspective: 150rem;
  position: relative;
  height: 45rem; }
  .card__side {
    height: 45rem;
    transition: all .8s ease;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    backface-visibility: hidden;
    border-radius: 5rem;
    overflow: hidden;
    box-shadow: 0 1.5rem 4rem rgba(0, 0, 0, 0.15); }
    .card__side--front {
      background-color: #fff; }
    .card__side--back {
      transform: rotateY(180deg); }
      .card__side--back-1 {
        background-image: linear-gradient(to right, #ffb900, #ff7730); }
      .card__side--back-2 {
        background-image: linear-gradient(to right, #8e9efc, #1c3eff); }
      .card__side--back-3 {
        background-image: linear-gradient(to right, #55c57a, #28b485); }
  .card:hover .card__side--front {
    transform: rotateY(-180deg); }
  .card:hover .card__side--back {
    transform: rotateY(0); }
  .card__picture {
    background-size: cover;
    height: 23rem;
    background-blend-mode: screen;
    clip-path: ellipse(80% 70% at 50% 30%); }
    .card__picture--1 {
      background-image:  url("../img/Cover\ \(3\).png"); }
    .card__picture--2 {
      background-image:  url("../img/hang.jpg"); }
    .card__picture--3 {
      background-image:  url("../img/quang.jpg"); }
  .card__heading {
    font-size: 2.8rem;
    font-weight: 300;
    text-align: right;
    text-transform: uppercase;
    color: #fff;
    position: absolute;
    top: 12rem;
    right: 2rem;
    width: 75%; }
  .card__heading-span {
    border-radius: 5rem;
    padding: 1rem 1.5rem;
    -webkit-box-decoration-break: clone; }
    .card__heading-span--1 {
      background-image: linear-gradient(to right bottom, rgba(255, 185, 0, 0.85), rgba(255, 119, 48, 0.85)); }
    .card__heading-span--2 {
      background-image: linear-gradient(to right bottom, rgba(142, 158, 252, 0.85), rgba(28, 62, 255, 0.85)); }
    .card__heading-span--3 {
      background-image: linear-gradient(to right bottom, rgba(85, 197, 122, 0.85), rgba(40, 180, 133, 0.85)); }
  .card__details {
    padding: 3rem; }
    .card__details ul {
      list-style: none;
      width: 70%;
      margin: 0 auto; }
      .card__details ul li {
        text-align: center;
        font-size: 1.5rem;
        padding: 1rem; }
        .card__details ul li:not(:last-child) {
          border-bottom: 1px solid #dbdbdb; }
  .card__cta {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 90%;
    text-align: center; }
  .card__price-box {
    text-align: center;
    color: #fff;
    margin-bottom: 8rem; }
  .card__price-only {
    font-size: 1.4rem;
    text-transform: uppercase; }
  .card__price-value {
    font-size: 6rem;
    font-weight: 100;
    margin-bottom: 5rem; }
  @media (max-width: 56.25em) {
    .card {
      height: auto; }
      .card__side {
        height: auto;
        border-radius: 5rem 5rem 0rem 0rem;
        position: relative; }
        .card__side--back {
          transform: rotateY(0);
          border-radius: 0rem 0rem 5rem 5rem; }
      .card:hover .card__side--front {
        transform: rotateY(0); }
      .card__cta {
        position: relative;
        top: 0;
        left: 0;
        transform: translate(0);
        width: 100%;
        padding: 4rem; }
      .card__price-box {
        margin-bottom: 3rem; }
      .card__price-value {
        font-size: 6rem; } }

.testimonial {
  width: 80%;
  margin: 0 auto;
  margin-bottom: 2rem;
  box-shadow: 0 3rem 6rem rgba(0, 0, 0, 0.15);
  border-radius: .5rem;
  padding: 6rem;
  padding-left: 9rem;
  font-size: 1.6rem;
  border-radius: 100rem;
  background-color: rgba(255, 255, 255, 0.1);
  z-index: 10; }
  @media (max-width: 56.25em) {
    .testimonial {
      width: 140%;
      margin-left: -20%; } }
  @media (max-width: 37.5em) {
    .testimonial {
      width: 100%;
      margin-left: auto; } }
  .testimonial__shape {
    width: 15rem;
    height: 15rem;
    margin-top: -1rem;
    float: left;
    -webkit-shape-outside: circle(50% at 50% 50%);
    shape-outside: circle(50% at 50% 50%);
    clip-path: circle(50% at 50% 50%);
    transform: translateX(-3rem);
    position: relative; }
  .testimonial__img {
    width: 100%;
    transform: translateY(-2rem);
    transition: all .3s;
    backface-visibility: hidden; }
  .testimonial__caption {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, 20%);
    color: #fff;
    text-transform: uppercase;
    font-size: 1.7rem;
    text-align: center;
    opacity: 0;
    transition: all .5s; }
  .testimonial:hover .testimonial__caption {
    opacity: 1;
    transform: translate(-50%, -50%); }
  .testimonial:hover .testimonial__img {
    transform: scale(1.05);
    filter: blur(0.5rem) brightness(70%); }

.bg-video {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  z-index: -1;
  opacity: .2;
  overflow: hidden; }
  .bg-video__content {
    height: 220%;
    width: 220%;
    object-fit: cover; }

.form__group:not(:last-child) {
  margin-bottom: 2rem; }

.form__input {
  color: inherit;
  font-size: 1.5rem;
  font-family: inherit;
  padding: 1.5rem 2rem;
  border-radius: 2px;
  background-color: rgba(255, 255, 255, 0.5);
  border: none;
  border-bottom: 3px solid transparent;
  width: 80%;
  display: block;
  transition: all .3s; }
  .form__input:focus {
    outline: none;
    box-shadow: 0 1rem 2rem rgba(0, 0, 0, 0.15);
    border-bottom: 3px solid #5a73fc; }
  .form__input:focus:invalid {
    border-bottom: 3px solid #ff7730; }
  .form__input::-webkit-input-placeholder {
    color: #999; }

.form__label {
  font-size: 1.2rem;
  font-weight: 700;
  margin-left: 2rem;
  margin-top: .7rem;
  display: block;
  transition: all .3s; }

.form__input:placeholder-shown + .form__label {
  opacity: 0;
  visibility: hidden;
  transform: translateY(-4rem); }

.form__radio-input {
  display: none; }

.form__radio-group {
  width: 45%;
  display: inline-block; }

.form__radio-label {
  font-size: 1.6rem;
  cursor: pointer;
  position: relative;
  padding-left: 5rem; }

.form__radio-button {
  height: 3rem;
  width: 3rem;
  border: 0.5rem solid #5a73fc;
  border-radius: 10rem;
  display: inline-block;
  position: absolute;
  left: 0;
  top: -.4rem; }
  .form__radio-button::after {
    content: "";
    display: block;
    height: 1.2rem;
    width: 1.2rem;
    border-radius: 50%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #5a73fc;
    opacity: 0;
    transition: opacity .2s; }

.form__radio-input:checked ~ .form__radio-label .form__radio-button::after {
  opacity: 1; }

.popup {
  height: 100vh;
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  background-color: rgba(0, 0, 0, 0.8);
  z-index: 9999;
  opacity: 0;
  visibility: hidden;
  transition: all .5s; }
  .popup__content {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    border-radius: 5rem;
    width: 75%;
    height: 40rem;
    background-color: #fff;
    box-shadow: 0 2rem 4rem rgba(0, 0, 0, 0.2);
    border-radius: 3rem;
    overflow: hidden;
    display: table;
    opacity: 0;
    transform: translate(-50%, -50%) scale(0.5);
    transition: all .4s .2s; }
  .popup__left {
    width: 33.333333%;
    display: table-cell; }
  .popup__right {
    width: 66.666667%;
    display: table-cell;
    vertical-align: middle;
    padding: 3rem 5rem; }
  .popup__img {
    display: block;
    width: 100%; }
  .popup__text {
    font-size: 1.4rem;
    margin-bottom: 4rem;
    column-count: 2;
    column-gap: 4rem;
    column-rule: 1px solid #f7f7f7;
    hyphens: auto; }
  .popup:target {
    opacity: 1;
    visibility: visible; }
  .popup:target .popup__content {
    opacity: 1;
    transform: translate(-50%, -50%) scale(1); }
  .popup__close:link, .popup__close:visited {
    color: #777;
    position: absolute;
    top: 2.5rem;
    right: 2.5rem;
    font-size: 3rem;
    text-decoration: none;
    display: inline-block;
    transition: all .2s; }
  .popup__close:hover {
    color: #5a73fc; }

.header {
  height: 95vh;
  background-image: linear-gradient(to right bottom, rgba(142, 158, 252, 0.8), rgba(28, 62, 255, 0.8)), url("../img/clb.png");
  background-size: cover;
  background-position: top;
  position: relative;
  clip-path: ellipse(60% 60% at 50% 33%); }
  @media (max-width: 37.5em) {
    .header {
      clip-path: ellipse(60% 50% at 50% 20%); } }
  .header__logo-box {
    position: absolute;
    top: 3rem;
    left: 3rem; }
  .header__logo {
    height: 7rem; }
  .header__text-box {
    position: absolute;
    top: 30vh;
    left: 46vw;
    transform: translate(-50%, -50%);
    text-align: center; }

.row {
  max-width: 114rem;
  margin: 0 auto; }
  .row:not(:last-child) {
    margin-bottom: 8rem; }
    @media (max-width: 56.25em) {
      .row:not(:last-child) {
        margin-bottom: 6rem; } }
  @media (max-width: 56.25em) {
    .row {
      max-width: 50rem;
      padding: 0 3rem; } }
  .row::after {
    content: "";
    display: table;
    clear: both; }
  .row [class^="col-"] {
    float: left; }
    .row [class^="col-"]:not(:last-child) {
      margin-right: 6rem; }
      @media (max-width: 56.25em) {
        .row [class^="col-"]:not(:last-child) {
          margin-right: 0;
          margin-bottom: 6rem; } }
    @media (max-width: 56.25em) {
      .row [class^="col-"] {
        width: 100% !important; } }
  .row .col-1-of-2 {
    width: calc((100% - 6rem)/ 2); }
  .row .col-1-of-3 {
    width: calc((100% - 2*6rem) / 3); }
  .row .col-2-of-3 {
    width: calc(2*((100% - 2*6rem) / 3) + 6rem); }
  .row .col-1-of-4 {
    width: calc((100% - 3*6rem) / 4); }
  .row .col-2-of-4 {
    width: calc(2*((100% - 3*6rem) / 4) + 6rem); }
  .row .col-3-of-4 {
    width: calc(3*((100% - 3*6rem) / 4) + 2*6rem); }

.footer {
  background-color: #333;
  padding: 10rem 0;
  font-size: 1.4rem;
  color: #f7f7f7; }
  @media (max-width: 56.25em) {
    .footer {
      padding: 8rem 0; } }
  .footer__logo-box {
    text-align: center;
    margin-bottom: 8rem; }
    @media (max-width: 56.25em) {
      .footer__logo-box {
        margin-bottom: 6rem; } }
  .footer__logo {
    width: 20rem;
    height: auto; }
  .footer__navigation {
    border-top: 1px solid #eeeeee;
    padding-top: 2rem;
    display: inline-block; }
    @media (max-width: 56.25em) {
      .footer__navigation {
        width: 100%;
        text-align: center; } }
  .footer__list {
    list-style: none; }
  .footer__item {
    display: inline-block; }
    .footer__item:not(:last-child) {
      margin-right: 1.5rem; }
  .footer__link:link, .footer__link:visited {
    color: #f7f7f7;
    background-color: #333;
    text-transform: uppercase;
    text-decoration: none;
    display: inline-block;
    border-radius: 5rem;
    transition: all .2s; }
  .footer__link:hover, .footer__link:active {
    color: #5a73fc;
    box-shadow: 0 1rem 2rem rgba(0, 0, 0, 0.4);
    transform: rotate(5deg) scale(1.05); }
  .footer__copyright {
    border-top: 1px solid #eeeeee;
    padding-top: 2rem;
    width: 70%;
    float: right; }
    @media (max-width: 56.25em) {
      .footer__copyright {
        width: 100%;
        text-align: center;
        float: none; } }
  .footer__title {
    display: block;
    color: #5a73fc; }

.navigation__checkbox {
  display: none; }

.navigation__button {
  background-color: #fff;
  height: 7rem;
  width: 7rem;
  position: fixed;
  top: 6rem;
  right: 6rem;
  border-radius: 50%;
  z-index: 2000;
  cursor: pointer;
  text-align: center;
  box-shadow: 0 1rem 3rem rgba(0, 0, 0, 0.15); }
  @media (max-width: 56.25em) {
    .navigation__button {
      top: 4rem;
      right: 4rem; } }
  @media (max-width: 37.5em) {
    .navigation__button {
      top: 3.5rem;
      right: 3.5rem; } }

.navigation__background {
  height: 6rem;
  width: 6rem;
  border-radius: 50%;
  position: fixed;
  top: 6.5rem;
  right: 6.5rem;
  background-image: radial-gradient(#5a73fc, #1c3eff);
  z-index: 1000;
  transition: transform .8s; }
  @media (max-width: 56.25em) {
    .navigation__background {
      top: 4.5rem;
      right: 4.5rem; } }
  @media (max-width: 37.5em) {
    .navigation__background {
      top: 4rem;
      right: 3.5rem; } }

.navigation__nav {
  height: 100vh;
  width: 100%;
  position: fixed;
  top: 0;
  right: 0;
  z-index: 1500;
  opacity: 0;
  width: 0;
  transition: all .8s; }

.navigation__list {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  list-style: none;
  text-align: center;
  width: 100%; }

.navigation__item {
  margin: 1rem; }

.navigation__link:link, .navigation__link:visited {
  display: inline-block;
  border-radius: 4rem;
  font-size: 3rem;
  font-weight: 300;
  padding: 1rem 2rem;
  color: #fff;
  text-decoration: none;
  text-transform: uppercase;
  background-image: radial-gradient(150% 200% ellipse at 115%, #fff 0%, #fff 50%, transparent 50%);
  background-size: 252%;
  transition: all .4s; }

.navigation__link:hover, .navigation__link:active {
  background-position: 100%;
  color: #5a73fc;
  transform: translateX(1rem); }

.navigation__checkbox:checked ~ .navigation__background {
  transform: scale(80); }

.navigation__checkbox:checked ~ .navigation__nav {
  opacity: 1;
  width: 100%; }

.navigation__icon {
  position: relative;
  margin-top: 3.2rem; }
  .navigation__icon, .navigation__icon::before, .navigation__icon::after {
    width: 3.5rem;
    height: .3rem;
    background-color: #999;
    display: inline-block; }
  .navigation__icon::before, .navigation__icon::after {
    content: "";
    position: absolute;
    left: 0;
    transition: all .2s; }
  .navigation__icon::before {
    top: -.8rem; }
  .navigation__icon::after {
    top: .8rem; }

.navigation__button:hover .navigation__icon::before {
  top: -1rem; }

.navigation__button:hover .navigation__icon::after {
  top: 1rem; }

.navigation__checkbox:checked + .navigation__button .navigation__icon {
  background-color: transparent; }

.navigation__checkbox:checked + .navigation__button .navigation__icon::before {
  top: 0;
  transform: rotate(135deg); }

.navigation__checkbox:checked + .navigation__button .navigation__icon::after {
  top: 0;
  transform: rotate(-135deg); }

.section-about {
  background-color: #f7f7f7;
  padding: 25rem 0;
  margin-top: -25rem; }
  @media (max-width: 56.25em) {
    .section-about {
      padding: 20rem 0;
      margin-top: -40rem; } }

.section-skills {
  margin-top: -20rem;
  padding: 20rem 0;
  background-image: linear-gradient(to right bottom, rgba(142, 158, 252, 0.8), rgba(28, 62, 255, 0.8)), url("../img/background2.jpg");
  background-size: cover;
  position: relative;
  clip-path: ellipse(70% 50% at 50% 50%); }
  @media (max-width: 56.25em) {
    .section-skills {
      padding: 15rem 0;
      clip-path: ellipse(90% 50% at 50% 50%); } }

.section-courses {
  background-color: #f7f7f7;
  padding: 25rem 0 10rem 0;
  margin-top: -20rem; }
  @media (max-width: 56.25em) {
    .section-courses {
      padding: 20rem 0 10rem 0;
      margin-top: -15rem; } }

.section-testimonials {
  position: relative;
  padding: 5rem 0 5rem 0; }

.section-enroll {
  padding: 10rem 0;
  background-image: linear-gradient(to right bottom, #8e9efc, #1c3eff); }

.enroll {
  background-image: radial-gradient(150% 200% ellipse at -15%, rgba(255, 255, 255, 0.8) 0%, rgba(255, 255, 255, 0.8) 50%, transparent 50%), url("../img/clb.png");
  background-size: cover;
  box-shadow: 0 1.5rem 4rem rgba(0, 0, 0, 0.2);
  border-radius: 5rem;
  height: 50rem; }
  @media (max-width: 75em) {
    .enroll {
      background-image: radial-gradient(150% 200% ellipse at -15%, rgba(255, 255, 255, 0.8) 0%, rgba(255, 255, 255, 0.8) 65%, transparent 35%), url("../img/clb.jpg"); } }
  @media (max-width: 56.25em) {
    .enroll {
      background-image: linear-gradient(to right, rgba(255, 255, 255, 0.8) 0%, rgba(255, 255, 255, 0.8) 100%), url("../img/clb.png"); } }
  .enroll__form {
    width: 50%;
    padding: 6rem; }
    @media (max-width: 75em) {
      .enroll__form {
        width: 65%; } }
    @media (max-width: 56.25em) {
      .enroll__form {
        width: 100%; } }
