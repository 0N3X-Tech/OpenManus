![banner](https://github.com/user-attachments/assets/9ebbbfa2-3ee8-4e87-a32e-ae441bf339ac)

# 👋 Welcome to ozManus

ozManus is a community-driven fork of OpenManus — an intelligent autonomous agent framework originally created by the MetaGPT team.
While OpenManus opened the gates to agentic creativity, ozManus removes all barriers to entry and supercharges the vision.

Whether you're exploring LLMs, building multi-agent workflows, or just curious about AI automation — ozManus is your sandbox.

## ✨ Why ozManus?

* 🚪 No Invite Code Required – ozManus is open to everyone.
* 🔄 Forked & Upgraded – Based on OpenManus, now with improvements for accessibility, developer experience, and experimentation.
* 🧠 LLM Agent Framework – Build and run ideas through powerful language models.
* 🌏 Born in Australia – Forked with love and built for openness, transparency, and limitless potential.

## 🚀 Getting Started

To start using ozManus, complete the following steps.

### 🛠 Prerequisites

* Python 3.12
* uv or conda
* An OpenAI API Key (or other LLM provider)

### ⚙️ Installation

Use one of the following methods to install ozManus.

1. ✅ **Method 1**: Using Conda

```bash
conda create -n oz_manus python=3.12
conda activate oz_manus
git clone https://github.com/YOUR-USERNAME/ozManus.git
cd ozManus
pip install -r requirements.txt
```

2. 🚀 **Method 2**: Using uv (Recommended)

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
git clone https://github.com/YOUR-USERNAME/ozManus.git
cd ozManus
uv venv --python 3.12
source .venv/bin/activate   # For Unix/macOS
# .venv\Scripts\activate    # For Windows
uv pip install -r requirements.txt
```

3. 🔍 (**Optional**) Install browser automation tools

```bash
playwright install
```

### 🧩 Configuration

ozManus requires the following configurations to connect to LLM providers such as OpenAI.

1. Copy the example config file.

```bash
cp config/config.example.toml config/config.toml
```

2. Edit your API keys and model preferences.

```toml
[llm]
model = "gpt-4o"
base_url = "https://api.openai.com/v1"
api_key = "sk-..."  # Your API key here
max_tokens = 4096
temperature = 0.0

[llm.vision]
model = "gpt-4o"
base_url = "https://api.openai.com/v1"
api_key = "sk-..."
```

You can customize your models, temperature, and other parameters as needed.

## ⚡Usage

Once set up, use any of the following ways to launch ozManus according to your use case.

### ✨ Quick Start
Run your own autonomous LLM agent:

```bash
python main.py
```

### 🧠 Run Multi-Agent MCP Tool

```bash
python run_mcp.py
```

### 🧪 Experimental Multi-Agent Flow (Unstable)

```bash
python run_flow.py
```

## 🧠 About ozManus

ozManus builds upon OpenManus by @Xinbin Liang and @Jinyu Xiang, with contributions from @Zhaoyang Yu, @Jiayi Zhang, and @Sirui Hong — all part of the MetaGPT team.

The goal of ozManus is to provide:

* A fully open-source LLM agent platform
* Easier developer onboarding
* Community-driven features and experiments
* A home for experimentation in reinforcement learning tuning for LLMs

We also support ozManus-RL, an advanced research project exploring RL fine-tuning (e.g., GRPO) for agent behaviors.
This work is inspired by collaborations between researchers from UIUC and OpenManus.

## 🤝 Contributing

We welcome your ideas, questions, and pull requests!
Here’s how to get involved:

### 🧰 Pre-commit Hook

Please run the following before submitting a PR:

```bash
pre-commit run --all-files
```

### 📮 Contact

Have questions or proposals?
Email us directly at `mannaandpoem@gmail.com`

### 🌐 Community

Join the ozManus community on Discord or Feishu to:

* 💬 Ask questions
* 🧠 Share ideas
* ⚒️ Collaborate on new features
* 🧪 Explore ozManus-RL

## 📜 License

ozManus is licensed under the MIT License.
