<p align="center">
  <img src="docs/screenshots/cn8n-flow.jpg" alt="n8n-flow cover" width="100%">
</p>

# 🎞️ AI-Powered Slideshow Video Creator (n8n Workflow)

This n8n workflow automatically creates slideshow-style videos from structured text data using AI-generated images and external video rendering tools.

## 🔧 Use Case

Turn text prompts (e.g., quotes, product info, story scenes) into visual content for:

- 🎥 TikTok / Reels / YouTube Shorts
- 🛍️ Product showcases
- 📚 Storytelling or educational content
- 📈 Video ads & social automation

## 🧠 How It Works

1. **Input Text**  
   Source data comes from Google Sheets or webhook input (e.g., prompt per slide).

2. **Image Generation**  
   Each prompt is passed to an AI image generator (e.g., Stable Diffusion, DALL·E, etc.) using an API.

3. **Slide Preparation**  
   Image + optional text overlay is saved for each slide.

4. **Video Assembly**  
   Collected assets are sent to FFMPEG or a webhook-based rendering service (like [RunPod](https://www.runpod.io/) or custom server).

5. **Final Output**  
   A complete slideshow video is created and can be uploaded to social platforms.

## 🛠 Tech Stack

- [n8n](https://n8n.io/)
- AI Image Generator API (e.g., Stable Diffusion / HuggingFace / DALL·E)
- Google Sheets (optional)
- FFMPEG / external rendering (e.g., webhook)
- Telegram / Email (optional delivery)

## 📁 Example Flow Nodes

- Google Sheets (or Webhook)
- HTTP Request (Image Generator)
- Set (format file names and slides)
- External webhook for rendering
- Telegram / Email for delivery

## 💡 Notes

- You can adjust image prompt styles, add branding, or insert subtitles.
- For more creative control, integrate templates (e.g., Canva, CapCut via APIs).
- Rendering can also be offloaded to services like RunPod or Replicate.

---

## 🚀 Output Example

Prompt 1: "A peaceful sunrise over a mountain lake" → slide 1
Prompt 2: "A child reading a book under a tree" → slide 2
...
→ Slideshow.mp4 (9:16 vertical, with transitions and soundtrack)



## 📬 Contact

Created by [Serhii Litus](https://www.upwork.com/freelancers/~016b54c2291f96bd7d)  
Let's build smart automations that work while you sleep ☕ 
