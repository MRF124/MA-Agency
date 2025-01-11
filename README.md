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
            background-color: #0d0d0d;
            color: #e1e1e1;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
        }
        header {
            background-color: #1a1a1a;
            padding: 80px 20px;
            text-align: center;
            position: relative;
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.9);
        }
        header h1 {
            margin: 0;
            font-size: 4.8rem;
            color: #e00000;
            text-shadow: 5px 5px 25px black;
        }
        header p {
            font-size: 1.5rem;
            font-style: italic;
            color: #aaa;
            margin-top: 15px;
            letter-spacing: 1px;
        }
        nav {
            background-color: #222;
            padding: 20px 25px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.8);
        }
        nav a {
            color: #fff;
            padding: 20px 30px;
            text-decoration: none;
            text-transform: uppercase;
            font-weight: bold;
            letter-spacing: 2px;
            margin: 0 20px;
            display: inline-block;
            border-radius: 5px;
            position: relative;
            transition: background-color 0.3s ease, transform 0.3s ease;
        }
        nav a::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(255, 0, 0, 0.2);
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        nav a:hover {
            background-color: #e00000;
            color: black;
            transform: scale(1.1);
        }
        nav a:hover::before {
            opacity: 1;
        }
        .hero {
            background: url('https://yourimagepath.com/agent47-bg.jpg') no-repeat center center/cover;
            height: 100vh;
            text-align: center;
            padding-top: 120px;
            color: white;
            position: relative;
            background-color: #0a0a0a;
        }
        .hero h2 {
            font-size: 4.5rem;
            color: #e00000;
            text-shadow: 6px 6px 30px black;
        }
        .hero p {
            font-size: 1.7rem;
            margin-top: 20px;
            color: #ddd;
            letter-spacing: 1px;
        }
        .cta-button {
            background-color: #333;
            color: white;
            padding: 20px 50px;
            text-decoration: none;
            font-size: 1.4rem;
            border-radius: 5px;
            margin-top: 50px;
            display: inline-block;
            letter-spacing: 2px;
            transition: background-color 0.4s ease, transform 0.3s ease, box-shadow 0.3s ease;
        }
        .cta-button:hover {
            background-color: #e00000;
            color: black;
            transform: scale(1.1);
            box-shadow: 0 6px 30px rgba(0, 0, 0, 0.8);
        }
        .agent-profile {
            background-color: #121212;
            color: white;
            padding: 80px 40px;
            text-align: center;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.8);
        }
        .agent-profile h2 {
            font-size: 3.5rem;
            color: #e00000;
            text-shadow: 4px 4px 20px black;
        }
        .agent-profile p {
            font-size: 1.4rem;
            line-height: 1.8;
            letter-spacing: 0.5px;
            margin-top: 10px;
        }
        footer {
            background-color: #111;
            color: #aaa;
            text-align: center;
            padding: 25px 15px;
            font-size: 1.2rem;
            position: fixed;
            width: 100%;
            bottom: 0;
            box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.7);
        }
        .audio-control {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background-color: #333;
            padding: 12px 25px;
            border-radius: 5px;
            display: flex;
            align-items: center;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.3s ease;
        }
        .audio-control:hover {
            background-color: #e00000;
            transform: scale(1.05);
        }
        .audio-control span {
            color: white;
            font-size: 1.2rem;
            margin-left: 12px;
        }
        .target-section {
            background-color: #121212;
            padding: 70px 30px;
            text-align: center;
            color: #e1e1e1;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.8);
        }
        .target-section h2 {
            font-size: 3.5rem;
            color: #e00000;
            text-shadow: 4px 4px 25px black;
        }
        .target-list {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-top: 25px;
        }
        .target-list p {
            font-size: 1.6rem;
            background-color: #333;
            padding: 12px 25px;
            border-radius: 6px;
            margin: 12px 0;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.7);
            letter-spacing: 1px;
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
    <a href="#target">Target</a>
    <a href="#contact">Contact</a>
</nav>

<div class="hero">
    <h2>Silent. Deadly. Unseen.</h2>
    <p>We deal in shadows, where only fear remains. Precision is our language, silence our weapon.</p>
    <a href="#contact" class="cta-button">Contact Us</a>
</div>

<section id="about" class="agent-profile">
    <h2>About MA Agency</h2>
    <p>Founded under absolute secrecy, MA Agency solves the most dangerous cases with a cold, calculated approach. Our agents are shadows—seen by no one, feared by all.</p>
</section>

<section id="agents" class="agent-profile">
    <h2>Our Agents</h2>
    <p><strong>Leads Agent 47:</strong> The most dangerous of them all. Cold. Silent. Relentless.</p>
    <p><strong>Information Collector 7:</strong> Every secret has its price. No information escapes his grasp.</p>
    <p><strong>Agent 37 & 27:</strong> Operatives whose identities are lost in the dark. They come, they eliminate, they vanish.</p>
</section>

<section id="target" class="target-section">
    <h2>Target List</h2>
    <div class="target-list">
        <p>Chonchol</p>
        <p>Tonmoy</p>
        <p>Rohom</p>
        <p>Hujaifa</p>
        <p>Aiman</p>
    </div>
</section>

<section id="contact" class="agent-profile">
    <h2>Contact Us</h2>
    <p>If you need discretion and results, reach out. Trust no one else but MA Agency.</p>
    <p><strong>Phone:</strong> 01308769690 | 01989747850</p>
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
