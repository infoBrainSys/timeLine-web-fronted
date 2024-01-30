<script>
  import '@/assets/posts.less'

  export default {
    data(){
      return{
        author:'Name',
        date: '2024-01-01',
        title: 'This is post title',
        contentEllipsis: 'lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do \n' +
            'iusmod tempor incididunt ut lab ore et dolore magna aliqua. Ut enim ad minim veniam,\n ' +
            'quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. \n' +
            'uis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat \n' +
            'ulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia. \n ',
        like: 59,
        comment: 12,
        share: 69
      }
    }
  }
</script>

<template>
  <div class="postsBox">
    <!--    帖子本体-->
    <div class="post">

<!--      帖子图片-->
      <div class="postPicBox">
        <img class="postPic" src="@/assets/img/postDemo.png" alt="">
      </div>

<!--      作者头像-->
      <div class="avatarBox">
        <img class="avatar" src="@/assets/img/avatar.jpg" alt="">
      </div>

<!--      作者名和时间盒子-->
      <div class="authorDateBox">
        <div class="authorBox">
          <i class="fa-solid fa-pen"></i>
          <a href="#">
            <p>{{ author }}</p>
          </a>
        </div>
        <div class="dateBox">
          <span class="date">2023-04-01</span>
        </div>
      </div>

<!--      帖子标题-->
      <div class="postTitle">
        <a href="#">
          <span>
            {{ title }}
          </span>
        </a>
        <div class="lineUnderTitle"></div>
      </div>

      <!--文章摘要本体-->
      <div class="textEllipsis">
        <p>{{ contentEllipsis }}</p>
      </div>

      <!--摘要下方横线设计-->
      <div class="lineUnderContent"></div>
      <!--  摘要下方点赞评论分享设计-->
      <div class="postBottom">
        <div class="like">
          <a href="#">
            <i class="fa-regular fa-heart"></i>
            <i class="fa-solid fa-heart liked"></i>
            <span>{{ like }}</span>
          </a>
        </div>
        <div class="comment">
          <a href="#">
            <i class="fa-regular fa-comment"></i>
            <span>{{ comment }}</span>
          </a>
        </div>
        <div class="share">
          <a href="#">
            <i class="fa-regular fa-share-from-square"></i>
            <span>{{ share }}</span>
          </a>
        </div>
      </div>
    </div>

    <!--    ===============================-->
    <!--    帖子本体-->
    <div class="post">

      <!--      帖子图片-->
      <div class="postPicBox">
        <img class="postPic" src="https://cdn.pixabay.com/photo/2023/06/28/10/00/ai-generated-8093991_640.jpg" alt="">
      </div>

      <!--      作者头像-->
      <div class="avatarBox">
        <img class="avatar" src="@/assets/img/avatar.jpg" alt="">
      </div>

      <!--      作者名和时间盒子-->
      <div class="authorDateBox">
        <div class="authorBox">
          <i class="fa-solid fa-pen"></i>
          <a href="#">
            <p>{{ author }}</p>
          </a>
        </div>
        <div class="dateBox">
          <span class="date">2023-04-01</span>
        </div>
      </div>

      <!--      帖子标题-->
      <div class="postTitle">
        <a href="#">
          <span>
            {{ title }}
          </span>
        </a>
        <div class="lineUnderTitle"></div>
      </div>

      <!--文章摘要本体-->
      <div class="textEllipsis">
<!--        <p>{{ contentEllipsis }}</p>
-->     <p>简介「官方说的」
        这个项目是基于大模型的智能对话机器人，支持微信、企业微信、公众号、飞书、钉钉接入，可选择 GPT3.5/GPT4.0/Claude/ 文心一言 / 讯飞星火 / 通义千问 / Gemini/LinkAI，能处理文本、语音和图片，通过插件访问操作系统和互联网等外部资源，支持基于自有知识库定制企业 AI 应用。 我目前只体验了个人微信的 GPT3.5

        OpenAI 账号注册
        这个作为一个成熟的程序员都会。 创建完账号则前往 API 管理页面 创建一个 API Key 并保存下来，后面需要在项目中配置这个 key。每个账号都有体验数量。花钱是不可能的。要是接入国内的就看看文档吧

        ————————————————
        原文作者：&#38647;&#38647;
        转自链接：https://learnku.com/laravel/t/85519
        版权声明：著作权归作者所有。商业转载请联系作者获得授权，非商业转载请保留以上作者信息和原文链接。</p>
      </div>

      <!--摘要下方横线设计-->
      <div class="lineUnderContent"></div>
      <!--  摘要下方点赞评论分享设计-->
      <div class="postBottom">
        <div class="like">
          <a href="#">
            <i class="fa-regular fa-heart"></i>
            <i class="fa-solid fa-heart liked"></i>
            <span>{{ like }}</span>
          </a>
        </div>
        <div class="comment">
          <a href="#">
            <i class="fa-regular fa-comment"></i>
            <span>{{ comment }}</span>
          </a>
        </div>
        <div class="share">
          <a href="#">
            <i class="fa-regular fa-share-from-square"></i>
            <span>{{ share }}</span>
          </a>
        </div>
      </div>
    </div>
    <!--    ===============================-->
    <!--    帖子本体-->
    <div class="post">

      <!--      帖子图片-->
      <div class="postPicBox">
        <img class="postPic" src="https://cdn.pixabay.com/photo/2023/06/20/01/31/ai-generated-8075773_640.jpg" alt="">
      </div>

      <!--      作者头像-->
      <div class="avatarBox">
        <img class="avatar" src="@/assets/img/avatar.jpg" alt="">
      </div>

      <!--      作者名和时间盒子-->
      <div class="authorDateBox">
        <div class="authorBox">
          <i class="fa-solid fa-pen"></i>
          <a href="#">
            <p>{{ author }}</p>
          </a>
        </div>
        <div class="dateBox">
          <span class="date">2023-04-01</span>
        </div>
      </div>

      <!--      帖子标题-->
      <div class="postTitle">
        <a href="#">
          <span>
            {{ title }}
          </span>
        </a>
        <div class="lineUnderTitle"></div>
      </div>

      <!--文章摘要本体-->
      <div class="textEllipsis">
<!--        <p>{{ contentEllipsis }}</p>-->
        <p>使用简单：使用 UI 界面操作，简单易用。
          web 框架：内置了 Gin 框架和常用的中间件 (日志、request_id、jwt 鉴权、限流、熔断、链路跟踪、指标采集等)
          自动生成代码：根据 sql 或 protobuf 和参数生成不同功能代码，例如生成 web 服务代码、handler (CRUD) 代码、dao (CRUD) 代码、model 代码、redis 缓存代码等。
          代码解耦可扩展：所有生成的代码都可以无缝衔接，不需要手动调整代码，支持自动合并新增模板代码，实现 api 接口” 低代码开发”。
          高可靠：服务代码解耦模块化设计，代码经过严格的测试，并遵循良好的编码规范。
          高性能：在单台服务器中的实际业务中压测获取数据 api 接口轻松过万 qps。
          部署简单：支持一键部署到服务器、docker、k8s 上。

          ————————————————
          原文作者：zhuyasen
          转自链接：https://learnku.com/articles/85517
          版权声明：著作权归作者所有。商业转载请联系作者获得授权，非商业转载请保留以上作者信息和原文链接。</p>
      </div>

      <!--摘要下方横线设计-->
      <div class="lineUnderContent"></div>
      <!--  摘要下方点赞评论分享设计-->
      <div class="postBottom">
        <div class="like">
          <a href="#">
            <i class="fa-regular fa-heart"></i>
            <i class="fa-solid fa-heart liked"></i>
            <span>{{ like }}</span>
          </a>
        </div>
        <div class="comment">
          <a href="#">
            <i class="fa-regular fa-comment"></i>
            <span>{{ comment }}</span>
          </a>
        </div>
        <div class="share">
          <a href="#">
            <i class="fa-regular fa-share-from-square"></i>
            <span>{{ share }}</span>
          </a>
        </div>
      </div>
    </div>
    <!--    ===============================-->
    <!--    帖子本体-->
<!--    <div class="post">-->

<!--      &lt;!&ndash;      帖子图片&ndash;&gt;-->
<!--      <div class="postPicBox">-->
<!--        <img class="postPic" src="https://cdn.pixabay.com/photo/2023/06/20/01/31/ai-generated-8075771_640.jpg" alt="">-->
<!--      </div>-->

<!--      &lt;!&ndash;      作者头像&ndash;&gt;-->
<!--      <div class="avatarBox">-->
<!--        <img class="avatar" src="@/assets/img/avatar.jpg" alt="">-->
<!--      </div>-->

<!--      &lt;!&ndash;      作者名和时间盒子&ndash;&gt;-->
<!--      <div class="authorDateBox">-->
<!--        <div class="authorBox">-->
<!--          <i class="fa-solid fa-pen"></i>-->
<!--          <a href="#">-->
<!--            <p>{{ author }}</p>-->
<!--          </a>-->
<!--        </div>-->
<!--        <div class="dateBox">-->
<!--          <span class="date">2023-04-01</span>-->
<!--        </div>-->
<!--      </div>-->

<!--      &lt;!&ndash;      帖子标题&ndash;&gt;-->
<!--      <div class="postTitle">-->
<!--        <a href="#">-->
<!--          <span>-->
<!--            {{ title }}-->
<!--          </span>-->
<!--        </a>-->
<!--        <div class="lineUnderTitle"></div>-->
<!--      </div>-->

<!--      &lt;!&ndash;文章摘要本体&ndash;&gt;-->
<!--      <div class="textEllipsis">-->
<!--        &lt;!&ndash;        <p>{{ contentEllipsis }}</p>&ndash;&gt;-->
<!--        <p>使用简单：使用 UI 界面操作，简单易用。-->
<!--          web 框架：内置了 Gin 框架和常用的中间件 (日志、request_id、jwt 鉴权、限流、熔断、链路跟踪、指标采集等)-->
<!--          自动生成代码：根据 sql 或 protobuf 和参数生成不同功能代码，例如生成 web 服务代码、handler (CRUD) 代码、dao (CRUD) 代码、model 代码、redis 缓存代码等。-->
<!--          代码解耦可扩展：所有生成的代码都可以无缝衔接，不需要手动调整代码，支持自动合并新增模板代码，实现 api 接口” 低代码开发”。-->
<!--          高可靠：服务代码解耦模块化设计，代码经过严格的测试，并遵循良好的编码规范。-->
<!--          高性能：在单台服务器中的实际业务中压测获取数据 api 接口轻松过万 qps。-->
<!--          部署简单：支持一键部署到服务器、docker、k8s 上。-->

<!--          ————————————————-->
<!--          原文作者：zhuyasen-->
<!--          转自链接：https://learnku.com/articles/85517-->
<!--          版权声明：著作权归作者所有。商业转载请联系作者获得授权，非商业转载请保留以上作者信息和原文链接。</p>-->
<!--      </div>-->

<!--      &lt;!&ndash;摘要下方横线设计&ndash;&gt;-->
<!--      <div class="lineUnderContent"></div>-->
<!--      &lt;!&ndash;  摘要下方点赞评论分享设计&ndash;&gt;-->
<!--      <div class="postBottom">-->
<!--        <div class="like">-->
<!--          <a href="#">-->
<!--            <i class="fa-regular fa-heart"></i>-->
<!--            <i class="fa-solid fa-heart liked"></i>-->
<!--            <span>{{ like }}</span>-->
<!--          </a>-->
<!--        </div>-->
<!--        <div class="comment">-->
<!--          <a href="#">-->
<!--            <i class="fa-regular fa-comment"></i>-->
<!--            <span>{{ comment }}</span>-->
<!--          </a>-->
<!--        </div>-->
<!--        <div class="share">-->
<!--          <a href="#">-->
<!--            <i class="fa-regular fa-share-from-square"></i>-->
<!--            <span>{{ share }}</span>-->
<!--          </a>-->
<!--        </div>-->
<!--      </div>-->
<!--    </div>-->


  </div>

</template>

<style scoped>

</style>