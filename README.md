<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>MA Agency - Elite Covert Operations</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #121212;
            color: #e1e1e1;
            margin: 0;
            padding: 0;
            overflow: hidden;
        }
        header {
            background-color: #0d0d0d;
            padding: 40px 20px;
            text-align: center;
            position: relative;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.8);
        }
        header h1 {
            margin: 0;
            font-size: 4rem;
            color: #ff4f4f;
            text-shadow: 3px 3px 15px black;
        }
        header p {
            font-size: 1.4rem;
            font-style: italic;
            color: #aaa;
            margin-top: 10px;
        }
        nav {
            background-color: #1a1a1a;
            padding: 15px 20px;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.6);
        }
        nav a {
            color: #fff;
            padding: 15px 25px;
            text-decoration: none;
            text-transform: uppercase;
            font-weight: bold;
            letter-spacing: 2px;
            margin: 0 15px;
            display: inline-block;
        }
        nav a:hover {
            background-color: #ff4f4f;
            color: black;
            transform: scale(1.1);
        }
        .hero {
            background: url('https://yourimagepath.com/agent47-bg.jpg') no-repeat center center/cover;
            height: 100vh;
            text-align: center;
            padding-top: 80px;
            color: white;
            position: relative;
        }
        .hero h2 {
            font-size: 3.5rem;
            color: #ff4f4f;
            text-shadow: 3px 3px 15px black;
        }
        .hero p {
            font-size: 1.6rem;
            margin-top: 20px;
            color: #ddd;
        }
        .cta-button {
            background-color: #444;
            color: white;
            padding: 18px 40px;
            text-decoration: none;
            font-size: 1.2rem;
            border-radius: 5px;
            margin-top: 30px;
            display: inline-block;
            transition: background-color 0.3s ease, transform 0.3s ease;
        }
        .cta-button:hover {
            background-color: #ff4f4f;
            color: black;
            transform: scale(1.1);
        }
        .agent-profile {
            background-color: #222;
            color: white;
            padding: 60px 30px;
            text-align: center;
        }
        .agent-profile h2 {
            font-size: 3rem;
            color: #ff4f4f;
            text-shadow: 3px 3px 10px black;
        }
        .agent-profile p {
            font-size: 1.3rem;
            line-height: 1.6;
        }
        footer {
            background-color: #111;
            color: #999;
            text-align: center;
            padding: 25px 10px;
            font-size: 1.1rem;
            position: fixed;
            width: 100%;
            bottom: 0;
            box-shadow: 0 -2px 5px rgba(0, 0, 0, 0.6);
        }

        /* Custom audio controls */
        .audio-control {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: #444;
            padding: 10px 20px;
            border-radius: 5px;
            display: flex;
            align-items: center;
            cursor: pointer;
        }

        .audio-control span {
            color: white;
            font-size: 1.2rem;
            margin-left: 10px;
        }
    </style>
</head>
<body>

<!-- Background Music -->
<audio id="bg-music" loop autoplay>
    <source src="YOUR_MUSIC_FILE_PATH.mp3" type="audio/mp3">
    Your browser does not support the audio element.
</audio>

<header>
    <h1>MA Agency</h1>
    <p>Elite Covert Operations | The Truth is in the Shadows</p>
</header>

<nav>
    <a href="#about">About</a>
    <a href="#agents">Agents</a>
    <a href="#contact">Contact</a>
</nav>

<div class="hero">
    <h2>Silent. Deadly. Unseen.</h2>
    <p>MA Agency operates in the shadows, delivering results with precision. When the world is asleep, we move.</p>
    <a href="#contact" class="cta-button">Contact Us</a>
</div>

<section id="about" class="agent-profile">
    <h2>About MA Agency</h2>
    <p>Founded under total secrecy, MA Agency has been solving the most sensitive and dangerous cases for decades. Operating in the shadows, our agents specialize in missions that leave no trace, bringing justice where others fear to tread.</p>
</section>

<section id="agents" class="agent-profile">
    <h2>Our Agents</h2>
    <p><strong>Leads Agent 47:</strong> The top agent of MA Agency. Known for his precision and unmatched skills. He does not miss his target.</p>
    <p><strong>Information Collector 7:</strong> A master of gathering intel. If the information exists, Agent 7 will find it.</p>
    <p><strong>Agent 37 & 27:</strong> Operatives who specialize in elimination and intelligence gathering. No one knows their true identities, but they never fail.</p>
</section>

<section id="contact" class="agent-profile">
    <h2>Contact Us</h2>
    <p>If you're in need of the utmost discretion, get in touch with us. We operate in silence and act with precision. You can trust no one but MA Agency.</p>
    <a href="mailto:contact@maagency.com" class="cta-button">Email Us Securely</a>
</section>

<footer>
    <p>&copy; 2025 MA Agency | Elite Covert Operations</p>
</footer>

<!-- Audio Control Button -->
<div class="audio-control" onclick="toggleAudio()">
    <span id="audio-status">Music On</span>
</div>

<script>
    const audioElement = document.getElementById('bg-music');
    const audioStatus = document.getElementById('audio-status');

    function toggleAudio() {
        if (audioElement.paused) {
            audioElement.play();
            audioStatus.innerText = "Music On";
        } else {
            audioElement.pause();
            audioStatus.innerText = "Music Off";
        }
    }
</script>

</body>
</html>
