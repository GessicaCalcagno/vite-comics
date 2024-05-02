<script>
export default {
    data() {
        return {
            dcComicsLinks: [
                { text: 'Characters', url: '#' },
                { text: 'Comics', url: '#' },
                { text: 'Movies', url: '#' },
                { text: 'TV', url: '#' },
                { text: 'Games', url: '#' },
                { text: 'Videos', url: '#' },
                { text: 'News', url: '#' }
            ],

            shopLinks: [
                { text: 'Shop DC', url: '#' },
                { text: 'Shop DC Collectibles', url: '#' }
            ],

            dcLinks: [
                { text: 'Terms Of Use', url: '#' },
                { text: 'Privacy policy (New)', url: '#' },
                { text: 'Ad Choices', url: '#' },
                { text: 'Advertising', url: '#' },
                { text: 'Jobs', url: '#' },
                { text: 'Subscriptions', url: '#' },
                { text: 'Talent Workshops', url: '#' },
                { text: 'CPSC Certificates', url: '#' },
                { text: 'Ratings', url: '#' },
                { text: 'Shop help', url: '#' },
                { text: 'Contact Us', url: '#' }
            ],

            sitesLinks: [
                { text: 'DC', url: '#' },
                { text: 'MAD Magazine', url: '#' },
                { text: 'DC Kids', url: '#' },
                { text: 'DC Universe', url: '#' },
                { text: 'DC Power Visa', url: '#' }
            ],

        }
    }
}
</script>

<template>
    <footer class="footer-top">
        <div class="container-footer">
            <div class=" col col1">
                <h4>DC COMICS</h4>
                <ul>
                    <li v-for="link in dcComicsLinks"> <a href="">{{ link.text }}</a></li>
                </ul>
                <h4>SHOP</h4>
                <ul>
                    <li v-for="link in shopLinks"> <a href="">{{ link.text }}</a></li>
                </ul>
            </div>

            <div class="col  col2">
                <h4>DC</h4>
                <ul>
                    <li v-for="link in dcLinks"> <a href="">{{ link.text }}</a></li>
                </ul>
            </div>

            <div class="col  col3">
                <h4>SITES</h4>
                <ul>
                    <li v-for="link in sitesLinks"> <a href="">{{ link.text }}</a></li>
                </ul>
            </div>

            <div class="ft-img-container">
                <img class="img-ft" src="../assets/img/dc-logo-bg.png" alt="Logo DC footer">
            </div>

        </div>



    </footer>
    <footer class="footer-bottom">
        <div class="container-footer-bottom">
            <div>
                <span class="f-button"><a href="">SIGN UP NOW!</a></span>
            </div>
            <div>
                <ul>
                    <li><a href="">FOLLOW US</a></li>
                    <li><a href=""><img src="../assets/img/footer-facebook.png" alt=""></a></li>
                    <li><a href=""><img src="../assets/img/footer-twitter.png" alt=""></a></li>
                    <li><a href=""><img src="../assets/img/footer-youtube.png" alt=""></a></li>
                    <li><a href=""><img src="../assets/img/footer-pinterest.png" alt=""></a></li>
                    <li><a href=""><img src="../assets/img/footer-periscope.png" alt=""></a></li>
                </ul>
            </div>

        </div>
    </footer>


</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

.container-footer {
    padding: 20px 20px;
    width: 80%;
    margin: 0 auto;
    display: flex;
}

.footer-top {
    color: white;
    position: relative;
    background-image: url(../assets/img/footer-bg.jpg);
    // background-repeat: no-repeat;
    overflow: hidden;
    font-size: 0.8rem;


    h4 {
        font-size: bold;
        padding-bottom: 20px;
    }


    ul {
        list-style-type: none;
        gap: 1rem;
        padding-right: 30px;
        margin-bottom: 28px;

        a {
            font-weight: 540;
            text-decoration: none;
            color: rgb(179, 176, 176);
            display: inline-block;
            padding-bottom: 15px;
        }
    }

    .ft-img-container {
        margin-left: 80px;
        position: absolute;
        width: 40%;
        bottom: -2rem;
        right: 6rem;
    }
}

// _______________________________________

.footer-bottom {
    background-color: #303030;
}

.container-footer-bottom {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    margin: 0 auto;
    padding: 30px 20px;

    ul {
        @include flex(row, center, center);
        list-style-type: none;
        gap: 1rem;

        a {
            text-decoration: none;
            color: $primary-color;
            font-weight: bold;

        }
    }

    .f-button a {
        text-decoration: none;
        color: white;
        display: inline-block;
        font-weight: bold;
        border: 3px solid;
        padding: 10px;
        border-color: $primary-color;
    }


}
</style>