# open-when-surprise
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>open when...</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Pacifico&family=Poppins:wght@300;400;600&display=swap');
        body {
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            font-family: 'Poppins', sans-serif;
            text-align: center;
            color: #ff4d94;
            padding: 20px;
            text-transform: lowercase;
        }
        h1 {
            font-family: 'Pacifico', cursive;
            font-size: 40px;
            color: #ff1493;
            text-shadow: 2px 2px 5px rgba(255, 20, 147, 0.5);
        }
        .container {
            max-width: 600px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(255, 105, 180, 0.3);
        }
        .button {
            display: block;
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            font-size: 18px;
            font-weight: 600;
            color: white;
            background: #ff69b4;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            box-shadow: 0 3px 5px rgba(255, 20, 147, 0.3);
            transition: 0.3s;
        }
        .button:hover {
            background: #ff1493;
            box-shadow: 0 5px 10px rgba(255, 20, 147, 0.5);
        }
        .message {
            display: none;
            padding: 15px;
            background: #ffe4e1;
            border-radius: 10px;
            margin-top: 10px;
            box-shadow: 0 2px 5px rgba(255, 105, 180, 0.2);
            text-align: left;
        }
        .message img {
            width: 100px;
            height: auto;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <h1>open when...</h1>
    <div class="container">
        <button class="button" onclick="showMessage('happy')">you're happy!</button>
        <div id="happy" class="message">
            <p>seeing you happy makes my whole world brighter. i love that beautiful smile of yours, and i hope you know that you deserve all the happiness in the universe. soak in every bit of joy, my love. 💖</p>
        </div>
        
        <button class="button" onclick="showMessage('sad')">you're sad...</button>
        <div id="sad" class="message">
            <p>i know things might feel heavy right now, but please don’t carry it all alone. i'm always here, no matter what. please take a deep breath and know that i love you so much. sending you the tightest hug ever. 💕</p>
        </div>
        
        <button class="button" onclick="showMessage('missing')">you miss me...</button>
        <div id="missing" class="message">
            <p>i miss you too, so so much. if i could, i’d teleport to you right now and squeeze you so tight. but even when we’re apart, i’m always thinking of you. we'll be together soon, i promise. 💞</p>
        </div>
        
        <button class="button" onclick="showMessage('stressed')">you're stressed...</button>
        <div id="stressed" class="message">
            <p>i know things feel overwhelming right now, but you don’t have to do it all at once. take it one step at a time, and know that i’m always here, cheering for you, supporting you. you got this. 💖</p>
        </div>
        
        <button class="button" onclick="showMessage('sick')">you're sick...</button>
        <div id="sick" class="message">
            <p>oh no, my love is sick? 🥺 i wish i could be there to cuddle you, make you soup, and spoil you with love. please rest and take care, okay? i love you so much. sending you all my warmth and kisses. 💗</p>
        </div>

        <button class="button" onclick="showMessage('tired')">you're tired...</button>
        <div id="tired" class="message">
            <p>i know you’ve been working so hard, and i’m so proud of you. but please don’t forget to rest, okay? you deserve it. cuddle up, close your eyes, and dream of something beautiful. i love you. 💕</p>
        </div>

        <button class="button" onclick="showMessage('angry')">you're angry...</button>
        <div id="angry" class="message">
            <p>it’s okay to be upset. you don’t have to bottle it up. if you wanna talk, i’m always here. if you need space, i’ll be right here waiting. just know that i love you no matter what. 💖</p>
        </div>

        <button class="button" onclick="showMessage('proud')">you feel proud...</button>
        <div id="proud" class="message">
            <p>you did it, love! i'm so proud of you and everything you’ve accomplished. you deserve all the recognition and more. keep shining, keep being amazing. 💞</p>
        </div>

        <button class="button" onclick="showMessage('random')">you just wanna smile...</button>
        <div id="random" class="message">
            <p>here’s a little reminder: you’re the cutest, sweetest, most wonderful person in the world. and i love you endlessly. 💕</p>
        </div>

        <h2>💖 a cute little game for you 💖</h2>
        <p>guess how much i love you! (hint: it's more than infinity)</p>
        <button class="button" onclick="alert('that’s right! i love you more than words can say! 💕')">click to see the answer</button>
    </div>
    
    <script>
        function showMessage(id) {
            var messages = document.querySelectorAll('.message');
            messages.forEach(msg => msg.style.display = 'none');
            document.getElementById(id).style.display = 'block';
        }
    </script>
</body>
</html>
