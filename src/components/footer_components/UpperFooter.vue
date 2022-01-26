<template>
    <div class="my-container row row-cols-3 pt-5 pb-5">
        <div class="logo p-2">
            <img src="../../assets/images/logotype-2-139x23.png" alt="">
        </div>
        <div class="links-container col d-flex justify-content-around">
            <ul class="d-flex">
                <li v-for="(element, index) in upperFooterLinks" :key="index" class="p-2">
                    <a href="">{{element.link}}</a>
                </li>
            </ul>
        </div>
        <div class="social-container">
            <ul class="d-flex flex-row-reverse">
                <li v-for="(el, index) in upperFooterSocial" :key="'Social' + index" class="p-2">
                    <a href=""><i :class="el.icon"></i></a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'UpperFooter',
    props: [
        'upperFooterLinks',
        'upperFooterSocial'
    ]
}
</script>

<style lang="scss" scoped>
    .my-container {
        width: 88%;
        margin: 0 auto;
        border-bottom: 1px solid var(--border-white-2);
        .links-container {
            ul {
                list-style-type: none;
                padding: 0;
                margin: 0;
                li {
                    a {
                        text-decoration: none;
                        color: var(--tx-grey-6);
                        font-size: 0.85em;
                    }
                }
            }
        }
    }
    .social-container {
            ul {
                list-style-type: none;
                padding: 0;
                margin: 0;
                li {
                    a{
                        text-decoration: none;
                        color: var(--tx-white-1);
                        i{
                        font-size: 1.2em; 
                    }
                    }
                    
                }    
            }
        }
</style>