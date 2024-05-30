<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-100">
                    <div class="dflex justify-content-between align-items">
                        <div class="footer-content">
   
                            <h3 class="py-10">Boolando s.r.l</h3>
                            <ul class="footer-list py-10">
                                <li>
                                    Informazioni legali
                                </li>
                                <li>
                                    Informativa sulla privacy
                                </li>
                                <li>
                                    Diritto di recesso
                                </li>
                            </ul>
                        </div>

                        <div class="footer-content">
                            <h3 class="py-10">Trovaci anche su</h3>
                            <ul class="footer-list py-10">

                                <li class="margin">
                                    <i class="fa fa-twitter"></i>
                                </li>
                                <li class="margin">
                                    <i class="fa fa-facebook-f"></i>
                                </li>
                                <li>
                                    <i class="fa fa-instagram"></i>
                                </li>
                                <li class="margin">
                                    <i class="fa fa-pinterest"></i>
                                </li>
                                <li class="margin">
                                    <i class="fa fa-youtube-play"></i>
                                </li>
                            </ul>
                        </div>    


                        

                </div>
            </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
name: 'FooterComponent'
}
</script>

<style scoped lang="scss">
footer {
    background-color: black;
    padding: 20px;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 15px;
}

.row {
  display: flex;
  flex-wrap: wrap;
}

.col-100 {
  flex: 1 1 100%;
  max-width: 100%;
}

.dflex {
  display: flex;
}

.justify-content-between {
  justify-content: space-between;
}

.align-items {
  align-items: center;
}

.footer-content {
margin: 0 20px;
}

.py-10 {
padding-top: 10px;
padding-bottom: 10px;
}

.footer-list {
list-style: none;
padding: 0;
margin: 0;
}

.footer-list li {
margin-bottom: 5px;
}

.margin {
margin-right: 10px;
}

.fa {
font-size: 20px;
color: #333;
}
</style>