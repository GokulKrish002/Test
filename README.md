    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <style>
            .effect_hover{
                position: relative;
                width: 200px;
                height: 300px;
                margin-left: 100px;
                margin-top: 100px;
            }
            .effect_hover::after{
                content: "";
                position:absolute;
                top: 0;
                left: 0;
                height: 100%;
                width: 100%;
                background-color: rgb(95, 95, 95);
                /* animation: hover_efft 2s;*/
                opacity: 50%; 
                top: 50%;
                    left: 50%;
                    height: 0%;
                    width: 0%;
            }
            .effect_hover::before{
                content: "";
                position:absolute;
                top: -3.5%;
                left: -5%;
                height: 107%;
                width: 110%;
                background-color: aqua;
                clip-path: polygon(0% 0%, 0% 100%, 3% 100%, 3% 2%, 97% 2%, 97% 98%, 3% 98%, 3% 100%, 100% 100%, 100% 0%);
                /* animation: hover_efft_2 2s; */
                opacity: 50%;
                top: -3.5%;
                    left: -5%;
                    height: 107%;
                    width: 110%;
            }

            /* @keyframes hover_efft {
                0%{height: 0px;width: 0px;margin-left: 100px;margin-top: 150px;}
                100%{height: 300px;width: 200px;margin-left: 0px;margin-top: 0px;}            
            }
            @keyframes hover_efft_2 {
                0%{
                    top: 50%;
                    left: 50%;
                    height: 0%;
                    width: 0%;
                }
                40%{
                    top: 50%;
                    left: 50%;
                    height: 0%;
                    width: 0%;
                }
                100%{
                    top: -3.5%;
                    left: -5%;
                    height: 107%;
                    width: 110%;
                }    
                        
            } */

            .effect_hover:hover::before{
                top: -3.5%;
                    left: -5%;
                    height: 107%;
                    width: 110%;
            }
            .effect_hover:hover::after{
                height: 300px;width: 200px;margin-left: 0px;margin-top: 0px;
            }
        </style>
        <div class="effect_hover">
            <img src="https://picsum.photos/200/300" alt="">
        </div>
    </body>
    </html>
