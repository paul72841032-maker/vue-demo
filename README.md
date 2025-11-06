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
### picture
```
<img width="909" height="199" alt="image" src="https://github.com/user-attachments/assets/d8621479-41e3-406e-a14f-6144378906eb" />
<img width="666" height="174" alt="image" src="https://github.com/user-attachments/assets/1667d05a-a48e-4f4f-83d2-e5366d59b535" />
<img width="794" height="186" alt="image" src="https://github.com/user-attachments/assets/3151640a-99f8-455e-937a-ee125cdb9cf9" />
<img width="715" height="653" alt="image" src="https://github.com/user-attachments/assets/77b07201-e32c-46d8-a12e-3cb466ce702d" />
<img width="633" height="237" alt="image" src="https://github.com/user-attachments/assets/ea4e073b-ca79-4ba3-9dbc-cc10fb9a2f55" />
<img width="522" height="389" alt="image" src="https://github.com/user-attachments/assets/c4fb5ae8-f18a-407f-888f-f4178ea9f8b9" />











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
