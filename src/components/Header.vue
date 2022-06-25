<template>
<div  style=" margin-left: 10px">
        <div class="dropdown myButton">
            <button class="btn btn-success dropdown-toggle" type="button"
                    id="dropdownMenuButton1" data-bs-toggle="dropdown" aria-expanded="false" style="width: 100px">{{ name }}</button>
            <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
                <li><a class="dropdown-item text-success" href="#">마이페이지</a></li>
                <li><a class="dropdown-item text-success" href="/logout">로그아웃</a></li>
            </ul>
    </div>
 
    <ul class="nav nav-tabs">
        <li class="nav-item">
            <a class="nav-link active text-success" href="/">StudyPlanner</a>
        </li>
        <li class="nav-item">
            <a class="nav-link text-secondary" href="/">계획 등록하기</a>
        </li>
        <li class="nav-item">
            <a class="nav-link text-secondary" href="/">공부중인 계획들</a>
        </li>
        <li class="nav-item">
            <a class="nav-link text-secondary" href="/">완료한 계획들</a>
        </li>
    </ul>
</div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

@Options({
  props: {
    name: String
  }
})
export default class Header extends Vue {
}
</script>

<style scoped>
    .myButton {
        float: right;
        margin-right: 10px
    }
</style>
