<To Farra Wahyu T. W.>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anniversary Celebration</title>
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            text-align: center;
            background: linear-gradient(to right, #e0eafc, #cfdef3);
            margin: 0;
            padding: 0;
            overflow-x: hidden;
        }
        .container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
            background: #ffffff;
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
            position: relative;
            overflow: hidden;
            z-index: 1;
        }
        .container:before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle, rgba(255, 223, 186, 0.2), rgba(255, 223, 186, 0.1));
            z-index: -1;
            pointer-events: none;
        }
        h1 {
            color: #2c3e50;
            font-size: 2.5em;
            margin: 0;
            padding: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
            animation: fadeIn 2s ease-out;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .section {
            margin: 20px 0;
            position: relative;
        }
        .section h2 {
            color: #007bff;
            font-size: 2em;
            margin-bottom: 10px;
            font-weight: 500;
            border-bottom: 2px solid #007bff;
            display: inline-block;
            padding-bottom: 5px;
            transition: color 0.3s, transform 0.3s;
        }
        .section h2:hover {
            color: #0056b3;
            transform: translateY(-5px);
        }
        .section img, .section video, .section audio {
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .section img:hover, .section video:hover, .section audio:hover {
            transform: scale(1.05);
            box-shadow: 0 12px 24px rgba(0, 0, 0, 0.4);
        }
        video, audio {
            display: block;
            margin: 20px auto;
            max-width: 100%;
        }
        .button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 8px;
            font-size: 1em;
            transition: background-color 0.3s, transform 0.3s;
            margin-top: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .button:hover {
            background-color: #0056b3;
            transform: translateY(-2px);
        }
        .overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            color: #fff;
            display: flex;
            justify-content: center;
            align-items: center;
            visibility: hidden;
            opacity: 0;
            transition: opacity 0.5s, visibility 0.5s;
            z-index: 1000;
        }
        .overlay.active {
            visibility: visible;
            opacity: 1;
        }
        .overlay-content {
            width: 90%;
            height: 90%;
            background: #343a40;
            padding: 10px;
            border-radius: 15px;
            position: relative;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        .overlay-content img {
            max-width: 100%;
            max-height: 100%;
            object-fit: contain;
        }
        .close {
            position: absolute;
            top: 10px;
            right: 10px;
            font-size: 1.5em;
            cursor: pointer;
            color: #f8f9fa;
            transition: color 0.3s;
        }
        .close:hover {
            color: #dc3545;
        }
        .card {
            background: #ffffff;
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
            margin: 10px;
            padding: 10px;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .card:hover {
            transform: scale(1.03);
            box-shadow: 0 12px 24px rgba(0, 0, 0, 0.3);
        }
        .card img {
            width: 100%;
            border-radius: 15px;
        }
        .fallback {
            font-size: 1em;
            color: #888;
            margin-top: 10px;
        }
        @media (max-width: 768px) {
            h1 {
                font-size: 2em;
            }
            .section h2 {
                font-size: 1.5em;
            }
            .button {
                font-size: 0.9em;
                padding: 8px 16px;
            }
            .card {
                margin: 10px 5px;
                padding: 10px 5px;
            }
        }
        @media (max-width: 480px) {
            h1 {
                font-size: 1.5em;
            }
            .section h2 {
                font-size: 1.2em;
            }
            .button {
                font-size: 0.8em;
                padding: 6px 12px;
            }
            .card {
                margin: 5px;
                padding: 5px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Happy Anniversary!</h1>
        
        <!-- Photo Section -->
        <div class="section">
            <h2>Our Special Photo</h2>
            <div class="card">
                <img src="your-photo.jpg" alt="Anniversary Photo" id="photo">
                <p>Here's a cherished memory from our journey together.</p>
            </div>
        </div>

        <!-- Songs Section -->
        <div class="section">
            <h2>Our Favorite Songs</h2>
            <div class="card">
                <audio controls>
                    <source src="song1.mp3" type="audio/mpeg">
                    Your browser does not support the audio element. <a href="song1.mp3" download>Download Song 1</a>
                </audio>
                <p>Enjoy this tune that always brings back memories.</p>
            </div>
            <div class="card">
                <audio controls>
                    <source src="[song2.mp3](https://github.com/fakfathur/fakfathur.github.io/blob/main/Farra's%20Smile.mp3)" type="audio/mpeg">
                    Your browser does not support the audio element. <a href="[song2.mp3](https://github.com/fakfathur/fakfathur.github.io/blob/main/Farra's%20Smile.mp3)" download>Download Song 2</a>
                </audio>
                <p>A melody that means so much to us.</p>
            </div>
        </div>

        <!-- Video Section -->
        <div class="section">
            <h2>Watch Our Video</h2>
            <div class="card">
                <video controls>
                    <source src="video.mp4" type="video/mp4">
                    Your browser does not support the video tag. <a href="video.mp4" download>Download Video</a>
                </video>
                <p>Relive the special moments with this video.</p>
            </div>
        </div>

        <a href="#" class="button" id="show-overlay">Click for a Surprise</a>
    </div>

    <!-- Overlay for Surprise -->
    <div class="overlay" id="overlay">
        <div class="overlay-content">
            <span class="close" id="close-overlay">&times;</span>
            <img src="surprise.jpg" alt="Surprise Image">
        </div>
    </div>

    <script>
        document.getElementById('show-overlay').addEventListener('click', function(event) {
            event.preventDefault();
            document.getElementById('overlay').classList.add('active');
        });

        document.getElementById('close-overlay').addEventListener('click', function() {
            document.getElementById('overlay').classList.remove('active');
        });

        window.addEventListener('click', function(event) {
            if (event.target === document.getElementById('overlay')) {
                document.getElementById('overlay').classList.remove('active');
            }
        });
    </script>
</body>
</html>
