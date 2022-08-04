<template>
  <div>
    <article>
      <div class="content">
        <h2>Euro 2021</h2>
        <h3>Final (Italy and England)</h3>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. At temporibus voluptate dolor itaque quas exercitationem deserunt deleniti, nam excepturi totam, quasi veritatis saepe numquam culpa facere pariatur, eveniet assumenda dolores incidunt officiis. Doloribus veritatis reprehenderit ducimus, perspiciatis natus temporibus ipsum quasi illum labore assumenda et fuga similique ullam blanditiis dolor illo nam! Voluptatem, blanditiis consequatur vel doloribus reprehenderit atque magni unde. Quia quas dolorum at. Dolorem, molestias nisi officiis ea autem quis quia, sequi natus veniam voluptatum voluptates eveniet a!</p>
        <p>Dolorum consequuntur laudantium tempore harum! Eveniet voluptate reiciendis quos autem accusamus quaerat error animi, accusantium voluptas ipsam. Ratione aut enim natus. Optio repellendus deleniti quas sapiente velit quam libero sit quod architecto quasi enim pariatur a iure iusto dolorem recusandae inventore voluptatem provident, ipsum, doloremque nulla quidem magnam? Qui perferendis nesciunt atque eaque recusandae, velit quibusdam totam, eius voluptatum asperiores ullam sequi dicta sed laboriosam labore sapiente? Enim maxime quia quas sit consectetur asperiores incidunt facere iste, minus labore commodi.</p>
        <p>Exercitationem debitis necessitatibus sunt officiis recusandae natus dolores laborum repudiandae, assumenda explicabo aperiam itaque excepturi obcaecati amet minus delectus voluptatum accusamus quae. Error voluptate tempore officiis et reiciendis accusamus, eveniet officia dicta rerum assumenda repellendus saepe, dolor, aliquid quidem asperiores id vero unde optio. Vitae blanditiis possimus nemo molestias fuga, repellendus dolores veniam quidem aliquam porro incidunt omnis a, deleniti pariatur sint molestiae, nobis et cum nulla dolorem tempora? Sed, accusamus veritatis. Quisquam voluptas aliquid expedita praesentium in, dolore nesciunt!</p>
        <p>Recusandae, mollitia sequi! Nesciunt corrupti accusamus omnis iste, minima ad molestias velit quam excepturi, sequi unde modi at quibusdam amet error, perferendis deserunt optio obcaecati reprehenderit ullam fuga aperiam. Cumque veniam nemo, optio culpa ut quidem, eum repudiandae cupiditate iusto dignissimos facilis error dicta consectetur at dolore sed laborum facere? Perferendis tempora et provident fugiat dolore asperiores soluta cumque consectetur assumenda quaerat repellat aliquid eaque, praesentium expedita nesciunt eligendi molestias ipsam ipsa. Error totam fuga voluptatem maiores sit dolores modi!</p>
        <p>Voluptatem exercitationem eveniet officiis dolores autem, perferendis a officia mollitia magnam cumque perspiciatis nesciunt ab ipsa error dolorem explicabo accusantium, aliquid maiores. Consectetur optio odio esse quam, cupiditate nihil explicabo corrupti vel in facere ipsam inventore voluptatum a, adipisci magnam dolor eligendi amet atque iste possimus alias laboriosam numquam ex quae? Deserunt consequatur explicabo labore fuga est quis harum sit nulla, necessitatibus quasi, hic consequuntur ex voluptate eveniet blanditiis exercitationem magnam praesentium, in nam odio et ratione. Minima, aspernatur unde!</p>
        <p>Corrupti, ullam rerum aliquid in dignissimos asperiores non repellat neque accusamus ut sapiente. Nostrum qui quisquam optio ipsa quam voluptas adipisci reiciendis illum, possimus repellendus consequatur id voluptatem tenetur illo nesciunt ab veniam facere expedita suscipit error ratione aliquam blanditiis, repudiandae commodi? Quos expedita ducimus accusamus qui dolorum quisquam voluptatem corporis dolorem iure. Ad sunt maiores quis rerum assumenda ex molestiae possimus fugiat exercitationem illo tempora animi pariatur omnis unde molestias, dolore, beatae modi perferendis facilis iusto. Repellendus, quibusdam harum.</p>
        <p>Cumque vitae possimus neque esse dicta optio, error perferendis veritatis voluptatum et quasi non minima, adipisci ad modi harum consequatur ab sint soluta omnis doloremque quod aspernatur. Pariatur recusandae ut, consectetur sit omnis delectus, ipsa ex laudantium aliquid expedita dolore neque deserunt tempora nulla. Dolorum voluptatem sed velit laudantium ipsam voluptates recusandae! Eos sit corrupti, dicta, voluptates hic nesciunt accusantium qui atque, quasi beatae porro commodi incidunt ab velit quidem. Sit neque sapiente corporis? Nostrum sint a eaque reiciendis corporis?</p>
        <p>Odit beatae debitis voluptatum ipsam, unde earum ex non ad quas facere corporis ducimus officiis doloremque blanditiis quibusdam quia? Quis eius in numquam officiis blanditiis sequi quas quos repudiandae, vero rerum, libero, dolorem quod excepturi alias iure minima repellat doloremque eos! Quos neque sint necessitatibus architecto, exercitationem minima quas. Est mollitia molestiae rerum assumenda nihil repudiandae quod dolores non cum repellendus incidunt maiores sequi nulla, ea recusandae quis libero dolor quas eos qui accusantium voluptate alias. Non aliquid doloribus magnam?</p>
      </div>
    </article>
  </div>
</template>
<script>
import { timeStamp } from 'console'

export default {
  name:'CompPost',
  mounted() {
    this.$el.addEventListener('scroll', function(){
      let scrollTop = this.$el.scrollTop
      let clientHeight = this.$el.clientHeight
      let scrollHeight = this.$el.scrollHeight
      let scrollPercent = Math.round((scrollTop)/(scrollHeight - clientHeight)*100)

      this.$emit('progressUpdate', scrollPercent)
   }.bind(this))
  },
}
</script>
<style>
.content {
  width: 100%;
  flex: 1 1 100%;
  height:88vh;
  background: aqua;
  overflow: scroll;
}
article .content{
  padding: 25px;
}

article .content h2{
  font-size: 32px;
  font-weight: 900;
  margin-bottom: 10px;
}
article .content h3{
  font-size: 22px;
  font-weight: 300;
  margin-bottom: 30px;
}
article .content p{
  font-size: 18px;
  font-weight: 300;
  margin-bottom: 15px;
  line-height: 1.5;
  color: #313131;
}

</style>
