<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy New Year</title>

    <link rel="shortcut icon" href="https://icons.iconarchive.com/icons/iconsmind/outline/512/Envelope-icon.png">

    <meta property="og:image" content="https://www.boston-discovery-guide.com/image-files/800-fireworks-over-harbor-matthew-landers-unsplash-3x2.jpg">
    <meta property="og:title" content="James' Card">
    <meta property="og:description" content="Happy New Year">

    <script src="https://s3.ap-northeast-2.amazonaws.com/materials.spartacodingclub.kr/xmas/snow.js"></script>

    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css2?family=Nanum+Gothic+Coding&family=Poor+Story&display=swap" rel="stylesheet">

    <style>
        * {
            font-family: 'Nanum Gothic Coding', monospace;
            font-family: 'Poor Story', cursive;
        }
        body {
            background-color: #9b070f;


        }

        .envelope {
            

            width: 200px;
            height: 200px;

            background-image: url('https://pngimg.com/uploads/envelope/envelope_PNG18366.png');
            background-size: cover;
            background-position: center;

            margin: 200px auto 0px auto;

            cursor: pointer;

        }

        .envelope-msg {
            color: white;
            text-align: center;
        }
        .letter-close {
            display: block;
        }
        .letter-open {
            display: none;
        }
        .rtan {
            background-color: white;

            width: 200px;
            height: 200px;

            background-image: url('https://upload.wikimedia.org/wikipedia/commons/e/e3/Seal_of_the_Republic_of_Korea_Marine_Corps.svg');
            background-size: cover;
            background-position: center;

            margin: 100px auto 0px auto;

            border-radius: 100px;

            border: 5px solid white;
            box-shadow: 0px 0px 10px 0px whitesmoke;

            

        }
        h1 {
            color: white;
            text-align: center;

            margin-top: 30px;
            margin-bottom: 30px;

        }
        .msgbox {
            background-color: ivory;

            width: 500px;
            margin: auto;

            color: brown;

            padding: 30px;

            font-size: 20px;
            line-height: 30px;

            box-shadow: 0px 0px 10px 0px whitesmoke;
        }
        .from {
            text-align: right;
            margin-bottom: 0px;
        }

        @media screen and (max-width: 760px) {
            .msgbox {
                width: 300px;
                padding: 20px;
            }
            .rtan {
                width: 150px;
                height: 150px;
                margin-top: 30px;
                margin-bottom: 30px;
                font-size: 28px;
            }
            h1 {
                font-size: 28px;
            }
            .envelope {
                margin: 150px auto 0px auto;
            }
        }
    </style>

    <script>

        function open_letter() {
            document.getElementsByClassName("letter-close")[0].style.display = 'none'
            document.getElementsByClassName("letter-open")[0].style.display = 'block'
        }

        
    </script>
</head>

<body>
    <div class="letter-close">
        <div class="envelope" onclick="open_letter()"></div>
        <h2 class="envelope-msg">You've Got Mail!</h2>
    </div>
    <div class="letter-open">
        <div class="rtan" onclick="go_rtan()"></div>
        <h1>Goodbye 2020!</h1>
        <div class="msgbox">
            Dear all, <br />
            2020 has been a rough <br />
            year for everyone.  <br />
            I wish you best of luck in 2021 <br />
            Happy New Year! <br />
            코로나 때문에 힘들었던 2020년은 잊고 <br />
            모두 행복한 2021년 되세요! <br />
            <p class="from">2020.12.31 Taeho</p>
        </div>
    </div>
    


</body>

</html>
