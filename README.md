# jarvis
JARVIS — Conversational AI Assistant
A full-stack AI assistant with real-time voice input, 3D neural network visualization, and persistent conversation context — built on the Claude API.

What it does
	•	Voice input — speak naturally; transcribed and sent to Claude in real time
	•	3D neural visualization — WebGL-rendered network that responds to conversation state
	•	Persistent context — conversation history maintained across the session
	•	Claude API — powered by Anthropic’s claude-sonnet model for natural language reasoning
	•	ElevenLabs voice synthesis — responses spoken back with realistic voice output

Tech Stack
|Layer       |Technology                     |
|------------|-------------------------------|
|Frontend    |React, TypeScript, Tailwind CSS|
|3D Rendering|WebGL                          |
|AI          |Claude API (Anthropic)         |
|Voice       |ElevenLabs API, Web Speech API |
|Build       |Vite                           |

Getting Started 
git clone https://github.com/Vraj4592/jarvis
cd jarvis
npm install

Create a .env file:
VITE_ANTHROPIC_API_KEY=your_claude_api_key
VITE_ELEVENLABS_API_KEY=your_elevenlabs_api_key

bash
npm run dev

Project Structure
src/
├── components/
│   ├── NeuralNetwork.tsx     # WebGL 3D visualization
│   ├── VoiceInput.tsx        # Web Speech API integration
│   └── ChatInterface.tsx     # Main conversation UI
├── hooks/
│   └── useClaudeAPI.ts       # Claude API calls + context management
├── lib/
│   └── elevenlabs.ts         # Voice synthesis
└── App.tsx

Why I built this
Wanted to explore what a genuinely useful AI assistant UI looks like beyond a chat box — combining voice, visual feedback, and a model that can actually reason. The 3D visualization responds to conversation depth and token usage in real time.