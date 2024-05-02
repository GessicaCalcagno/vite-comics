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
            <div class="col1">
                <h4>DC COMICS</h4>
                <ul>
                    <li v-for="link in dcComicsLinks"> <a href="">{{ link.text }}</a></li>
                    <!-- <li> <a href="">Comics</a></li>
                    <li> <a href="">Movies</a></li>
                    <li> <a href="">TV</a></li>
                    <li> <a href="">Games</a></li>
                    <li> <a href="">Videos</a></li>
                    <li> <a href="">News</a></li> -->
                </ul>
                <h4>SHOP</h4>
                <ul>
                    <li v-for="link in shopLinks"> <a href="">{{ link.text }}</a></li>
                    <!-- <li> <a href="">Shop DC Collectibles</a></li> -->
                </ul>
            </div>

            <div class="col2">
                <h4>DC</h4>
                <ul>
                    <li v-for="link in dcLinks"> <a href="">{{ link.text }}</a></li>
                    <!-- <li> <a href="">Privacy policy (New)</a></li>
                    <li> <a href="">Ad Choices</a></li>
                    <li> <a href="">Advertising</a></li>
                    <li> <a href="">Jobs</a></li>
                    <li> <a href="">Subscriptions</a></li>
                    <li> <a href="">Talent Workshops</a></li>
                    <li> <a href="">CPSC Certificates</a></li>
                    <li> <a href="">Ratings</a></li>
                    <li> <a href="">Shop help</a></li>
                    <li> <a href="">Contact Us</a></li> -->
                </ul>
            </div>

            <div class="col3">
                <h4>SITES</h4>
                <ul>
                    <li v-for="link in sitesLinks"> <a href="">{{ link.text }}</a></li>
                    <!-- <li> <a href="">MAD Magazine</a></li>
                    <li> <a href="">DC Kids</a></li>
                    <li> <a href="">DC Universe</a></li>
                    <li> <a href="">DC Power Visa</a></li> -->
                </ul>
            </div>
        </div>


    </footer>
    <footer class="footer-bottom">
        <div class="container-footer">
            <h2> --> Content goes here <-- </h2>
        </div>
    </footer>


</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

.footer-top {
    color: white;
    background-image: url(../assets/img/footer-bg.jpg);


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
}


.container-footer {
    padding: 20px 20px;
    width: 80%;
    margin: 0 auto;
    display: flex;
}
</style>