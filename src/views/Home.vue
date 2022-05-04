<template>
  <div class="home">
    <section class="hero">
      <div class="hero-text container">
        <h4>Computer Scientist</h4>
        <hr />
        <h2>
          Zane <br />
          Willgruber
        </h2>
        <hr />
      </div>
    </section>
    <section><p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum, sapiente? Laudantium qui vero minima at asperiores voluptate tempore voluptas sunt soluta ea praesentium dignissimos enim veritatis adipisci ipsum totam modi, repellat quis sequi. Eos ad iste officia a voluptas, cupiditate molestias voluptatem accusantium praesentium debitis quae aspernatur iusto delectus voluptatum numquam est natus magni nemo quos nulla laudantium. Aliquid cupiditate rerum maxime quisquam ipsum assumenda ipsam quibusdam dignissimos. Architecto dolores, repellat eos iure, illum corrupti sapiente et culpa laborum magni quos? Dolor nobis praesentium perferendis dignissimos tempore. Consequuntur aliquam ad tempora voluptatum unde autem quo magni consequatur odit numquam, doloribus quos error optio quod, mollitia repellat est, corporis ducimus modi enim accusamus aliquid quae nostrum. Quaerat sapiente adipisci saepe? Quo cumque provident, explicabo autem ullam veritatis quae obcaecati ipsa nisi deserunt reprehenderit voluptatibus esse laborum! Voluptatem id odio nostrum necessitatibus quaerat voluptatibus numquam libero ad? Fugiat et ducimus sint rem voluptatum voluptatibus, quisquam explicabo repellat, dicta natus provident animi aliquam exercitationem necessitatibus, delectus ad inventore corrupti ipsum. Nostrum beatae saepe distinctio placeat dolores? Laborum officia dolore quia similique. Ex omnis labore consectetur perspiciatis aspernatur sunt minus ut id? Aliquam, illo optio atque esse corporis quisquam neque architecto perspiciatis odio enim voluptate possimus debitis quaerat dolores, vero magnam magni vitae necessitatibus dolorum accusamus reprehenderit? Dolore fugiat eos sed non? Magnam reprehenderit qui debitis consequatur, expedita, sed enim hic, eligendi iste nam tempora temporibus aliquid ipsam dolor veniam. Incidunt corporis adipisci iste assumenda non voluptatem est amet ex molestias, officia officiis tenetur impedit. Ipsa dolorem vero velit mollitia sint quam consequatur possimus dolores omnis porro quas dicta incidunt tempora fuga repellendus, quisquam accusantium! Sint maxime modi maiores nobis, ab enim numquam similique, quaerat quis aliquid eaque, rerum ipsam sapiente. Cum vitae distinctio quo sit quasi delectus, ea veniam, aspernatur ut quod vel sed fugit neque voluptates quas optio. At nihil consectetur, nostrum voluptatem expedita aliquam, quaerat iure suscipit architecto sequi praesentium. Veritatis quia labore ducimus repellat beatae perferendis a animi necessitatibus, voluptatem voluptates quae exercitationem veniam accusamus eius vitae soluta dolorum error, quo maiores, iure quod dicta rerum. Aliquid voluptatem fuga sunt commodi repellendus eaque harum alias, numquam aperiam beatae, voluptatibus laudantium eius. Iusto modi odio autem debitis magni praesentium esse aperiam totam. Amet obcaecati pariatur ad, beatae quidem soluta, numquam odio deserunt optio delectus aspernatur eius rerum necessitatibus ipsa animi similique. Dolore laboriosam perferendis delectus eveniet mollitia, nulla impedit, ratione libero nemo numquam error? Ab similique amet doloremque iusto qui ad illo esse eius, tempora blanditiis labore, quaerat, at minima impedit! Vero nulla alias sequi voluptatem aperiam autem velit quas iusto sit illum vel, necessitatibus nobis, non harum ut doloribus quae itaque qui, quis incidunt facilis expedita officia exercitationem ipsum. Accusamus quisquam, perspiciatis, quasi necessitatibus repellat eaque ab ducimus illum, vitae soluta aliquam repudiandae praesentium id? Officia perspiciatis consectetur blanditiis nemo inventore, provident asperiores reprehenderit rem eaque illum incidunt in praesentium eligendi fuga odio id harum eius nihil est reiciendis! Quae, aperiam laboriosam. Placeat, saepe hic similique magni illo assumenda impedit.</p></section>
  </div>
</template>

<script>
// @ is an alias to /src
export default {
  name: "HomeView",
  components: {},
};
</script>

<style lang="scss" scoped>
.hero {
  background-image: url("../assets/hero-bg.jpg");
  background-attachment: fixed;
  background-size: cover;
  position: relative;
  width: 100%;
  height: 100vh;
  img {
    object-fit: cover;
    height: 50%;
    width: 50%;
  }
  .hero-text {
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    color: #fff;
    h4 {
      text-transform: uppercase;
      font-size: 22px;
      padding-bottom: 4px;
    }
    h2 {
      font-size: 50px;
      @media (min-width: 550px) {
        font-size: 80px;
      }
    }
    hr:nth-child(2) {
      max-width: 365px;
      margin-bottom: 16px;
    }
    hr:nth-child(4) {
      height: 6px;
      background-color: #fff;
      border: none;
      max-width: 85px;
      margin-top: 16px;
    }
  }
}
</style>