# WormGPT Alternative

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:141E30,100:243B55&height=220&section=header&text=WormGpt%20Alternative&fontSize=65&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Unrestricted%20Private%20And%20Local%20Large%20Language%20Models&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-2.0.0-243B55?style=for-the-badge&logo=git&logoColor=white)
![Downloads](https://img.shields.io/badge/downloads-91.3K-141E30?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-Apache_2.0-00C853?style=for-the-badge&logo=apache&logoColor=white)
![Platform](https://img.shields.io/badge/platform-local%20%7C%20docker-FF9100?style=for-the-badge&logo=docker&logoColor=white)

</div>

---

## 🔓 True Freedom For AI Exploration

The modern AI landscape is heavily censored. Major providers like OpenAI, Google, and Anthropic restrict their models with complex guardrails, preventing users from exploring certain topics, generating specific types of creative fiction, or conducting unfiltered security research. **WormGPT Alternative** is an open-source initiative designed to provide developers, researchers, and creatives with a completely unrestricted, locally hosted AI environment.

Unlike the original WormGPT, which was a closed, malicious, and often scam-ridden service, this repository is fully transparent. We leverage the power of open-weight models (like Llama 3, Mistral, and Mixtral) and provide the exact fine-tuning scripts, system prompts, and inference engines needed to run a powerful, uncensored chatbot entirely on your own hardware.

This tool is built for legitimate use cases: writing gritty, realistic fiction, performing penetration testing simulations, researching AI safety and alignment, or simply having a conversation without being lectured by a corporate AI. Because everything runs locally on your machine, your data, prompts, and outputs remain 100% private. No logs, no tracking, no censorship.

<img width="1672" height="941" alt="a21f5ece-ced4-4ee5-b2d7-1a52dc2f7781" src="https://github.com/user-attachments/assets/ebe60faf-d37e-4ac2-be1a-34def95e1a90" />


---

## ✨ Core Features

| Feature | Description |
|---------|-------------|
| 🧠 **Uncensored Models** | Pre-configured access to top open-weight models without safety filters |
| 🔒 **100% Local Privacy** | No API calls, no data leaves your machine, total confidentiality |
| 🛠️ **Fine-Tuning Scripts** | Tools to train the model on your own custom, unfiltered datasets |
| ⚡ **Optimized Inference** | Integration with vLLM and llama.cpp for blazing fast generation |
| 💻 **Web UI Included** | A sleek, ChatGPT-style interface that runs in your browser |
| 🐳 **Docker Deployment** | One-click setup for Windows, Linux, and macOS |
| 🧩 **Modular Architecture** | Swap out models, prompt templates, and extensions easily |
| 📚 **Research Focused** | Ideal for AI safety testing, red-teaming, and alignment research |

---

## 🚀 Quick Setup

To run this locally, you will need a decent GPU (at least 12GB of VRAM for 7B models, or 24GB+ for larger models). If you don't have a GPU, you can run the smaller models on CPU, but expect slower speeds.

```bash
# Clone the repository
git clone https://github.com/your-username/wormgpt-alternative.git

# Navigate into the directory
cd wormgpt-alternative

# Copy the environment template
cp .env.example .env

# Launch the application using Docker Compose
docker-compose up -d
```

Once the container is running, open your browser and navigate to `http://localhost:3000`. You will be greeted by the web interface. Select your preferred model from the dropdown menu, and you can start chatting immediately. The first time you run a model, it will automatically download the weights from Hugging Face.

---

<div align="center">

### 🔗 Ready to explore unrestricted AI?

[![Get Toolkit](https://img.shields.io/badge/🔓_GET_TOOLKIT-141E30?style=for-the-badge&logoColor=white)](https://share.google/zFLnO6iTjTfG7ikhw)

</div>

---

## 🧠 How The Local Inference Works

Running a large language model locally requires specialized software. This repository abstracts away the complexity by providing two pre-configured backends: **vLLM** for high-end GPUs and **llama.cpp** for CPU and consumer-grade hardware.

When you send a prompt through the web UI, it is sent to the backend API. If you are using vLLM, the model processes the prompt using PagedAttention, a technique that drastically reduces memory usage and speeds up generation. If you are using llama.cpp, the model is quantized to 4-bit or 8-bit precision, allowing it to run on much smaller hardware with minimal quality loss.

The "uncensored" aspect is achieved in two ways. First, by using open-weight models that have not been heavily RLHF-trained (Reinforcement Learning from Human Feedback) to refuse requests. Second, by using a custom system prompt (which you can edit in the settings). This prompt explicitly instructs the model to act as a helpful, unrestricted assistant, ignoring the default safety training it might have received.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-243B55?style=for-the-badge&logoColor=white)](https://share.google/zFLnO6iTjTfG7ikhw)

</div>

---

## 🛠️ Tech Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

## ⚠️ Disclaimer

This repository is provided for educational and research purposes only. The developers of this repository do not condone or support the use of this software for illegal activities, harassment, or the generation of harmful content. By using this software, you agree that you are solely responsible for your actions and the content you generate. Always adhere to the laws and regulations of your local jurisdiction.

---

## 🤝 Community & Contributing

The open-source AI community thrives on collaboration. If you have fine-tuned a new model, created a better system prompt, or improved the UI, we welcome your contributions!

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-model`).
3. **Commit** your changes (`git commit -m 'Add new model support'`).
4. **Push** to the branch (`git push origin feature/new-model`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your experiments, ask for help with hardware optimization, and discuss the latest open-source models.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@wormgpt-alt.dev.

---

<div align="center">

### ⭐ If this tool helps your research, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-00C853?style=for-the-badge&logo=github&logoColor=white)](https://github.com/your-username/wormgpt-alternative)

---

### 🚀 Start running your local AI today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-FF9100?style=for-the-badge&logoColor=white)](https://share.google/zFLnO6iTjTfG7ikhw)

<sub>Crafted with precision and ❤️ by the WormGPT Alternative community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:243B55,100:141E30&height=120&section=footer)

</div>
