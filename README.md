# 뷰로 사이트 만들기

## 미리보기

## 설치
-`npm create vue@latest`
-`npm instal`
-`npm run format`
-`npm run dev`

## .ellintrc.cjs / .prettierrc.json 설치
1. ctrl + , : format on save 체크

## 메모
- template
- router : 페이지를 연동시키는 페이지
- 'HomeView.vue'에서 props를 사용하여 components에서 script선언 후 export default를 사용하여 props를 받아와서 사용(속성안에사용시 []를 묶어서 사용하고 태그안에 바로사용시 `{{}}`두번 사용해서 사용)
- 배열 생성시 script안에 `data :funcion(){ retun{ 이름:[] } }`을 사용하여 배열을 생성함
- 반복문 사용시 속성값으로 `v-for="(el, i) in cardInfo" :key="i"`를 사용함
- npm run build
