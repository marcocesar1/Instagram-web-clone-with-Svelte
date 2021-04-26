<script>
    import {clickOutside} from '../functions/outside';
    let clickSearch = false

    function search(valor){
        //
        if(valor)
            document.getElementById('search').focus()
        clickSearch = valor        
    }
</script>

<nav class="navbar navbar-expand-lg navbar-white">
    <div class="container d-flex justify-content-between align-items-center">
        <div class="navbar-logo-box">
            <a class="navbar-brand" href="#">
                <img src="img/logo.png" alt="instagram" loading="lazy">
            </a>
        </div>
            <form use:clickOutside on:click_outside={() => { search(false) }} class="d-none d-md-block navbar-form">
                <input placeholder="Busca" class="form-control" type="text" id="search">
                {#if !clickSearch}
                    <div on:click={ () => { search(true) } } class="placeholder-box">
                        <div class="placeholder d-flex justify-content-center align-items-center h-100">
                            <span class="sprite sprite__search"></span>
                            <span class="text">Busca</span>
                        </div>
                    </div>
                {:else}
                    <span class="sprite sprite__search sprite__searchFocus"></span>
                    <span on:click={ () => { search(false) } } class="sprite sprite__clear"></span>
                {/if}
            </form>
        <ul class="d-flex navbar__list m-0 pl-0">
            <li class="navbar__item">
                <a href="#">
                    <svg aria-label="Inicio" class="_8-yf5 " fill="#262626" height="22" viewBox="0 0 48 48" width="22"><path d="M45.5 48H30.1c-.8 0-1.5-.7-1.5-1.5V34.2c0-2.6-2.1-4.6-4.6-4.6s-4.6 2.1-4.6 4.6v12.3c0 .8-.7 1.5-1.5 1.5H2.5c-.8 0-1.5-.7-1.5-1.5V23c0-.4.2-.8.4-1.1L22.9.4c.6-.6 1.6-.6 2.1 0l21.5 21.5c.3.3.4.7.4 1.1v23.5c.1.8-.6 1.5-1.4 1.5z"></path></svg>
                </a>
            </li>
            <li class="navbar__item">
                <a href="#">
                    <svg aria-label="Direct" class="_8-yf5 " fill="#262626" height="22" viewBox="0 0 48 48" width="22"><path d="M47.8 3.8c-.3-.5-.8-.8-1.3-.8h-45C.9 3.1.3 3.5.1 4S0 5.2.4 5.7l15.9 15.6 5.5 22.6c.1.6.6 1 1.2 1.1h.2c.5 0 1-.3 1.3-.7l23.2-39c.4-.4.4-1 .1-1.5zM5.2 6.1h35.5L18 18.7 5.2 6.1zm18.7 33.6l-4.4-18.4L42.4 8.6 23.9 39.7z"></path></svg>
                </a>
            </li>
            <li class="navbar__item">
                <a href="#">
                    <svg aria-label="Buscar personas" class="_8-yf5 " fill="#262626" height="22" viewBox="0 0 48 48" width="22"><path clip-rule="evenodd" d="M24 0C10.8 0 0 10.8 0 24s10.8 24 24 24 24-10.8 24-24S37.2 0 24 0zm0 45C12.4 45 3 35.6 3 24S12.4 3 24 3s21 9.4 21 21-9.4 21-21 21zm10.2-33.2l-14.8 7c-.3.1-.6.4-.7.7l-7 14.8c-.3.6-.2 1.3.3 1.7.3.3.7.4 1.1.4.2 0 .4 0 .6-.1l14.8-7c.3-.1.6-.4.7-.7l7-14.8c.3-.6.2-1.3-.3-1.7-.4-.5-1.1-.6-1.7-.3zm-7.4 15l-5.5-5.5 10.5-5-5 10.5z" fill-rule="evenodd"></path></svg>
                </a>
            </li>
            <li class="navbar__item">
                <a href="#">
                    <svg aria-label="Sección de actividades" class="_8-yf5 " fill="#262626" height="22" viewBox="0 0 48 48" width="22"><path d="M34.6 6.1c5.7 0 10.4 5.2 10.4 11.5 0 6.8-5.9 11-11.5 16S25 41.3 24 41.9c-1.1-.7-4.7-4-9.5-8.3-5.7-5-11.5-9.2-11.5-16C3 11.3 7.7 6.1 13.4 6.1c4.2 0 6.5 2 8.1 4.3 1.9 2.6 2.2 3.9 2.5 3.9.3 0 .6-1.3 2.5-3.9 1.6-2.3 3.9-4.3 8.1-4.3m0-3c-4.5 0-7.9 1.8-10.6 5.6-2.7-3.7-6.1-5.5-10.6-5.5C6 3.1 0 9.6 0 17.6c0 7.3 5.4 12 10.6 16.5.6.5 1.3 1.1 1.9 1.7l2.3 2c4.4 3.9 6.6 5.9 7.6 6.5.5.3 1.1.5 1.6.5.6 0 1.1-.2 1.6-.5 1-.6 2.8-2.2 7.8-6.8l2-1.8c.7-.6 1.3-1.2 2-1.7C42.7 29.6 48 25 48 17.6c0-8-6-14.5-13.4-14.5z"></path></svg>
                </a>
            </li>
            <li class="navbar__item d-flex align-items-center">
                <a href="#">
                    <div class="profile-pic rounded-circle">
                        <img class="img-fluid" src="./img/profile_pic.jpg" alt="marco ram">
                    </div>
                </a>
            </li>
        </ul>
    </div>
</nav>

<style type="text/scss">
    .navbar {
        &-white{
            background-color: #fff;
            border-bottom: 1px solid #dbdbdb;
        }
        & .form-control{
            margin: 0;
            padding: 3px 10px 3px 26px;
            height: 100%;
            border-radius: 3px;
            background-color: #fafafa;
            &:focus {
                outline: none !important;
                border: 1px solid #ced4da;
                box-shadow: none !important;
            }
        }
        &-logo-box{            
            @media(min-width: 768px){
                width: 220px;
            }
        }
        &-form{
            min-width: 125px;
            width: 215px;
            height: 28px;
            position: relative;
        }
        &__list{
            list-style: none;
        }
        &__item{
            margin-left: 22px;
        }
        & .placeholder{
            &-box{
                position: absolute;
                top: 0;
                left: 0;
                right: 0;
                bottom: 0px;
                cursor: text;
                background-color: #fafafa;
                border: solid 1px #dbdbdb;
                border-radius: 3px;
            }
            & .text{
                color: #8e8e8e;
                font-size: 14px;
            }
        }
    }
    .profile-pic{
        overflow: hidden;
        width: 22px;
        height: 22px;
        & >img{
            transform: scale(1.5);
        }
    }
    .sprite{
        &__search{
                background-repeat: no-repeat;
                background-position: -399px -321px;
                height: 10px;
                width: 10px;
                margin-right: 6px;
                margin-top: 1px;
        }
        &__searchFocus{
            position: absolute;
            top: 8px;
            left: 12px;
            margin-right: 0px;
        }
        &__clear{
            background-position: -318px -333px;
            height: 20px;
            width: 20px;
            position: absolute;
            top: 5px;
            right: 6px;
            cursor: pointer;
        }
    }
</style>