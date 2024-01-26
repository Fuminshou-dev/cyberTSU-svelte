<script>
    import { page } from '$app/stores'

    import cyberLogo from '$lib/images/be.png'
    
    console.log($page.route.id)

   
       export const navs = [
           {
               title: "Главная",
               href: "/"
           },
           {
               title: "Команды",
               href: "/teams"
           },
           {
               title: "О нас",
               href: "/about"
           },
           {
               title: "Контакты",
               href: "/contacts"
           },
           {
               title: "Соц. сети",
               href: "/social"
           },
           {
               title: "Магазин",
               href: "/shop"
           },
           {
               title: "Вакансии",
               href: "/vacancy"
           },
   
       ]
   </script>
   
   <nav>
       <ul>
           <a class='logo 'href="/">
               <img src={cyberLogo} alt="">
           </a>
           {#each navs as {title, href}}
           <li>
               <a {href} class:active={$page.route.id === href} >{title}</a>
           </li>    
           {/each}
       </ul>
   </nav>
   

<style>
    .active {
        text-decoration: underline;
        color: rgba(255, 255, 255, 0.6)
    }
    nav {
        border-bottom: 1px solid white;
        padding: 0;
        margin: 0;
        height: 50px;
    }
    .logo {
        padding-right: 7em;
    }
    img {
        width: 3em;
        margin-left: 0px;
        padding: 0;
    }
    a {
        color: white;
        text-decoration: none;
        cursor: pointer;
        margin: 0;
    }
    ul {
        list-style-type: none;
        padding-top: 0px;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }   
    li {
        padding-right: 2em;
    }
</style>