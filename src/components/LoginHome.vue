<template>
<div class="full-container">
    <div class="title-container">
        <h1 style="font-size: 48px" class="text-secondary">스터디 플래너</h1>
    </div>
    <div class="flex-container">
        <div class="form-floating mb-3" style="width: 500px">
            <input type="email" class="form-control" placeholder="이메일" id="floatingEmail">
            <label for="floatingEmail">이메일</label>
        </div>

        <div class="form-floating" style="width: 500px">
            <input type="password" class="form-control" id="floatingPassword" placeholder="비밀번호">
            <label for="floatingPassword">비밀번호</label>
        </div>

        <div style="line-height: 10vh">
            <button type="submit" class="btn btn-lg btn-success" style="width: 500px" href="/"> 로 그 인 </button>
        </div>

            <div style="line-height: 1vh;">
                <a style="color: #6c757d" href="/member">회원가입</a>
            </div>
    </div>
</div>
</template>

<style scoped>
 .full-container{
            height: 75vh;
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
        }
        .flex-container{
            display: flex;
            align-items: stretch;
            justify-content: center;
            flex-direction: column;
            /*border: 2px solid #b6d4fe;*/
        }

        .title-container{
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            margin-bottom: 30px;
        }
</style>
