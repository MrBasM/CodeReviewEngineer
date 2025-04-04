# CodeReviewEngineer - 🧠 Java Code Review AI 
(powered by Gemma 3)

An automated code review assistant for Java projects, powered by large language models (LLMs) like Google's Gemma 3.

This tool helps developers review `.java` files by analyzing code quality, readability, best practices, and potential bugs — and returns structured feedback in Markdown format.

---

## 🚀 Features

- 📄 Upload individual Java files, full directories, or recursive folders
- 💬 Prompt-driven AI review using a flexible LLM backend
- 🧠 Built-in support for [Gemma 3](https://huggingface.co/google/gemma-1.5-4b-it)
- 📂 Generates one markdown file per Java class
- 📊 Central summary report with class names, line numbers, and suggestions
- 💡 Future-proof architecture (easily switch between Gemma, LLaMA, Mistral, etc.)

---

## 📥 Input

- Plain `.java` files
- Optional: Future versions will support Git diffs and PR reviews

---

## 📤 Output

- `reviews/ClassName.java.md` → Individual review file  
- `reviews/README.md` → Summary table of all findings

Example output snippet:

```markdown
| Class            | Line | Issue                                 |
|------------------|------|----------------------------------------|
| AccountManager   | 24   | Magic number detected (`1234`)         |
| OrderService     | 45   | Missing null check for orderId         |
