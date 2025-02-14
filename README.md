# Vision Chat Assistant with LLaVA

## 📝 Project Overview
This repository features a Vision Chat Assistant using LLaVA (Large Language and Vision Assistant), enabling image-based conversations with intelligent responses.

## ✨ Features
- **🖼️ Image-Based Conversations:** Conducts dialogues with image context.
- **📸 Image Descriptions:** Generates detailed visual interpretations.
- **📝 Text Extraction (OCR):** Reads text from images.
- **💬 Conversational Memory:** Maintains dialogue context over multiple interactions.
- **⚙️ Efficient Inference:** Supports 8-bit quantization for faster processing.

## ⚙️ Installation

# Clone the repository
git clone https://github.com/yourusername/vision-chat-assistant-with-llava.git
cd vision-chat-assistant-with-llava

# Install dependencies
pip install git+https://github.com/haotian-liu/LLaVA.git@786aa6a19ea10edc6f574ad2e16276974e9aaa3a
pip install torch transformers pillow requests

## 🚀 Usage

# 📤 Start a New Conversation

chatbot = LLaVAChatBot(load_in_8bit=True)
response = chatbot.start_new_chat(
    img_path="https://example.com/image.jpg",
    prompt="Describe the scene in the image."
)
print(response)

# 💬 Continue a Conversation

response = chatbot.continue_chat("What else can you observe?")
print(response)

# 📂 File Structure

- 📜 vision_chat_assistant_with_llava.py: Main script implementing the assistant.

- 📘 README.md: Documentation for setup and usage.

# 📦 Dependencies

- torch

- transformers

- pillow

- requests

- llava

# 💡 Notes

- Utilizes LLaVA for vision-language processing.

- 8-bit quantization is applied for performance efficiency.

- A CUDA-enabled GPU is recommended for optimal speed.
