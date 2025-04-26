<!DOCTYPE html>
<html>
<meta charset='UTF-8' />
<meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport' />
<meta content='IE=edge' http-equiv='X-UA-Compatible' />

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Shippori+Antique:wght@400;500;700&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Dancing+Script&display=swap" rel="stylesheet">

<script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script><script src="https://unpkg.com/typeit@8.7.0/dist/index.umd.js"></script><script src="https://kit.fontawesome.com/4f3ce16e3e.js" crossorigin="anonymous"></script><link rel="stylesheet" href="https://htmlku.com/taubedanya/main/styles.css">

<head>
    <title>S.id/taubedanya - Script HTML buat Kamu</title>
    <meta name="description" content="Feeldream Coding">

    <!-- 
    Made with love by feeldream!

    Blog: https://feeldream.id

    Thanks to all <3
    -->
</head>

<body>

    <!-- Ganti Audio di sini -->
    <audio src="https://feeldreams.github.io/maimuna.mp3" id="linkmp3" class="sembunyi"></audio>

    <div id="bodyblur">
        <!-- Wallpaper --><img src="https://i.ibb.co.com/z2dmFv3/f8cb72d992f0d1fb846ef559d58ededc.jpg" id="wallpaper" />
        <div id="beneranblur"></div>
    </div>

    <div id='Content'>

        <!-- Tombol LOVE -->
        <div id="loveIn">
            <a href="#" class="lovein">&#10084;</a>
        </div>
        <p id="ket">Sentuh LOVEnya!</p>

        <div class="kumpulanstiker">
            <!-- Stiker untuk Konten -->
            <img src="https://feeldreams.github.io/pandapanah.gif" id="fotostiker" />
            <img src="https://feeldreams.github.io/pusn.gif" id="fotostiker1" />
            <img src="https://feeldreams.github.io/mikir.gif" id="fotostiker2" />
            <img src="https://feeldreams.github.io/g5.gif" id="fotostiker3" />
            <img src="https://feeldreams.github.io/mmm.gif" id="fotostiker4" />
            <img src="https://feeldreams.github.io/emawh.gif" id="fotostiker5" />
        </div>

        <p id="halo" class="halo"></p>

        <div>
            <blockquote id='bq' data-text=''>

                <p id="kalimat"><span style="font-size:15px">Aku Punya Pesan<br>Nih buat Kamu đŤ˘â¤ď¸</span></p>
                <p id="kalimatb"></p>

                <!-- Pesan -->
                <p id="pesan1"><b style="font-size:16px">Klik 4 LOVE ini! đŤŁ</b></p>
                <div id="kolombaru">
                    <li id="lv1">đ</li>
                    <li id="lv2">đ</li>
                    <li id="lv3">đ</li>
                    <li id="lv4">đ</li>
                </div>

                <p id="pesan2"></p>
                <p id="pesan3"></p>
                <p id="pesan4" class="sty2b"><b>Kamu tau gaa? đŤŁ</b></p>
                <p id="pesan5" class="sty2b">Bedanya helm sama<br>kamu itu apa? đŤ˘</p>
                <p id="pesan6" class="sty2b">Kalo helm buat kepala...</p>
                <p id="pesan7" class="sty2b left"><b>Kalo kamu...<br>Buat aku ajaaa! đđ</b></p>
                <p id="pesan8" class="sty2b left"><i>Hehehe</i> đ<br>Btw, Hati Hati Dijalan ya pulang kampungnya, jangan lupa balik lagi ke palu đĽšđ</p>

                <!-- Tombol Lanjut -->
                <p id="opsL">Klik untuk Lanjut</p>
            </blockquote>
        </div>

        <!-- Tombol Kirim Pesan -->
        <div id="Tombol"><a id="By" href="https://wa.me/6281234567890" target="_blank">&#128140; Balas</a></div>

        <!-- Pesan Ditolak -->
        <div id="pesanditolak">
            <img id="stikerditolak" src="https://feeldreams.github.io/weee.gif" />
            <p id="kataditolak">Harus balik lagi ke palu đ</p>
        </div>

    </div>

    <script>
        function welcome() {
            teksWelcome = "Hai, " + nama + " â¨";
        }

        //Variable Pertanyaan Akhir
        var tanya = 'Balik ke palu lagi ee đśâ¤ď¸';
        var opstanya = 'Ayo jawab đ';
        var tompositif = 'Iya';
        var tomnegatif = 'Nda Mau';

        async function pertanyaan() {
            var { isConfirmed: prtanya } = await swals.fire({ title: nama + ' ' + tanya, text: '' + opstanya, imageUrl: '' + fotostiker5.src, showCancelButton: true, confirmButtonText: '' + tompositif, cancelButtonText: '' + tomnegatif, });
            if (prtanya) {
                pesanwhatsapp = "Iyaa " + nama + " Nanti Balik kepalu lagi";
                menujuWA();
            } else {
                pesanwhatsapp = nama + " nda mau wleeee";
                await swalst.fire({ title: '' + kataditolak.innerHTML, timer: 2000, imageUrl: '' + stikerditolak.src, });
                menujuWA();
            }
        }
    </script>
    <script src="https://htmlku.com/taubedanya/main/script.js"></script>

</body>
</html>
