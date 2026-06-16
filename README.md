Dr Synthetica (Syntribot)

An interactive webcam-based art piece built with p5.js and ml5.js.

Dr Synthetica uses a Teachable Machine image-classification model to interpret facial expressions captured through a webcam, then initiates a simulated therapy session that adapts its questioning based on the detected emotional state.

The project explores the limitations of emotion-recognition AI and the human tendency to project understanding, empathy, and authority onto computational systems.


Features


Real-time webcam emotion classification
Teachable Machine image-model integration
Branching conversation paths based on detected emotion
Interactive text-based "therapy session"
Conversation transcript log
Restart functionality
Browser-based — no build process required



Technologies

p5.js · ml5.js · Teachable Machine · HTML · CSS · JavaScript


How It Works


The app starts the user's webcam and loads a Teachable Machine image-classification model.
A short analysis period lets the model classify the user's facial expression.
Based on the detected emotion, Dr Synthetica selects a corresponding bank of questions.
The user responds to each question through a text input.
The conversation progresses until the selected question sequence is complete.


Emotion Model

The project uses the following Teachable Machine model:

https://teachablemachine.withgoogle.com/models/HmMegiSBC/


Running the Project

This is a static site with no build step. Because webcam access requires a secure context, serve the project through a local web server rather than opening index.html directly from the file system.

bash# from the project root
python -m http.server 8000

Then open http://localhost:8000 and allow camera access when prompted.





Project Evolution

The project exists in two versions.

Current , sketch.js
HTML-based interface, conversation transcript, timed facial-expression analysis, restart functionality, and an improved interaction flow.

Original prototype , sketch.original.js
Drew interface elements directly onto the canvas and used a single p5.js input box. Served as the initial proof of concept.


Conceptual Framework

Dr Synthetica investigates how humans interact with systems that claim to interpret emotion. By reducing emotional understanding to a simple classification model and pairing it with therapeutic questioning, the project surfaces the assumptions, limitations, and biases embedded within emotion-recognition technologies.

The work draws on early conversational systems such as ELIZA while examining contemporary claims surrounding artificial intelligence and emotional intelligence.


Development Notes

AI tools were used during development for debugging, code assistance, and interface implementation. The project concept, artistic direction, interaction design, research, and written content are the author's own.


Author

Tia Tshabola
Creative Technologist, Engineer, and Artist exploring the intersection of emerging technologies, culture, identity, and human-computer interaction.
