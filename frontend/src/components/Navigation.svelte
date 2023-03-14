<script>
  import { link } from 'svelte-spa-router'
  import { page, access_token, username, is_login } from "../lib/store"
    let home="home";
    let lang = [];
     let title1="Home";
     let title11="Preface";
     let title12="Table of contents";
     let title13="Guide";
     let title14="AI news";
     let title2="chatGPT";
     let title21="chat1";
     let title22="chat2";
     let title23="chat3";
     let title24="chat4";
     let title3="Google";
     let title31="Goog1";
     let title32="Goog2";
     let title33="Goog3";
     let title34="Goog4";
     let title4="Pybo";
     let title41="Pybo";
     let title42="Sign up";
     let title43="Login";
     let title44="Pybo4";
  
function chageLangSelect(){
     if (lang=="kor") {
      title1="홈";
      title11="머릿말";
      title12="목차";
      title13="가이드";
      title14="AI 뉴스";
      title2="쳇GPT";
      title21="쳇1";
      title22="쳇2";
      title23="쳇3";
      title24="쳇4";
      title3="구글";
      title31="구글1";
      title32="구글2";
      title33="구글3";
      title34="구글4";
      title4="게시판";
      title41="파이보";
      title42="회원가입";
      title43="로그인";
      title44="파이보4";
    } else {
      title1="Home";
      title11="Preface";
      title12="Table of contents";
      title13="Guide";
      title14="AI news";
      title2="chatGPT";
      title21="chat1";
      title22="chat2";
      title23="chat3";
      title24="chat4";
      title3="Google";
      title31="Goog1";
      title32="Goog2";
      title33="Goog3";
      title34="Goog4";
      title4="Pybo";
      title41="Pybo";
      title42="Sign up";
      title43="Login";
      title44="Pybo4";

    }
  }
//  bind:value={lang}
</script>

<!-- 네비게이션바 -->
<div class="w-100">
  <table  height=25 bgcolor="#ffffff" class="nav nav-pills mb-3" id="menu-tab" role="tablist"><tr>
    <td       class="nav-item"      role="presentation">
      <button class="nav-link active" id="menu1-tab" data-bs-toggle="pill" data-bs-target="#menu1" type="button" role="tab" aria-controls="menu1" aria-selected="true"><a use:link class="navbar-brand" href="/Home0">{title1}</a></button></td>
    <td       class="nav-item"      role="presentation">
      <button class="nav-link"        id="menu2-tab" data-bs-toggle="pill" data-bs-target="#menu2" type="button" role="tab" aria-controls="menu2" aria-selected="true">{title2}</button>
    </td>
    <td       class="nav-item"      role="presentation">
      <button class="nav-link"        id="menu3-tab" data-bs-toggle="pill" data-bs-target="#menu3" type="button" role="tab" aria-controls="menu3" aria-selected="true">{title3}</button></td>
    <td       class="nav-item"      role="presentation">
      <button class="nav-link"        id="menu4-tab" data-bs-toggle="pill" data-bs-target="#menu4" type="button" role="tab" aria-controls="menu4" aria-selected="true">{title4}</button></td>
    <td       class="nav-item"      role="presentation">

     </tr></table>
</div>
<div class="tab-content" id="pills-tabContent">
  <div class="tab-pane fade show active" id="menu1" role="tabpanel" aria-labelledby="menu1-tab" tabindex="0">
    <table  bgcolor="#eeeeee" height=40 class="nav nav-pills mb-3" id="submenu1-tab" role="tablist"><tr>
      <td       class="nav-item"      role="presentation">
        <button class="nav-link" id="menu11-tab" data-bs-toggle="pill" data-bs-target="#menu11" type="button" role="tab" aria-controls="menu11" aria-selected="true"> <a use:link class="navbar-brand" href="/Home1">{title11}</a></button></td>
      <td       class="nav-item"      role="presentation">
        <button class="nav-link"        id="menu12-tab" data-bs-toggle="pill" data-bs-target="#menu12" type="button" role="tab" aria-controls="menu12" aria-selected="true"><a use:link class="navbar-brand" href="/Home2">{title12}</a></button></td>
      <td       class="nav-item"      role="presentation">
        <button class="nav-link"        id="menu13-tab" data-bs-toggle="pill" data-bs-target="#menu13" type="button" role="tab" aria-controls="menu13" aria-selected="true"><a use:link class="navbar-brand" href="/Home3">{title13}</a></button></td>
      <td       class="nav-item"      role="presentation">
        <button class="nav-link"        id="menu14-tab" data-bs-toggle="pill" data-bs-target="#menu14" type="button" role="tab" aria-controls="menu14" aria-selected="true"><a use:link class="navbar-brand" href="/Home4">{title14}</a></button></td>
    </tr></table>
  </div>
  <div class="tab-pane fade" id="menu2" role="tabpanel" aria-labelledby="menu2-tab" tabindex="0">
    <table  bgcolor="#eeeeee" height=40 class="nav nav-pills mb-3" id="submenu2-tab" role="tablist"><tr>
      <td       class="nav-item"     role="presentation">
        <button class="nav-link"       id="menu21-tab" data-bs-toggle="pill" data-bs-target="#menu21" type="button" role="tab" aria-controls="menu21" aria-selected="true"><a use:link class="navbar-brand" href="/Chat1">{title21}</a></button></td>
      <td       class="nav-item"     role="presentation">
        <button class="nav-link"       id="menu22-tab" data-bs-toggle="pill" data-bs-target="#menu22" type="button" role="tab" aria-controls="menu22" aria-selected="true"><a use:link class="navbar-brand" href="/Chat2">{title22}</a></button></td>
      <td       class="nav-item"     role="presentation">
        <button class="nav-link"       id="menu23-tab" data-bs-toggle="pill" data-bs-target="#menu23" type="button" role="tab" aria-controls="menu23" aria-selected="true"><a use:link class="navbar-brand" href="/Chat3">{title23}</a></button></td>
      <td       class="nav-item"     role="presentation">
        <button class="nav-link"       id="menu24-tab" data-bs-toggle="pill" data-bs-target="#menu24" type="button" role="tab" aria-controls="menu24" aria-selected="true"><a use:link class="navbar-brand" href="/Chat4">{title24}</a></button></td>
    </tr></table>
  </div>
  <div class="tab-pane fade" id="menu3" role="tabpanel" aria-labelledby="menu3-tab" tabindex="0" >
    <table  bgcolor="#eeeeee" height=40 class="nav nav-pills mb-3" id="submenu3-tab" role="tablist"><tr>
      <td       class="nav-item"     role="presentation">
        <button class="nav-link "      id="menu31-tab" data-bs-toggle="pill" data-bs-target="#menu31" type="button" role="tab" aria-controls="menu31" aria-selected="true"><a use:link class="navbar-brand" href="/Goog1">{title31}</a></button></td>
      <td       class="nav-item"     role="presentation">
        <button class="nav-link"       id="menu32-tab" data-bs-toggle="pill" data-bs-target="#menu32" type="button" role="tab" aria-controls="menu32" aria-selected="true"><a use:link class="navbar-brand" href="/Goog2">{title32}</a></button></td>
      <td       class="nav-item"     role="presentation">
        <button class="nav-link"       id="menu33-tab" data-bs-toggle="pill" data-bs-target="#menu33" type="button" role="tab" aria-controls="menu33" aria-selected="true"><a use:link class="navbar-brand" href="/Goog3">{title33}</a></button></td>
      <td       class="nav-item"     role="presentation">
        <button class="nav-link"       id="menu34-tab" data-bs-toggle="pill" data-bs-target="#menu34" type="button" role="tab" aria-controls="menu34" aria-selected="true"><a use:link class="navbar-brand" href="/Goog4">{title34}</a></button></td>
    </tr></table>
  </div>
  <div class="tab-pane fade" id="menu4" role="tabpanel" aria-labelledby="menu4-tab"  tabindex="0" >
    <table  bgcolor="#eeeeee" height=40 class="nav nav-pills mb-3" id="submenu4-tab" role="tablist"><tr>
      <td class="nav-item" role="presentation">      
        <button class="nav-link" id="menu41-tab" data-bs-toggle="pill" data-bs-target="#menu41" type="button" role="tab" aria-controls="menu41" aria-selected="true">
          <a use:link class="navbar-brand" href="/" on:click="{() => {$page = 0}}">{title41}</a>
        </button>
      </td>
      {#if $is_login }
        <td height=20 class="nav-item" role="presentation">
          <button class="nav-link" id="menu42-tab" data-bs-toggle="pill" data-bs-target="#menu42" type="button" role="tab" aria-controls="menu42" aria-selected="true">
            <a use:link href="/user-login" class="nav-link" on:click={() => {
              $access_token = ''
              $username = ''
              $is_login = false
          }}>로그아웃 ({$username})</a>
          </button>
        </td>
      {:else}
        <td height=20 class="nav-item" role="presentation">
          <button class="nav-link" id="menu43-tab" data-bs-toggle="pill" data-bs-target="#menu43" type="button" role="tab" aria-controls="menu43" aria-selected="true">
          <a use:link class="nav-link" href="/user-create">회원가입</a>
          </button>
        </td>
        <td height=20 class="nav-item" role="presentation">
          <button class="nav-link" id="menu44-tab" data-bs-toggle="pill" data-bs-target="#menu44" type="button" role="tab" aria-controls="menu44" aria-selected="true">
          <a use:link class="nav-link" href="/user-login">로그인</a>
          </button>
        </td>
      {/if}
      <td class="nav-item" role="presentation">
        <select bind:value={lang} on:change={()=>chageLangSelect()}>
          <option value="kor">한국어</option>
          <option value="eng">English</option>
       </select>    </td></tr></table>
  </div>
</div>

<style>
  .nav-link {border-radius: 0;}
</style>
