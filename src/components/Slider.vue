<template>
    <section id="sliderType" :class="['slider__wrap', element]">
        <h2 class="blind">{{ title }}</h2>
        <div class="slider__inner">
            <div class="slider">
                <div class="slider__img">
                    <div class="desc">
                        <span>developer</span>
                        <h3>new frontend</h3>
                        <p>
                            너무 무리하지 말아요! 이미 당신은 잘하고 있고!<br />
                            앞으로도 잘 할 수 있어요!
                        </p>
                        <div class="btn">
                            <a href="/">자세히 보기</a>
                            <a href="/" class="black">사이트 보기</a>
                        </div>
                    </div>
                </div>
                <div class="slider__arrow">
                    <a href="/" class="left"><span class="ir">이전 이미지</span></a>
                    <a href="/" class="right"><span class="ir">다음 이미지</span></a>
                </div>
                <div class="slider__dot">
                    <a href="/" class="dot active"><span class="ir">1</span></a>
                    <a href="/" class="dot"><span class="ir">2</span></a>
                    <a href="/" class="dot"><span class="ir">3</span></a>
                    <a href="/" class="play"><span class="ir">플레이</span></a>
                    <a href="/" class="stop"><span class="ir">정지</span></a>
                </div>
            </div>
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
/* sliderType */
.slider {
    position: relative;
}

.slider__img {
    background: url(../assets/img/slider_bg01.jpg) no-repeat center center / cover;
}

.slider__img .desc {
    width: 1160px;
    margin: 0 auto;
    padding: 100px 20px;
}

.slider__img .desc span {
    font-size: 16px;
    background-color: #fff;
    padding: 1px 14px 0 14px;
    border-radius: 30px;
    text-transform: uppercase;
    margin-bottom: 10px;
    display: inline-block;
}

.slider__img .desc h3 {
    font-size: 110px;
    font-weight: 300;
    line-height: 1;
    color: #fff;
    text-transform: uppercase;
    margin-bottom: 16px;
    margin-left: -8px;
}

.slider__img .desc p {
    font-size: 20px;
    font-weight: 300;
    color: #fff;
    line-height: 1.35;
    margin-bottom: 130px;
}

.slider__img .desc .btn a {
    font-size: 16px;
    background: #fff;
    padding: 11px 50px;
    display: inline-block;
}

.slider__img .desc .btn a.black {
    background: #000;
    color: #fff;
}

.slider__arrow a {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    width: 30px;
    height: 56px;
    background-image: url(../assets/img/slider_icon.svg);
}

.slider__arrow a.left {
    left: 20px;
}

.slider__arrow a.right {
    right: 20px;
    background-position: -50px 0;
}

.slider__dot {
    position: absolute;
    left: 50%;
    bottom: 25px;
    transform: translateX(-50%);
}

.slider__dot a {
    display: inline-block;
    width: 16px;
    height: 16px;
    background-image: url(../assets/img/slider_icon.svg);
    background-position: -20px -70px;
}

.slider__dot a.active {
    background-position: 0px -70px;
}

.slider__dot a.play {
    background-position: -40px -70px;
}

.slider__dot a.stop {
    background-position: -60px -70px;
}
</style>