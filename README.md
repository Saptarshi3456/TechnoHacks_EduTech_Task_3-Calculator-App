# TechnoHacks_EduTech_Task_3-Calculator-App

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" href="style.css">

    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">

    <script src="https://kit.fontawesome.com/cb518267ee.js" crossorigin="anonymous"></script>

</head>

<body>

    <section class="container">
        <div class="mobile-mock">
            <header>
                <div id="time" class="left"></div>
                <div class="center">
                    <div class="speaker"></div>
                    <div class="camera"></div>
                </div>
                <div class="right">
                    <img src="Images/wifi.png">
                    <img src="Images/network.png">
                    <img src="Images/battery.png">
                </div>
            </header>

            <main class="calculator">
                <form>
                    <div class="cal-screen">
                        <input type="text" name="display">
                    </div>
                    <div>
                        <input type="button" value="AC" class="grey" onclick="display.value = ''" onkeypress="">
                        <input type="button" value="DE" class="grey" onclick="display.value = display.value.toString().slice(0,-1)">
                        <input type="button" value="%" class="grey" onclick="display.value += '%'">
                        <input type="button" value="/" class="grey" onclick="display.value += '/'">
                    </div>
                    <div>
                        <input type="button" value="7" class="num-key" onclick="display.value += '7'" onkeypress="display.value += '7'">
                        <input type="button" value="8" class="num-key" onclick="display.value += '8'" onkeypress="display.value += '8'">
                        <input type="button" value="9" class="num-key" onclick="display.value += '9'" onkeypress="display.value += '9'">
                        <input type="button" value="*" class="grey" onclick="display.value += '*'" onkeypress="display.value += '*'">
                    </div>
                    <div>
                        <input type="button" value="4" class="num-key" onclick="display.value += '4'" onkeypress="display.value += '4'">
                        <input type="button" value="5" class="num-key" onclick="display.value += '5'" onkeypress="display.value += '5'">
                        <input type="button" value="6" class="num-key" onclick="display.value += '6'" onkeypress="display.value += '6'">
                        <input type="button" value="-" class="grey" onclick="display.value += '-'" onkeypress="display.value += '-'">
                    </div>
                    <div>
                        <input type="button" value="1" class="num-key" onclick="display.value += '1'" onkeypress="display.value += '1'">
                        <input type="button" value="2" class="num-key" onclick="display.value += '2'" onkeypress="display.value += '2'">
                        <input type="button" value="3" class="num-key" onclick="display.value += '3'" onkeypress="display.value += '3'">
                        <input type="button" value="+" class="grey" onclick="display.value += '+'" onkeypress="display.value += '+'">
                    </div>
                    <div>
                        <input type="button" value="00" class="num-key"onclick="display.value += '00 '" onkeypress="display.value += '0'">
                        <input type="button" value="0" class="num-key" onclick="display.value += '0'" onkeypress="display.value += '0'">
                        <input type="button" value="." class="num-key" onclick="display.value += '.'" onkeypress="display.value += '.'">
                        <input type="button" value="=" class="orange" onclick="display.value = eval(display.value)">
                    </div>
                </form>
            </main>

            <footer>
                <div><svg class="icon bar" xmlns="http://www.w3.org/2000/svg"
                        viewBox="0 0 448 512"><!--! Font Awesome Pro 6.3.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. -->
                        <path
                            d="M0 96C0 78.3 14.3 64 32 64H416c17.7 0 32 14.3 32 32s-14.3 32-32 32H32C14.3 128 0 113.7 0 96zM0 256c0-17.7 14.3-32 32-32H416c17.7 0 32 14.3 32 32s-14.3 32-32 32H32c-17.7 0-32-14.3-32-32zM448 416c0 17.7-14.3 32-32 32H32c-17.7 0-32-14.3-32-32s14.3-32 32-32H416c17.7 0 32 14.3 32 32z" />
                    </svg>
                </div>

                <div><svg class="icon home" xmlns="http://www.w3.org/2000/svg"
                        viewBox="0 0 576 512"><!--! Font Awesome Pro 6.3.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. -->
                        <path
                            d="M575.8 255.5c0 18-15 32.1-32 32.1h-32l.7 160.2c0 2.7-.2 5.4-.5 8.1V472c0 22.1-17.9 40-40 40H456c-1.1 0-2.2 0-3.3-.1c-1.4 .1-2.8 .1-4.2 .1H416 392c-22.1 0-40-17.9-40-40V448 384c0-17.7-14.3-32-32-32H256c-17.7 0-32 14.3-32 32v64 24c0 22.1-17.9 40-40 40H160 128.1c-1.5 0-3-.1-4.5-.2c-1.2 .1-2.4 .2-3.6 .2H104c-22.1 0-40-17.9-40-40V360c0-.9 0-1.9 .1-2.8V287.6H32c-18 0-32-14-32-32.1c0-9 3-17 10-24L266.4 8c7-7 15-8 22-8s15 2 21 7L564.8 231.5c8 7 12 15 11 24z" />
                    </svg>
                </div>

                <div><svg class="icon back" xmlns="http://www.w3.org/2000/svg"
                        viewBox="0 0 320 512"><!--! Font Awesome Pro 6.3.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. -->
                        <path
                            d="M267.5 440.6c9.5 7.9 22.8 9.7 34.1 4.4s18.4-16.6 18.4-29V96c0-12.4-7.2-23.7-18.4-29s-24.5-3.6-34.1 4.4l-192 160L64 241V96c0-17.7-14.3-32-32-32S0 78.3 0 96V416c0 17.7 14.3 32 32 32s32-14.3 32-32V271l11.5 9.6 192 160z" />
                    </svg>
                </div>
            </footer>
        </div>
    </section>






















    <script src="app.js"></script>
</body>

</html>
