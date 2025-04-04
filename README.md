# 🎬✨ Welcome to the Video-Generator-with-AI Repository! 🚀🌟

- In this project, you input a topic, and then separate prompts for both audio and video are generated, allowing you to edit them before finalizing. Once the prompts are set, a complete video with synchronized audio is created. Additionally, you can enhance the final output by adding a song of your choice, integrating a talking face for more engaging visuals, and including subtitles in the video.
- The code is in spanish, but with a few changes it will work on other languages
- Requires Google Gemini and Elevenlabs API keys (free trials available)



- Watch some of the videos 
<div align="center">
  <a href="https://igna-s.github.io/Video-Generator-with-AI/Previews/video_preview.html" target="_blank">
    <img src="https://img.shields.io/static/v1?label=Watch&message=Video_I&color=yellow&logo=youtube">
  </a> &ensp;
  <a href="https://igna-s.github.io/Video-Generator-with-AI/Previews/video_previewII.html" target="_blank">
    <img src="https://img.shields.io/static/v1?label=Watch&message=Video_II&color=blue&logo=youtube">
  </a> &ensp;
  <a href="https://igna-s.github.io/Video-Generator-with-AI/Previews/video_previewIII.html" target="_blank">
    <img src="https://img.shields.io/static/v1?label=Watch&message=Video_III&color=orange&logo=youtube">
  </a> &ensp;
</div>


---

## 📂 Project Structure

- **Tests:**  
  Contains sample cropped videos that demonstrate the final output without modifying the prompting process.

- **Old Versions and Trials:**  
  This folder houses previous trials and various image models used during development. If you have an Nvidia graphics card with more than 15GB of VRAM, you can try Wan-Ai.

- **The Final Project & The Final Project Better Graphics:**  
  These directories contain the main generators:
  - **The Final Project:** Uses **Stable Diffusion XL** for image generation.
  - **The Final Project Better Graphics:** Uses **Sana** to produce even more refined and impressive imagery.
  
  Each one of them has **two modules** (Audio and Video Generator and Subtitle, Music and Talking Head Generator) and an extra section to test the correct operation of some libraries, such as yt-dlp.

---

## 1️⃣ Audio and Video Generator (First Gradio Interface) 🎙️📸

In this module, you enter a topic as input and it is transformed into a complete video. Here’s how it works:

- **Script Generation:**  
  Using the latest version of Google Gemini, the system generates detailed scripts for your topic. This ensures that both the visuals and the voiceover are perfectly synchronized in tone and style.

- **Prompt Processing:**  
  Once the script is generated, with the press of a button, it splits into two parts:
  - A **photo script** that outlines a visual narrative.
  - An **audio script** that designs the auditory experience.  
  You can edit them if you don't like some part (each line is a photo and is matched with its corresponding audio line).

- **Integration with Sana and Elevenlabs:**  
  - The **photo script** is sent to **Sana**, the image generation engine that creates the video.
  - The **audio script** is forwarded to **Elevenlabs**, which produces high-quality audio narration.

---

## 2️⃣ Subtitle, Music and Talking Head Generator (Second Gradio Interface) 💬📜

This part of the project is designed to add an extra layer of engagement by combining additional audio, a talking face, and perfectly synchronized subtitles.

- **Subtitle Integration:**  
  - The generated subtitles are carefully timed to match the audio, ensuring that every word appears just when it’s needed.
  - In the Gradio interface you can edit the parameters and positioning of the subtitles.

- **Audio Enrichment with yt-dlp:**  
  - Utilize **yt-dlp** to import additional audio elements or include some songs from the NCS library (attribution required to NCS).
  - It also has a preview audio section where you can test the beginning of the song.

- **Talking Face with SadTalker:**  
  - You can use **SadTalker**, an advanced talking face generator that creates a lifelike avatar capable of mimicking facial expressions and lip-syncing with the provided audio, making the content more interactive and engaging.
  - It also has a preview section where you can test how it would look, generate AI images, or upload your own.

---

## 📜 Licenses and Mentions

This project was made for educational purposes.

**Main Licenses:**

- **Yt-dlp**: Unlicense license [<button>GitHub</button>](https://github.com/yt-dlp/yt-dlp)
- **Wan-ai**: Apache-2.0 license [<button>GitHub</button>](https://github.com/Wan-Video/Wan2.1)
- **Sana**: Apache License 2.0 [<button>GitHub</button>](https://github.com/Wan-Video/Wan2.1)
- **Diffusers**: Apache-2.0 license [<button>GitHub</button>](https://github.com/huggingface/diffusers)
- **Stability_AI (SD_XL)**: MIT license [<button>GitHub</button>](https://github.com/Stability-AI/generative-models)
- **SadTalker**: Apache 2.0 License (except for third-party components) [<button>GitHub</button>](https://github.com/OpenTalker/SadTalker?tab=License-1-ov-file#readme)
- **NCS** [<button>Page</button>](https://ncs.io/ ) . Credits to their respective authors (On and On, Heroes Tonight, Fearless)
- **Google Gemini and ElevenLabs**: Terms and conditions of their respective pages when you get their api keys.
- **Note**: Some of the models in the test area were imported from Hugging Face, check their respective licences.


As for me, nothing more than the license in my project.


