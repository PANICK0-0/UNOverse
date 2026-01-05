<hmtl lang="en">
    <style>
        @keyframes fade {
            0% {
                transform: translateY(100px);
                opacity: 0%;
            }
            100% {
                transform: translateY(0px);
                opacity: 100%;
            }
        }
        :root {
            --color1: #e7e7e7;
            --color3: #00d;
            --color4: #99f;
            --color5: #00f;
            --bgcolor: #003;
        }
        body {
            margin: 0;
            font-family: arial;
            background: var(--bgcolor);
        }
        header {
            background: linear-gradient(to right,var(--color3),transparent) ;
            display: flex;
            flex-direction: column;
            padding: 10px;
            justify-content: center;
        }
        header p {
            color: var(--color1);
            margin: 50px;
            opacity: 75%;
        }
        header .img {
            background: url("C:/Users/siapp/OneDrive/Desktop/unoverse.png");
            background-position: center;
            background-size: 400px;
            background-repeat: no-repeat;
            width: 400px;
            height: 400px;
            margin: 50px auto;
            animation: fade 1s;
        }
        nav {
            display: flex;
            flex-direction: column;
            padding: 10px;
            gap: 10px;
        }
        .navBox,.navBox2 {
            transition: 500ms;
            background: linear-gradient(to right,var(--color3),var(--color5));
            padding: 10px;
            width: 25%;
            margin: 50px;
            border-radius: 10px;
            overflow: hidden;
            position: relative;
        }
        .navBox h1,.navBox2 h1 {
            transition: 500ms;
            color: var(--color1);
            padding: 10px;
        }
        .navBox p,.navBox2 p {
            transition: 1s;
            color: var(--color1);
            opacity: 75%;
            padding: 10px;
            text-align: justify;
            width: 250px;
        }
        .navBox .img {
            transition: 500ms;
            background: url(https://www.pngkey.com/png/full/110-1108582_uno-card-png.png);
            background-position: center;
            background-size: 200px;
            background-repeat: no-repeat;
            width: 300px;
            height: 300px;
            position: absolute;
            bottom: 0;
            right: 0;
            translate: 50% 50%;
        }
        .navBox2 .img {
            transition: 500ms;
            background: url(https://shop.mattel.com.au/cdn/shop/files/glh50.png?v=1688899789);
            background-position: center;
            background-size: 200px;
            background-repeat: no-repeat;
            width: 300px;
            height: 300px;
            position: absolute;
            bottom: 0;
            right: 0;
            translate: 50% 50%;
            rotate: 10deg;
        }
        .flex1 {
            display: flex;
            flex-direction: row;
        }
        nav h1 {
            color: var(--color1);
            margin: 50px;
        }
    </style>
    <body>
        <header>
            <div class="img">

            </div>
            <p>
                Welcome to the 
                <b>
                    UNOverse
                </b>
                , a place where everybody plays, enjoys and creates UNO Ideas.
            </p>
        </header>
        <nav>
            <h1>
                    Local Concepts
                </h1>
            <div class="flex1">
                <div class="navBox" id="NB1">
                    <div class="img" id="IM">

                    </div>
                    <h1 id="AN1">
                        UNO classic
                    </h1>
                    <p id="P1">
                        UNO Classic is the timeless card game everyone knows and loves. Match colors and numbers, use action cards to change the flow, and be the first to get rid of all your cards. Simple rules make it easy to learn, while fast gameplay keeps every round exciting.
                    </p>
                </div>
                <div class="navBox2"  id="NB2">
                    <div class="img" id="IM2">

                    </div>
                    <h1 id="AN2">
                        UNO flip
                    </h1>
                    <p id="P2">
                        UNO Flip adds a bold twist to the classic experience with double-sided cards. When a Flip card is played, the game switches to the dark side, introducing tougher penalties and surprising new actions that can change everything in seconds.
                    </p>
                </div>
            </div>
        </nav>
        <script>
            const AN1 = document.getElementById('AN1') ;
            const NB1 = document.getElementById('NB1') ;
            const P1 = document.getElementById('P1') ;
            const IM = document.getElementById('IM') ;

            const AN2 = document.getElementById('AN2') ;
            const NB2 = document.getElementById('NB2') ;
            const P2 = document.getElementById('P2') ;
            const IM2 = document.getElementById('IM2') ;

            window.addEventListener('load', () => {
                AN1
            });

            NB1.addEventListener('mouseover', () => {
                AN1.style.transform = 'translateX(10px)' ;
                P1.style.transform = 'translateX(10px)' ;

                IM.style.backgroundSize = '210px' ;
            });
            NB1.addEventListener('mouseleave', () => {
                AN1.style.transform = 'translateX(0px)' ;
                P1.style.transform = 'translateX(0px)' ;

                IM.style.backgroundSize = '200px' ;
            });


            NB2.addEventListener('mouseover', () => {
                AN2.style.transform = 'translateX(10px)' ;
                P2.style.transform = 'translateX(10px)' ;

                IM2.style.backgroundSize = '210px' ;
            });
            NB2.addEventListener('mouseleave', () => {
                AN2.style.transform = 'translateX(0px)' ;
                P2.style.transform = 'translateX(0px)' ;

                IM2.style.backgroundSize = '200px' ;
            });
        </script>
    </body>
</hmtl># UNOverse

