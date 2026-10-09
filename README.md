# VoxAura AI Voice Studio — 3D Plus

## Requirements
- Node.js LTS
- An ElevenLabs account and API key

## Setup (Windows PowerShell)
1. Extract the ZIP and open the extracted folder in VS Code.
2. Copy `.env.example` to a new file named `.env` in the project root (same folder as `package.json`).
3. Add your ElevenLabs API key to `ELEVENLABS_API_KEY` in `.env`. Keep this file private. Confirm the voice IDs are available in your ElevenLabs account.
4. Open Terminal → New Terminal and run:
   ```powershell
   npm.cmd install
   npm.cmd run dev
   ```
5. Open the Vite URL shown in the terminal (normally http://localhost:5173).

## What's updated
- Stronger mouse-driven 3D tilt: up to 24° X and 30° Y rotation with perspective and lift.
- Much less glow: restrained shadows and ambient color, no intense neon pulse/glow loops.
- Larger typography throughout for improved readability.
- Tilted voice option controls and depth on the preview/audio controls.
- Generation-in-progress tilt/wave animation and MP3 download after successful generation.
- API key remains server-side; never put it in frontend code or commit `.env`.

The text-to-speech backend uses ElevenLabs' `eleven_multilingual_v2` model. Voice IDs in `.env.example` are examples and may need changing to IDs available in your account.
