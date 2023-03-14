<script>
  import Router from 'svelte-spa-router'
  import First from "./routes/First.svelte"
  import Home from "./routes/Home.svelte"
  import Detail from "./routes/Detail.svelte"
  import QuestionCreate from "./routes/QuestionCreate.svelte"
  import Navigation from "./components/Navigation.svelte"
  import UserCreate from "./routes/UserCreate.svelte"
  import UserLogin from "./routes/UserLogin.svelte"


  import Chat1 from "./routes/Chat1.svelte"
  import Chat2 from "./routes/Chat2.svelte"
  import Chat3 from "./routes/Chat3.svelte"
  import Chat4 from "./routes/Chat4.svelte"
 
  import Home0 from "./routes/Home0.svelte"
  import Home1 from "./routes/Home1.svelte"
  import Home2 from "./routes/Home2.svelte"
  import Home3 from "./routes/Home3.svelte"
  import Home4 from "./routes/Home4.svelte"

  import Goog1 from "./routes/Goog1.svelte"
  import Goog2 from "./routes/Goog2.svelte"
  import Goog3 from "./routes/Goog3.svelte"
  import Goog4 from "./routes/Goog4.svelte"

  const routes = {
    '/first': First,  
    '/Chat1': Chat1,  
    '/Chat2': Chat2,  
    '/Chat3': Chat3,  
    '/Chat4': Chat4,

    '/Home0': Home0,  
    '/Home1': Home1,  
    '/Home2': Home2,  
    '/Home3': Home3,  
    '/Home4': Home4,

    '/Goog1': Goog1,  
    '/Goog2': Goog2,  
    '/Goog3': Goog3,  
    '/Goog4': Goog4,
    '/': Home,
    '/detail/:question_id': Detail,
    '/question-create': QuestionCreate,
    '/user-create': UserCreate,
    '/user-login': UserLogin,
  }
</script>
<Navigation />
<Router {routes}/>
<!--
//<Nav01 />
//<Router {routes}/>  
-->