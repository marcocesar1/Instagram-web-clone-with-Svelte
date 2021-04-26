<script>

</script>

<div class="row">
    <div class="col-md-12 stories-wrap">
        <div>
            <ul class="stories d-flex">
                <li class="stories__item py-3 px-3">
                    <a class="stories__link" href="">
                        <div class="stories-img-box rounded-circle">
                            <img class="img-fluid" src="./img/stories/storie-1.jpg" alt="">
                        </div>
                        <span>demiancrate</span>
                    </a>
                </li>
                <li class="stories__item py-3">
                    <a class="stories__link" href="">
                        <div class="stories-img-box rounded-circle">
                            <img class="img-fluid" src="./img/stories/storie-2.jpg" alt="">
                        </div>
                        <span>montgomer...</span>
                    </a>
                </li>
                <li class="stories__item py-3">
                    <a class="stories__link" href="">
                        <div class="stories-img-box rounded-circle">
                            <img class="img-fluid" src="./img/stories/storie-3.jpg" alt="">
                        </div>
                        <span>elshowde_ch</span>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</div>

<style type="text/scss">
    .stories{
        list-style: none;
        padding: 0;
        margin: 0;
        text-align: center;
        &-wrap{
            border: 1px solid #ced4da;
            border-radius: 3px;
            background-color: white;
        }
        &-img-box{
            width: 66px;
            height: 66px;
            overflow: hidden;
            border: 2px solid #dd326e;
        }
        &__item{
            padding-right: 12px;
            & span{
                font-size: 12px;
                display: block;
            }           
        }
        &__link{
            color: black;
            &:hover{
                text-decoration: none;
            }
        }
    }
</style>