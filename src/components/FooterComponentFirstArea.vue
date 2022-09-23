<template>
  <footer>
    <img src="img/dc-logo-bg.png" alt="Logo Footer">
    <div class="navigationFooter">
        <div class="col-1">
            <h2>DC COMICS</h2>
            <ul>
                <li v-for="menu_1_A in col_1_A" :key="menu_1_A.textLink"><a :href="menu_1_A.link">{{menu_1_A.textLink}}</a></li>
            </ul>
            <h2>SHOP</h2>
            <ul>
                <li v-for="menu_1_B in col_1_B" :key="menu_1_B.textLink"><a :href="menu_1_B.link">{{menu_1_B.textLink}}</a></li>
            </ul>
        </div>
        <div class="col-2">
            <h2>DC</h2>
            <ul>
                <li v-for="menu_2 in col_2" :key="menu_2.textLink"><a :href="menu_2.link">{{menu_2.textLink}}</a></li>
            </ul>
        </div>
        <div class="col-3">
            <h2>SITES</h2>
            <ul>
                <li v-for="menu_3 in col_3" :key="menu_3.textLink"><a :href="menu_3.link">{{menu_3.textLink}}</a></li>
            </ul>
        </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComponentFirstArea",
  data(){
    return {
        col_1_A:[
            {
                textLink: 'Characters',
                link: '#'
            },
            {
                textLink: 'Comics',
                link: '#'
            },
            {
                textLink: 'Movies',
                link: '#'
            },
            {
                textLink: 'TV',
                link: '#'
            },
            {
                textLink: 'Games',
                link: '#'
            },
            {
                textLink: 'Videos',
                link: '#'
            },
            {
                textLink: 'News',
                link: '#'
            },
        ],
        col_1_B:[
            {
                textLink: 'Shop DC',
                link: '#'
            },
            {
                textLink: 'Shop DC Collectibles',
                link: '#'
            }
        ],
        col_2:[
            {
                textLink: 'Terms Of Use',
                link: '#'
            },
            {
                textLink: 'Privacy policy (New)',
                link: '#'
            },
            {
                textLink: 'Ad Choices',
                link: '#'
            },
            {
                textLink: 'Advertising',
                link: '#'
            },
            {
                textLink: 'Jobs',
                link: '#'
            },
            {
                textLink: 'Subscriptions',
                link: '#'
            },
            {
                textLink: 'Talent Workshops',
                link: '#'
            },
            {
                textLink: 'CPSC Certificates',
                link: '#'
            },
            {
                textLink: 'Ratings',
                link: '#'
            },
            {
                textLink: 'Shop Help',
                link: '#'
            },
            {
                textLink: 'Contact Us',
                link: '#'
            },
        ],
        col_3:[
            {
                textLink: 'DC',
                link: '#'
            },
            {
                textLink: 'MAD Magazine',
                link: '#'
            },
            {
                textLink: 'DC Kids',
                link: '#'
            },
            {
                textLink: 'DC Universe',
                link: '#'
            },
            {
                textLink: 'DC Pawer Visa',
                link: '#'
            }
        ]
    }
  }
};
</script>

<style lang="scss" scoped>
footer {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-content: center;
  background-image: url("../../public/img/footer-bg.jpg");
  background-size: 120%;
  padding: 40px 8% 70px;
  position: relative;
  overflow: hidden;

  img{
    position: absolute;
    top: -80px;
    right: 8%;
    transform: scale(1.1);
  }

  .navigationFooter{
    width: 40%;
    display: flex;

    .col-1,
    .col-2,
    .col-3{
        width: calc(100% / 3);
        height: 100%;

        h2{
            color: #fff;
            font-size: 1.3rem;
            padding: 15px 0;
        }

        ul{
            list-style-type: none;

            li a{
                text-decoration: none;
                color: #848485;
                font-size: 0.9rem;
                line-height: 1.3rem;

                &:hover{
                    color: #fff;
                }
            }
        }
    }
  }
}
</style>