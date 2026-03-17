<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>We love you</title>

  <style>
 
    .glow-box {
  background: rgba(0, 0, 0, 0.6);
  border: 1px solid rgba(255, 215, 0, 0.7); 
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 0 20px rgba(124, 58, 237, 0.7); 
  color: white;
  max-width: 500px;
  margin: 20px auto;
}
.Sarah-font {
  font-family: "Comic Sans MS", cursive;
  font-style: italic;
}

.Mags-font {
  font-family: "Arial Black", sans-serif;
  letter-spacing: 1px;
}
.Gabby-font {
  font-family: "Courier New", monospace;
  text-shadow: 0 0 8px #edcc3a;
}
.nick-font {
  font-family: "Georgia", serif;
  font-style: italic;
}
.Cinder-font {
  font-family: "Arial Black", sans-serif;
  letter-spacing: 1px;
}
.Yukis-font {
  font-family: "Courier New", monospace;
  text-shadow: 0 0 8px #7c3aed;
}


    body {
      background: #000000; 
      color: #ffffff;      
      font-family: Arial, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      text-align: center;
      
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    p {
      color: #cccccc;
      max-width: 450px;
      margin-bottom: 2rem;
    }

    
    .choice {
      display: inline-block;
      margin: 0.5rem;
      padding: 0.8rem 1.6rem;
      background: #e11d48; 
      color: #ffffff;
      text-decoration: none;
      font-weight: bold;
      border-radius: 10px;
      transition: 0.3s ease;
      box-shadow: 0 0 20px rgba(225, 29, 72, 0.6);
      cursor: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" height="32" width="32"><text y="24" font-size="24">✨</text></svg>') 0 0, auto;
    }

    .choice:hover {
      background: #000000; 
      box-shadow: 0 0 30px rgba(124, 58, 237, 0.9);
      transform: scale(1.07);
    }

    /* Gold reveal message */
    #reveal {
      margin-top: 2rem;
      font-size: 1.3rem;
      color: #facc15; /* gold */
      opacity: 0;
      transform: translateY(10px);
      transition: opacity 1.2s ease, transform 1.2s ease;
      max-width: 500px;
      line-height: 1.5;
    }

    #reveal.show {
      opacity: 1;
      transform: translateY(0);
    }
  </style>
</head>
<div class="glow-box">
<body>

  <h1>This is how much your loved</h1>
  <p>Every choice opens a letter. Pick anyone first.</p>
</div>
  <div>
    <button class="choice" onclick="revealMessage('Sarah')">Sarahs letter</button>
    <button class="choice" onclick="revealMessage('Mags')">Mags letter</button>
    <button class="choice" onclick="revealMessage('Mags pt2')">Mags letter pt2</button>
    <button class="choice" onclick="revealMessage('Nick')">Nicks letter</button>
    <button class="choice" onclick="revealMessage('Gabby')">Gabbys letter</button>
    <button class="choice" onclick="revealMessage('Cinder')">cinders letter</button>
    <button class="choice" onclick="revealMessage('Yuki')">yukis letter</button> 
  </div>

   <div id="reveal"></div>

  <script>
    function revealMessage(path) {
      const reveal = document.getElementById('reveal');
      reveal.classList.remove("show", "Sarah-font", "Mags-font","Nick-font","Gabby-font", "Cinder-font", "Yuki-font", "Jordi-font" );

      let text = "";

      if (path === "Sarah") {
        text = `✨😏 Hey Father, I wanted to let you know I am grateful for all you have done for me, I appreciate you being here and honestly there are not enough words to describe my gratitude towards you. 
        I am grateful you are my friend and my father, and I hope your birthday is the best one yet! 
        #BestFatherOfTheYear #BestVoiceActor #WRizz - Your Daughter. 😏
       ✨`;reveal.classList.add("Gabby-font");
      }

      if (path === "Mags") {
        text = `✨ To my best friend, a true gentleman, and my protector... I will watch over and take
        care of you all the days that we live this life together. There is no strength that's strong enough 
        that could tear you out from my heart. There isn't a single thing you could ever do to make me hate you.
        I love you with all of my heart, and all I want is for you to always remember that, and to always be safe.
        I know you already know, but I don't care. I'll say it til the day I die. You are the sweetest, most caring 
        person I know.(cont'd)✨`;
      reveal.classList.add("Mags-font");
      }
      if (path === "Mags pt2") {
        text = `✨You choose to be good and fair, even when so often no one is good or fair to you. You find a 
        way to love people somehow in a world full of hate and lust. Your spirit burns hotter with faith than anyone
        that I have ever known. You set me ablaze with your compassion. You are my brother, and my mentor, and best friend.
        You will never know how much you mean to me, and I think that is the most painful part. We are literally born from 
        suffering and live through it still, and yet… I feel at peace. I could go the rest of my life without another person's
        love and die happy that God gave us each other, you for me, and me for you, orphans in an orphanage, different blood but
        bound together in a strange twist of fate. All the pain of my days here on this little pinpoint in a vast universe of 
        nothingness, and I will look back and say I’d do it all again just to live this short life with you.
        - Maggizine Celeste Smith <3 ✨`;
      reveal.classList.add("Mags-font");
      }
      if (path === "Nick") {
        text = `✨ For putting up with my BS and retardation you are the realest mf. 🫡`;
        reveal.classList.add("Nick-font");
      }
      if (path === "Gabby") {
        text = `✨Hai Blake, \\ I just want you to know how much your loved and appreciated. you are such a kind, caring, loving, lovable,
        amazing person and I want to thank you for everything you've done for me. Youv've help me in so many ways and im so greatful to 
        have you in my life. You mak me so happy and im so glad sarah has someone like you in life. You are a great singer/musicain, author,
        voice actor, gamer and so much more and i cant wait til you get all the good you deserve in life. I love you and Happy Birthday I hope
        you get blessed with many more and i hope they get better every time.❤️ `;reveal.classList.add("Gabby-font");
      }

      if (path === "Cinder") {
        text = `✨“dear victor, i hope u have ur having a great birthday so far. i’m writing this in participation of gabbys gift to u. 

       victor u are one of the bestest friends ive had in a very long time and i am so grateful to have met u. ur honestly one of the best people ive ever met… and i mean that. 

       thank u for being u and everything that comes with that… ur kindness, love, care, givingness, respect, compassion, strength, laughter and so much more. 

        there’s not enough words to describe the kind of gratitude and appreciation i have for u. ur one of a kind and i feel honored to be ur friend… thank u for all u do and continue to do. 

        much love victor, 

        ~natalie” ✨`;
        reveal.classList.add("Cinder-font");
      }

      if (path === "Yuki") {
        text = `✨ Hey Tony, \\

       I just realized we’ve been friends for a whole year now, which honestly feels kind of crazy to think about. I’m really glad we became friends and that we got to know each other the way we did.

       I’m really happy to see you doing what you love with voice acting. It’s awesome seeing you go after something you’re passionate about, and I hope you keep going with it. I also really hope you continue working on your novel, since that’s how we first started becoming friends in the first place, and that will always be special to me.

       And I can’t forget all the late night gaming sessions, especially league. (Fuck Pyke) Those nights staying up, playing, laughing, and just talking are honestly some really great memories for me.

       I’m really grateful for our friendship and I hope we make a lot more memories like that in the future.`;
        reveal.classList.add("Yuki-font");
      }
      reveal.textContent = text;

      setTimeout(() => {
        reveal.classList.add("show");
      }, 50);
    }
  </script>

</body>
</html>
