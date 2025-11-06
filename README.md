# vue-demo

## Project setup
```
npm install
```
### update example
```
-EO1--- Options API -> ref()를 사용한 Composition API로 변경
-EO2--- data(), conputed -> computed/ onMountd Composition API로 변경
-EO3--- Options API data() -> ref로 정의하고 <script setup> 에서 v-model 그대로 사용
-EO4--- Options API -> ref/conputed로 선언 후 <script set up>
-EO5--- props를 Options API로 사용 -> defineProps/defineEmits로 Composition API로 변셩
-EO6--- provide()/inject배열 -> provide('key', value) inject('key')로 변경
-EO7--- Options API(props, data...) -> Composition API 버전으로 제공
-EO8--- Options API setup()을 Composition API로 전환 -> setup()내부에서 ref, computed 등을 사용해 기능 유지
-EO9--- setup()기반 코드+중복된 <script> -> 하나의 <script setup>로 통합, props.name선언
-EO10--- setup()에거 ref(0)로 선언 -> <script setup>으로 간결화
-EO11--- reactive로 객체 상태 관리 -> <script setu>에서 reactive로 상태 선언 후 매서드에서 속성 조작
-EO12--- ref로 DOM요소 참조 -> <script setup>로 간단 작성 
### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
