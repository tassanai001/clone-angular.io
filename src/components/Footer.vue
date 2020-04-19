<template>
  <v-card elevation="0" class="footer" style="border-radius: unset;">
    <v-footer absolute class="footer footer__container--desktop">
      <v-col class="footer__container">
        <table>
          <tr>
            <th>RESOURCES</th>
            <th>HELP</th>
            <th>COMPANY</th>
            <th>LANGUAGES</th>
          </tr>
          <tr>
            <td>Alfreds Futterkiste</td>
            <td>Maria Anders</td>
            <td>Germany</td>
            <td>Germany</td>
          </tr>
          <tr>
            <td>Centro comercial Moctezuma</td>
            <td>Francisco Chang</td>
            <td>Mexico</td>
            <td>Mexico</td>
          </tr>
          <tr>
            <td>Ernst Handel</td>
            <td>Roland Mendel</td>
            <td>Mexico</td>
            <td>Austria</td>
          </tr>
          <tr>
            <td>Island Trading</td>
            <td>Helen Bennett</td>
            <td>Mexico</td>
            <td>UK</td>
          </tr>
        </table>
      </v-col>
      <p
        style="color: white; text-align: center; margin: 10px 0 5px;"
      >Super-powered by Google ©2010-2020. Code licensed under an MIT-style License. Documentation licensed under CC BY 4.0.</p>
      <br />
      <p
        style="color: white; text-align: center; margin: 10px 0 5px;"
      >Version 9.1.3-local+sha.793a001d7c.</p>
    </v-footer>

    <v-footer absolute class="footer footer__container--mobile">
      <v-col class="footer__container">
        <div class="grid-fluid">
          <div class="footer-block ng-star-inserted">
            <h3>Resources</h3>
            <ul>
              <li class="ng-star-inserted">
                <a class="link" href="about" title="Angular contributors.">About</a>
              </li>
              <li class="ng-star-inserted">
                <a
                  class="link"
                  href="resources"
                  title="Angular tools, training, and blogs from around the web."
                >Resource Listing</a>
              </li>
              <li class="ng-star-inserted">
                <a
                  class="link"
                  href="presskit"
                  title="Press contacts, logos, and branding."
                >Press Kit</a>
              </li>
              <li class="ng-star-inserted">
                <a class="link" href="https://blog.angular.io/" title="Angular Blog">Blog</a>
              </li>
              <li class="ng-star-inserted">
                <a class="link" href="analytics" title="Angular Usage Analytics">Usage Analytics</a>
              </li>
            </ul>
          </div>
          <div class="footer-block ng-star-inserted">
            <h3>Help</h3>
            <ul>
              <li class="ng-star-inserted">
                <a
                  class="link"
                  href="https://stackoverflow.com/questions/tagged/angular"
                  title="Stack Overflow: where the community answers your technical Angular questions."
                >Stack Overflow</a>
              </li>
              <li class="ng-star-inserted">
                <a
                  class="link"
                  href="https://gitter.im/angular/angular"
                  title="Chat about Angular with other birds of a feather."
                >Gitter</a>
              </li>
              <li class="ng-star-inserted">
                <a
                  class="link"
                  href="https://github.com/angular/angular/issues"
                  title="Post issues and suggestions on github."
                >Report Issues</a>
              </li>
              <li class="ng-star-inserted">
                <a
                  class="link"
                  href="https://github.com/angular/code-of-conduct/blob/master/CODE_OF_CONDUCT.md"
                  title="Treating each other with respect."
                >Code of Conduct</a>
              </li>
            </ul>
          </div>
          <div class="footer-block ng-star-inserted">
            <h3>Community</h3>
            <ul>
              <li class="ng-star-inserted">
                <a class="link" href="events" title="Angular events around the world.">Events</a>
              </li>
              <li class="ng-star-inserted">
                <a
                  class="link"
                  href="http://www.meetup.com/topics/angularjs/"
                  title="Attend a meetup and learn from fellow developers."
                >Meetups</a>
              </li>
              <li class="ng-star-inserted">
                <a class="link" href="https://twitter.com/angular" title="Twitter">Twitter</a>
              </li>
              <li class="ng-star-inserted">
                <a class="link" href="https://github.com/angular/angular" title="GitHub">GitHub</a>
              </li>
              <li class="ng-star-inserted">
                <a class="link" href="contribute" title="Contribute to Angular">Contribute</a>
              </li>
            </ul>
          </div>
          <div class="footer-block ng-star-inserted">
            <h3>Languages</h3>
            <ul>
              <li class="ng-star-inserted">
                <a class="link" href="https://angular.cn/" title="简体中文版">简体中文版</a>
              </li>
              <li class="ng-star-inserted">
                <a class="link" href="https://angular.tw/" title="正體中文版">正體中文版</a>
              </li>
              <li class="ng-star-inserted">
                <a class="link" href="https://angular.jp/" title="日本語版">日本語版</a>
              </li>
              <li class="ng-star-inserted">
                <a class="link" href="https://angular.kr/" title="한국어">한국어</a>
              </li>
            </ul>
          </div>
        </div>
      </v-col>
      <p
        class="footer__contact"
      >Super-powered by Google ©2010-2020. Code licensed under an MIT-style License. Documentation licensed under CC BY 4.0.</p>
      <br />
      <p class="footer__version">Version 9.1.3-local+sha.793a001d7c.</p>
    </v-footer>
  </v-card>
</template>

<script>
export default {
  name: "Footer",
  components: {},
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  }
};
</script>


<style scoped>
@media (max-width: 480px) {
  .footer__container--mobile {
    bottom: unset !important;
  }
  .footer__container--mobile {
    display: block;
    text-align: start;
  }
  .footer__container--desktop {
    display: none;
  }
  .footer {
    line-height: 24px;
    line-height: 2.4rem;
    flex: 1;
    /* padding: 48px; */
    background-color: #1976d2;
    font-weight: 300;
    z-index: 0;
  }
  .footer::after {
    content: "";
    position: absolute;
    z-index: -1;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    background: url("../assets/images/angular_whiteTransparent_withMargin.png")
        top 0 left 0 repeat,
      url("../assets/images/angular_whiteTransparent_withMargin.png") top 80px
        left 160px repeat;
    opacity: 0.05;
    background-size: 320px auto;
  }

  th {
    text-align: start;
    color: white;
    padding: 0 24px;
  }
  td {
    text-align: start;
    color: white;
    padding: 0 24px;
  }

  .footer__container {
    display: flex;
    justify-content: center;
  }

  h3 {
    font-size: 16px;
    text-transform: uppercase;
    font-weight: 400;
    margin: 8px 0 12px;
    color: #fff;
  }

  ul {
    list-style-type: none;
    padding-left: unset;
  }
  a {
    color: white;
    text-decoration: none;
  }

  .footer__contact {
    color: white;
    text-align: center;
    margin: 10px 0 5px;
  }
  .footer__version {
    color: white;
    text-align: center;
    margin: 10px 0 5px;
  }
}

@media (min-width: 481px) and (max-width: 768px) {
  .footer__container--mobile {
    display: none;
    text-align: start;
  }
  .footer__container--desktop {
    bottom: unset !important;
    display: block;
    padding: 48px;
  }
  .footer {
    line-height: 24px;
    line-height: 2.4rem;
    flex: 1;
    background-color: #1976d2;
    font-weight: 300;
    z-index: 0;
  }
  .footer::after {
    content: "";
    position: absolute;
    z-index: -1;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    background: url("../assets/images/angular_whiteTransparent_withMargin.png")
        top 0 left 0 repeat,
      url("../assets/images/angular_whiteTransparent_withMargin.png") top 80px
        left 160px repeat;
    opacity: 0.05;
    background-size: 320px auto;
  }

  th {
    text-align: start;
    color: white;
    padding: 0 24px;
  }
  td {
    text-align: start;
    color: white;
    padding: 0 24px;
  }

  .footer__container {
    display: flex;
    justify-content: center;
  }
}

@media (min-width: 769px) and (max-width: 1024px) {
  .footer__container--mobile {
    display: none;
    text-align: start;
  }
  .footer__container--desktop {
    bottom: unset !important;
    display: block;
    padding: 48px;
  }
  .footer {
    line-height: 24px;
    line-height: 2.4rem;
    flex: 1;
    background-color: #1976d2;
    font-weight: 300;
    z-index: 0;
  }
  .footer::after {
    content: "";
    position: absolute;
    z-index: -1;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    background: url("../assets/images/angular_whiteTransparent_withMargin.png")
        top 0 left 0 repeat,
      url("../assets/images/angular_whiteTransparent_withMargin.png") top 80px
        left 160px repeat;
    opacity: 0.05;
    background-size: 320px auto;
  }

  th {
    text-align: start;
    color: white;
    padding: 0 24px;
  }
  td {
    text-align: start;
    color: white;
    padding: 0 24px;
  }

  .footer__container {
    display: flex;
    justify-content: center;
  }
}

@media (min-width: 1025px) {
  .footer__container--mobile {
    display: none;
    text-align: start;
  }
  .footer__container--desktop {
    bottom: unset !important;
    display: block;
    padding: 48px;
  }
  .footer {
    line-height: 24px;
    line-height: 2.4rem;
    flex: 1;
    background-color: #1976d2;
    font-weight: 300;
    z-index: 0;
  }
  .footer::after {
    content: "";
    position: absolute;
    z-index: -1;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    background: url("../assets/images/angular_whiteTransparent_withMargin.png")
        top 0 left 0 repeat,
      url("../assets/images/angular_whiteTransparent_withMargin.png") top 80px
        left 160px repeat;
    opacity: 0.05;
    background-size: 320px auto;
  }

  th {
    text-align: start;
    color: white;
    padding: 0 24px;
  }
  td {
    text-align: start;
    color: white;
    padding: 0 24px;
  }

  .footer__container {
    display: flex;
    justify-content: center;
  }
}
</style>
