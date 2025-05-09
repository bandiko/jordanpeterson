<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jordan Peterson Speech Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: #111;
            color: #f0f0f0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            padding: 20px;
        }
        h1 {
            color: #e63946;
        }
        textarea, input, button {
            width: 100%;
            max-width: 600px;
            margin: 10px 0;
            padding: 10px;
            font-size: 16px;
            border-radius: 5px;
            border: none;
        }
        button {
            background-color: #457b9d;
            color: white;
            cursor: pointer;
        }
        button:hover {
            background-color: #1d3557;
        }
        #speech {
            white-space: pre-wrap;
            background: #222;
            padding: 15px;
            border-radius: 8px;
            margin-top: 20px;
            max-width: 800px;
            width: 100%;
        }
        #voiceSelect {
            margin: 10px 0;
        }
    </style>
</head>
<body>
    <h1>Jordan Peterson Speech Generator</h1>
    <input id="topic" type="text" placeholder="Enter a topic (e.g., Responsibility)" />
    <button onclick="generateSpeech()">Generate Speech</button>
    <button onclick="playSpeech()">Play Audio</button>
    <div id="speech"></div>
    
    <select id="voiceSelect">
        <option value="">Select a voice</option>
    </select>

    <script>
        let lastSpeech = "";
        let voices = [];
        let selectedVoice = null;

        // Function to load voices once they are available
        function loadVoices() {
            voices = speechSynthesis.getVoices();
            if (voices.length === 0) {
                setTimeout(loadVoices, 100); // Retry if voices aren't available yet
            } else {
                populateVoiceList();
            }
        }

        // Populate voice selection dropdown
        function populateVoiceList() {
            const voiceSelect = document.getElementById('voiceSelect');
            voiceSelect.innerHTML = '<option value="">Select a voice</option>'; // Reset options

            voices.forEach(voice => {
                const option = document.createElement('option');
                option.value = voice.name;
                option.textContent = `${voice.name} (${voice.lang})`;
                voiceSelect.appendChild(option);
            });

            // Set the default selected voice to the first one
            if (voices.length > 0) {
                voiceSelect.value = voices[0].name;
                selectedVoice = voices[0];
            }
        }

        // Wait for voices to load initially
        loadVoices();

        // Function to generate the speech based on the input topic
        function generateSpeech() {
            const topic = document.getElementById('topic').value.trim();
            const speechOutput = document.getElementById('speech');

            if (!topic) {
                speechOutput.textContent = 'Please enter a topic.';
                return;
            }

            // The speech generated based on the input topic
            const speech = `Now listen — when we talk about ${topic}, we're not just dealing with a casual idea, alright? We're dealing with something fundamental, something that speaks to the very structure of our society. 

The world — it's chaotic. And without ${topic}, without some guiding principle to orient yourself, you’re just floundering in the abyss. And people don't realize — they really don't — how deep that abyss goes.

So what do you do? You take responsibility. You confront ${topic} with honesty and strength. You tell the truth — or at least, you don't lie. And you voluntarily shoulder the burden, because that’s what gives your life meaning.

Meaning, after all, is what protects you from suffering — from malevolence, from despair. And ${topic}? It’s a moral imperative, not a suggestion. Without it, we devolve. But with it? We stand a chance at order, and maybe even something like redemption.`;

            // Display the generated speech in the HTML
            speechOutput.textContent = speech;
            lastSpeech = speech;
        }

        // Function to play the generated speech
        function playSpeech() {
            if (!lastSpeech) {
                alert("Please generate a speech first.");
                return;
            }

            if (!selectedVoice) {
                alert("Please select a voice.");
                return;
            }

            // Create the speech synthesis object
            const speech = new SpeechSynthesisUtterance(lastSpeech);
            speech.lang = selectedVoice.lang;  // Use the selected voice's language
            speech.voice = selectedVoice; // Use the selected voice

            // Play the speech using the browser's speech synthesis
            speechSynthesis.speak(speech);
        }

        // Handle voice selection
        document.getElementById('voiceSelect').addEventListener('change', function () {
            const selectedVoiceName = this.value;
            selectedVoice = voices.find(voice => voice.name === selectedVoiceName);
        });
    </script>
</body>
</html>
