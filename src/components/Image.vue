<template>
    <section id="imageType" :class="['image__wrap', element]">
        <h2>{{ title }}</h2>
        <p>이미지 유형입니다. 마우스 오버시 자세한 정보가 나와는 구조입니다.</p>
        <div class="image__inner container">
            <article class="image img1">
                <h3 class="image__title">강아지계의 연예인</h3>
                <p class="image__desc">최근 연예인들 사이에서 키우는 강아지로 유명해진 비숑프리제는 생김새가 아주 작은 바빗과 매우 흡사하여 바비숑이라는</p>
                <a class="image__btn" href="/">자세히 보기</a>
            </article>
            <article class="image img2">
                <h3 class="image__title">강아지계의 마스코트</h3>
                <p class="image__desc">최근 연예인들 사이에서 키우는 강아지로 유명해진 비숑프리제는 생김새가 아주 작은 바빗과 매우 흡사하여 바비숑이라는</p>
                <a class="image__btn yellow" href="/">자세히 보기</a>
            </article>
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
/* imageType */
.image__inner {
    display: flex;
    justify-content: space-between;
}

.image {
    width: 49%;
    height: 370px;
    padding: 200px 30px 30px 30px;
    box-sizing: border-box;
    color: #fff;
}

.image.img1 {
    background: url(../assets/img/image_bg01.jpg) no-repeat center / cover;
}

.image.img2 {
    background: url(../assets/img/image_bg02.jpg) no-repeat center / cover;
}

.image__title {
    font-size: 32px;
    margin-bottom: 10px;
}

.image__desc {
    font-size: 16px;
    margin-bottom: 10px;
    line-height: 1.4;
    font-weight: 300;
    padding-right: 100px;
    overflow: hidden;
    text-overflow: ellipsis;
    display: -webkit-box;
    -webkit-line-clamp: 2;
    -webkit-box-orient: vertical;
    margin-bottom: 10px;
}

.image__btn {
    font-size: 16px;
    font-weight: 300;
    color: #fff;
    background-color: #B45A30;
    padding: 10px 20px;
    display: inline-block;
}

.image__btn.yellow {
    background-color: #B59140;
}
</style>