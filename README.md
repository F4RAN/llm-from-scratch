# Building Language Models from Scratch

A hands-on guide for software engineers to understand how language models work by implementing them from first principles.

## 📚 Article Series

1. [Words as Numbers - The Foundation](link-to-medium)
2. [The Sequence Problem - Why Order Matters](link-to-medium)
3. [Attention - The Breakthrough Idea](link-to-medium)
4. [Multiple Perspectives - Multi-Head Attention](link-to-medium)
5. [Transformation - The Feed-Forward Network](link-to-medium)
6. [Stacking Layers - Building Depth](link-to-medium)
7. [Learning - The Training Process](link-to-medium)
8. [Generation - Making it Talk](link-to-medium)
9. [Real Implementation - Mini GPT](link-to-medium)

## 🚀 Quick Start
```bash
# Clone the repository
git clone https://github.com/f4ran/llm-from-scratch.git
cd language-models-from-scratch

# Install dependencies
pip install -r requirements.txt

# Start with article 1
cd 01-words-as-numbers
python word_vectors.py
```

## 📂 Structure

Each folder corresponds to one article and contains:
- `README.md` - Summary and instructions
- Complete, runnable code
- Example data
- Visualizations

## 🎯 Learning Path

**Beginner?** Start from Article 1 and go sequentially.

**Experienced?** Jump to any article - each has its own README with context.

**Want to experiment?** Each folder is standalone - modify and run!

## 💡 Key Concepts

- **No ML background needed** - explained from first principles
- **Runnable code** - every concept has working implementation
- **Visual learning** - plots and diagrams throughout
- **Progressive complexity** - each article builds on the last

## 🛠️ Requirements

- Python 3.8+
- NumPy
- Matplotlib
- (Optional) Jupyter for notebooks

## 📖 About This Series

Written for software engineers who want to truly understand how ChatGPT, Claude, and similar models work under the hood. No hand-waving, no magic - just clear code and explanations.

## 🤝 Contributing

Found a bug? Have a suggestion? PRs welcome!

## 📬 Questions?

Open an issue or reach out on [LinkedIn](https://www.linkedin.com/in/f4ran/)

---
**Start your journey**: [Article 1 - Words as Numbers](link)
---

## **Publishing Strategy**

### **Release Schedule:**
- **Week 1:** Articles 1-2 (Foundation)
- **Week 2:** Article 3 (Attention - the big concept)
- **Week 3:** Articles 4-5 (Multi-head + FFN)
- **Week 4:** Article 6 (Deep models)
- **Week 5:** Article 7 (Training)
- **Week 6:** Articles 8-9 (Generation + Final)

### **Cross-linking:**
Each article should:
1. Link to GitHub folder at the top
2. Reference previous/next articles
3. Have "Read the full series" link
4. Include call-to-action to clone repo

### **Engagement Hooks:**
- **End each article** with a challenge: "Before the next article, try modifying X..."
- **Comments section**: "Share your results when you run the code!"
- **GitHub**: "Star the repo to follow along"

---

## **Bonus Content Ideas**

### **Article 10 (Optional):** "Beyond Basics - What's Different in Real Models?"
- Explain GPT-3/4 scale differences
- Tokenization (BPE vs character)
- Training on GPUs
- Distributed training
- Fine-tuning
