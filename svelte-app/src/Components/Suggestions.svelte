<script>
</script>

<div class="pl-4 d-none d-lg-block">
    <a href="#" class="profile d-flex align-items-center">
        <div class="profile-box rounded-circle">
            <img class="img-fluid" src="./img/profile_pic.jpg" alt="marco ram">        
        </div>
        <div class="pl-3 text-left">
            <span class="profile__usuario">markocesar1</span>
            <span class="profile__nombre">Marco Cesar</span>
        </div>
    </a>
    <div class="sugerencias">
        <div class="d-flex justify-content-between align-items-end">
            <span class="sugerencias__titulo">Sugerencias para ti</span>
            <a href="#" class="sugerencias__todo">Ver todo</a>
        </div>
        <ul class="sugerencias__list p-0 my-3">
            <li class="d-flex justify-content-between align-items-center pb-3">
                <a href="" class="sugerencias__usuario d-flex align-items-center">
                    <div class="sugerencias-box-img rounded-circle">
                        <img class="img-fluid" src="./img/sugg/sugg-1.jpg" alt="">
                    </div>
                    <span class="pl-3">3rondy_b_s</span>
                </a>
                <a href="" class="sugerencias__seguir">Seguir</a>
            </li>
            <li class="d-flex justify-content-between align-items-center pb-3">
                <a href="" class="sugerencias__usuario d-flex align-items-center">
                    <div class="sugerencias-box-img rounded-circle">
                        <img class="img-fluid" src="./img/sugg/sugg-2.jpg" alt="">
                    </div>
                    <span class="pl-3">baelmacedland</span>
                </a>
                <a href="" class="sugerencias__seguir">Seguir</a>
            </li>
            <li class="d-flex justify-content-between align-items-center pb-3">
                <a href="" class="sugerencias__usuario d-flex align-items-center">
                    <div class="sugerencias-box-img rounded-circle">
                        <img class="img-fluid" src="./img/sugg/sugg-3.jpg" alt="">
                    </div>
                    <span class="pl-3">tacosfredy</span>
                </a>
                <a href="" class="sugerencias__seguir">Seguir</a>
            </li>
            <li class="d-flex justify-content-between align-items-center pb-3">
                <a href="" class="sugerencias__usuario d-flex align-items-center">
                    <div class="sugerencias-box-img rounded-circle">
                        <img class="img-fluid" src="./img/sugg/sugg-4.jpg" alt="">
                    </div>
                    <span class="pl-3">felicianelo023</span>
                </a>
                <a href="" class="sugerencias__seguir">Seguir</a>
            </li>
            <li class="d-flex justify-content-between align-items-center pb-3">
                <a href="" class="sugerencias__usuario d-flex align-items-center">
                    <div class="sugerencias-box-img rounded-circle">
                        <img class="img-fluid" src="./img/sugg/sugg-5.jpg" alt="">
                    </div>
                    <span class="pl-3">queensbarbecuewings</span>
                </a>
                <a href="" class="sugerencias__seguir">Seguir</a>
            </li>
        </ul>
    </div>
    <div class="info">
        <ul class="clearfix info__list d-block m-0 p-0">
            <li class="info__item d-inline-block"><a class="info__link" href="https://about.instagram.com/" rel="nofollow noopener noreferrer" target="_blank">Información</a></li
            ><li class="info__item d-inline-block"><a class="info__link" href="https://help.instagram.com/">Ayuda</a></li><li class="info__item d-inline-block"><a class="info__link" href="https://about.instagram.com/blog/">Prensa</a></li
            ><li class="info__item d-inline-block"><a class="info__link" href="/developer/">API</a></li
            ><li class="info__item d-inline-block"><a class="info__link" href="/about/jobs/">Empleo</a></li
            ><li class="info__item d-inline-block"><a class="info__link" href="/legal/privacy/">Privacidad</a></li><li class="info__item d-inline-block"><a class="info__link" href="/legal/terms/">Condiciones</a></li
            ><li class="info__item d-inline-block"><a class="info__link" href="/explore/locations/">Ubicaciones</a></li
            ><li class="info__item d-inline-block"><a class="info__link" href="/directory/profiles/">Cuentas destacadas</a></li
            ><li class="info__item d-inline-block"><a class="info__link" href="/directory/hashtags/">Hashtags</a></li
            ><li class="info__item d-inline-block"><a class="info__link" href="/directory/hashtags/">Idioma</a></li>
        </ul>
    </div>
    <span class="instagram mt-4 d-inline-block">© 2020 Instagram from Facebook</span>
</div>

<style type="text/scss">
    .profile{
        margin-top: 30px;
        margin-bottom: 20px;
        &:hover{
            text-decoration: none;
        }
        &-box{
            width: 56px;
            height: 56px;
            overflow: hidden;
        }
        & span{
            display: block;            
        }
        &__usuario{
            font-weight: bold;
            font-size: 12px;
            color: black;
        }
        &__nombre{
            font-size: 12px;
            color: #8e8e8e;
        }
    }
    .sugerencias{
        &__titulo{
            color: #8e8e8e;
            font-weight: bold;
            font-size: 14px;
        }
        &__todo{
            color: black;
            font-weight: bold;
            font-size: 12px;
        }
        &__list{
            list-style: none;
        }
        &-box-img{
            height: 32px;
            width: 32px;
            overflow: hidden;
        }
        &__usuario{
            color: black;
            font-weight: bold;
            font-size: 14px;
        }
        &__seguir{
            color: #0095f6;
            font-size: 12px;
            font-weight: bold;
        }
    }
    .info{
        &__list{
            list-style: none;
            vertical-align: baseline;
            & .info__item{
                color: #c7c7c7;
                &:not(:last-of-type)::after {
                    content: '\00B7';
                    margin: 0 .25em 0 .25em;
                }
            }
        }
        &__item{
            vertical-align: baseline;
            font-size: 11px !important;
            line-height: 1.5em;
            height: auto;
            float: left;
        }
        &__link{
            color: #c7c7c7;            
            &:hover{
                text-decoration: none;                
            }            
        }
    }
    .instagram{
        color: #c7c7c7;
        font-size: 11px;
        text-transform: uppercase;
    }
    .clearfix::after {
  content: "";
  clear: both;
  display: table;
}
</style>