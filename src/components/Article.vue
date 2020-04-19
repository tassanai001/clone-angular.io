<template>
  <div class="article__parent">
    <div class="article__container">
      <div class="article__img">
        <img :src="articleList[0].image" class="article__index0--img" />
      </div>
      <div class="article__text" style="margin-left: 15px;">
        <p class="article__text--title">{{ articleList[0].title }}</p>
        <p class="article__text--desc">{{ articleList[0].desc }}</p>
      </div>
    </div>
    <hr />
    <div class="article__container">
      <div class="article__text">
        <p class="article__text--title">{{ articleList[1].title }}</p>
        <p class="article__text--desc">{{ articleList[1].desc }}</p>
      </div>
      <div class="article__img" style="margin-left: 15px;">
        <img :src="articleList[1].image" class="article__index1--img" />
      </div>
    </div>
    <hr />
    <div class="article__container">
      <div class="article__img">
        <img :src="articleList[2].image" class="article__index2--img" />
      </div>
      <div class="article__text" style="margin-left: 15px;">
        <p class="article__text--title">{{ articleList[2].title }}</p>
        <p class="article__text--desc">{{ articleList[2].desc }}</p>
      </div>
    </div>
    <hr />
    <div class="article__container">
      <div class="article__text">
        <p class="article__text--title">{{ articleList[3].title }}</p>
        <p class="article__text--desc">{{ articleList[3].desc }}</p>
      </div>
      <div class="article__img" style="margin-left: 20px;">
        <img :src="articleList[3].image" class="article__index3--img" />
      </div>
    </div>
    <div class="article__bottom">
      <v-card class="mx-auto" max-width="344">
        <v-card-text class="article__cardcontainer">
          <div class="article__img" style="margin: 16px;">
            <img :src="codeIcon" height="70" />
          </div>
          <div class="article__text">
            <p class="article__text--title">Get Started</p>
            <p class="article__cardtext--desc">Start building an Angular application.</p>
          </div>
        </v-card-text>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  name: "Article",
  components: {},
  data() {
    return {
      articleList: [
        {
          title: "DEVELOP ACROSS ALL PLATFORMS",
          desc: `Learn one way to build applications with Angular 
              and reuse your code and abilities to
              build apps for any deployment target.
              For web, mobile web, native mobile and native desktop.`,
          image: require("@/assets/images/responsive-framework.svg")
        },
        {
          title: "SPEED & PERFORMANCE",
          desc: `Achieve the maximum speed possible on the Web Platform today, and take it further, 
                 via Web Workers and server-side rendering.

                Angular puts you in control over scalability. 
                Meet huge data requirements by building data models on RxJS, Immutable.js or another push-model.`,
          image: require("@/assets/images/speed-performance.svg")
        },
        {
          title: "INCREDIBLE TOOLING",
          desc: `Build features quickly with simple, declarative templates. 
          Extend the template language with your own components and use a wide array of existing components. 
          Get immediate Angular-specific help and feedback with nearly every IDE and editor. 
          All this comes together so you can focus on building amazing apps rather than trying to make the code work.`,
          image: require("@/assets/images/joyful-development.svg")
        },
        {
          title: "LOVED BY MILLIONS",
          desc: `From prototype through global deployment, 
          Angular delivers the productivity and scalable infrastructure that 
          supports Google's largest applications.`,
          image: require("@/assets/images/loved-by-millions.svg")
        }
      ],
      codeIcon: require("@/assets/images/code-icon.svg")
    };
  }
};
</script>

<style scoped>
.article__parent {
  padding: 24px;
}
@media (max-width: 480px) {
  .article__container {
    display: flex;
    justify-content: center;
    flex-direction: column;
    max-width: 920px;
    margin: 32px auto;
  }
  .article__text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    max-width: 100%;
  }
  .article__text--title {
    text-align: center;
    font-size: 20px;
    font-size: 20px;
    font-weight: 500;
    color: #1976d2;
    text-transform: uppercase;
  }

  .article__text--desc {
    text-align: center;
    margin: 14px 0 0;
    font-size: 14px;
    line-height: 24px;
    line-height: 1.7rem;
    font-weight: 400;
    color: #444;
  }

  .article__bottom {
    display: flex;
    justify-content: center;
    align-items: center;
    box-sizing: border-box;
  }

  hr {
    border: none;
    background: #dbdbdb;
    height: 1px;
  }
  .article__cardcontainer {
    display: flex;
    justify-content: center;
  }

  .article__cardtext--desc {
    text-align: start;
    margin: 14px 0 0;
    font-size: 0.8rem;
    line-height: 24px;
    line-height: 1rem;
    font-weight: 400;
    color: #444;
  }

  .article__index0--img {
    width: 244px;
    height: 143px;
  }

  .article__index1--img {
    width: 244px;
    height: 151px;
  }

  .article__index2--img {
    width: 244px;
    height: 153px;
  }

  .article__index3--img {
    width: 244px;
    height: 122px;
  }

  .article__img {
    margin: unset !important;
  }
}

@media (min-width: 481px) and (max-width: 768px) {
  .article__container {
    display: flex;
    justify-content: center;
    flex-direction: row;
    max-width: 920px;
    margin: 32px auto;
  }
  .article__text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    max-width: 50%;
  }
  .article__text--title {
    text-align: start;
    font-size: 20px;
    font-weight: 500;
    color: #1976d2;
    text-transform: uppercase;
  }

  .article__text--desc {
    text-align: start;
    margin: 14px 0 0;
    font-size: 14px;
    line-height: 24px;
    line-height: 1.7rem;
    font-weight: 400;
    color: #444;
  }

  .article__bottom {
    display: flex;
    justify-content: center;
    align-items: center;
    box-sizing: border-box;
  }

  hr {
    border: none;
    background: #dbdbdb;
    height: 1px;
  }
  .article__cardcontainer {
    display: flex;
    justify-content: center;
  }

  .article__cardtext--desc {
    text-align: start;
    margin: 14px 0 0;
    font-size: 0.8rem;
    line-height: 24px;
    line-height: 1rem;
    font-weight: 400;
    color: #444;
  }

  .article__index0--img {
    width: 196px;
    height: 115;
  }

  .article__index1--img {
    width: 196px;
    height: 121px;
  }

  .article__index2--img {
    width: 196px;
    height: 123px;
  }

  .article__index3--img {
    width: 196px;
    height: 98px;
  }

  .article__img {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
}

@media (min-width: 769px) and (max-width: 1024px) {
  .article__container {
    display: flex;
    justify-content: center;
    flex-direction: row;
    max-width: 920px;
    margin: 32px auto;
  }
  .article__text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    max-width: 50%;
  }
  .article__text--title {
    text-align: start;
    font-size: 20px;
    font-weight: 500;
    color: #1976d2;
    text-transform: uppercase;
  }

  .article__text--desc {
    text-align: start;
    margin: 14px 0 0;
    font-size: 14px;
    line-height: 24px;
    line-height: 1.7rem;
    font-weight: 400;
    color: #444;
  }

  .article__bottom {
    display: flex;
    justify-content: center;
    align-items: center;
    box-sizing: border-box;
  }

  hr {
    border: none;
    background: #dbdbdb;
    height: 1px;
  }
  .article__cardcontainer {
    display: flex;
    justify-content: center;
  }

  .article__cardtext--desc {
    text-align: start;
    margin: 14px 0 0;
    font-size: 0.8rem;
    line-height: 24px;
    line-height: 1rem;
    font-weight: 400;
    color: #444;
  }

  .article__index0--img {
    width: 306px;
    height: 179;
  }

  .article__index1--img {
    width: 290px;
    height: 179px;
  }

  .article__index2--img {
    width: 355px;
    height: 223px;
  }

  .article__index3--img {
    width: 355px;
    height: 178px;
  }
}

@media (min-width: 1025px) {
  .article__container {
    display: flex;
    justify-content: center;
    flex-direction: row;
    max-width: 920px;
    margin: 32px auto;
  }
  .article__text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    max-width: 50%;
  }
  .article__text--title {
    text-align: start;
    font-size: 20px;
    font-size: 1.3rem;
    font-weight: 500;
    color: #1976d2;
    text-transform: uppercase;
  }

  .article__text--desc {
    text-align: start;
    margin: 14px 0 0;
    font-size: 1rem;
    line-height: 24px;
    line-height: 1.7rem;
    font-weight: 400;
    color: #444;
  }

  .article__bottom {
    display: flex;
    justify-content: center;
    align-items: center;
    box-sizing: border-box;
  }

  hr {
    border: none;
    background: #dbdbdb;
    height: 1px;
  }
  .article__cardcontainer {
    display: flex;
    justify-content: center;
  }

  .article__cardtext--desc {
    text-align: start;
    margin: 14px 0 0;
    font-size: 0.8rem;
    line-height: 24px;
    line-height: 1rem;
    font-weight: 400;
    color: #444;
  }

  .article__index0--img {
    width: 306px;
    height: 179px;
  }

  .article__index1--img {
    width: 290px;
    height: 179px;
  }

  .article__index2--img {
    width: 360px;
    height: 225px;
  }

  .article__index3--img {
    width: 409px;
    height: 205px;
  }
}
</style>
