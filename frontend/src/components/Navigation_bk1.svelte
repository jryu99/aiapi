<script>
    import { link } from 'svelte-spa-router'
</script>

<!-- 네비게이션바 -->
<ul class="nav nav-pills mb-3" id="pills-tab" role="tablist">
    <table bgcolor="#eeeeee" width=100%  height=40>
      <tr>
        <td class="nav-item" role="presentation">
          <button class="nav-link active" id="pills-home-tab" data-bs-toggle="pill" data-bs-target="#pills-home" type="button" role="tab" aria-controls="pills-home" aria-selected="true">Home</button>
        </td>
        <td class="nav-item" role="presentation">
          <button class="nav-link" id="pills-profile-tab" data-bs-toggle="pill" data-bs-target="#pills-profile" type="button" role="tab" aria-controls="pills-profile" aria-selected="false">chatGPT</button>
        </td>
        <td class="nav-item" role="presentation">
          <button class="nav-link" id="pills-contact-tab" data-bs-toggle="pill" data-bs-target="#pills-contact" type="button" role="tab" aria-controls="pills-contact" aria-selected="false">Google</button>
        </td>
        <td class="nav-item" role="presentation">
          <button class="nav-link" id="pills-disabled-tab" data-bs-toggle="pill" data-bs-target="#pills-disabled" type="button" role="tab" aria-controls="pills-disabled" aria-selected="false" disabled>Naver</button>
        </td>
     </tr>
   </table>
  </ul>
  <div class="tab-content" id="pills-tabContent">
    <div class="tab-pane fade show active" id="pills-home" role="tabpanel" aria-labelledby="pills-home-tab" tabindex="0">
        <table bgcolor="#ffddee" height=40 width=100%>
            <tr>
                <td align=center width=20%><a use:link class="navbar-brand" href="/first">First</a></td>
                <td align=center width=20%><a use:link class="nav-link" href="/user-create">회원가입1</a></td>
                <td align=center width=20%><a use:link class="nav-link" href="/user-login">로그인1</a></td>
            </tr>  
        </table>
    
    </div>
    <div class="tab-pane fade" id="pills-profile" role="tabpanel" aria-labelledby="pills-profile-tab" tabindex="0">
      <table bgcolor="#ffddee" height=40 width=100%>
            <tr>
                <td align=center width=20%><a use:link class="navbar-brand" href="/">Pybo</a></td>
                <td align=center width=20%><a use:link class="nav-link" href="/user-create">회원가입</a></td>
                <td align=center width=20%><a use:link class="nav-link" href="/user-login">로그인</a></td>
            </tr>  
        </table>
    </div>
    <div class="tab-pane fade" id="pills-contact" role="tabpanel" aria-labelledby="pills-contact-tab" tabindex="0">
      <table bgcolor="#ffddee" height=40 width=100%>
        <tr>
            <td align=center width=20%><a use:link class="navbar-brand" href="/">Pybo</a></td>
            <td align=center width=20%><a use:link class="nav-link" href="/user-create">회원가입</a></td>
            <td align=center width=20%><a use:link class="nav-link" href="/user-login">로그인</a></td>
        </tr>  
      </table>
    </div>
    <div class="tab-pane fade" id="pills-disabled" role="tabpanel" aria-labelledby="pills-disabled-tab" tabindex="0">
      <table bgcolor="#ffddee" height=40 width=100%>
        <tr>
            <td align=center width=20%><a use:link class="navbar-brand" href="/">Pybo</a></td>
            <td align=center width=20%><a use:link class="nav-link" href="/user-create">회원가입</a></td>
            <td align=center width=20%><a use:link class="nav-link" href="/user-login">로그인</a></td>
        </tr>  
      </table>
    </div>
  </div>

<style>
</style>
