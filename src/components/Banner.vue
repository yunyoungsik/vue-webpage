<template>
    <section id="bannerType" :class="['baaner__wrap', element]">
        <h2 class="blind">{{ title }}</h2>
        <div class="banner__inner">
            <h3 class="title">유튜버 웹보이</h3>
            <p class="desc">
                더 다양한 강의는 유튜브를 통해 제공하고 있습니다.
                <a href="/" title="유튜브 페이지 이동">youtube.com/c/Webstoryboy</a>
            </p>
            <span class="small">배너 유형01</span>
        </div>
    </section>
</template>
<script>
export default {
    props: {
        props: "string",
        title: "string"
    }
}
</script>

<style>
/* bannerType */
.banner__inner {
    background-image: url(../assets/img/banner_bg01.jpg);
    background-repeat: no-repeat;
    background-position: center center;
    background-size: cover;
    text-align: center;
    padding: 120px 0;
    color: #fff;
}

.banner__inner .title {
    font-size: 50px;
    line-height: 1;
    font-weight: 300;
    margin-bottom: 40px;
}

.banner__inner .desc {
    font-size: 24px;
    line-height: 1.5;
    font-weight: 300;
    margin-bottom: 70px;
}

.banner__inner .desc a {
    display: block;
    color: #fff;
}

.banner__inner .small {
    font-size: 16px;
    text-decoration: underline;
}
</style>