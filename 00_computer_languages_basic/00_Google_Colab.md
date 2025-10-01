## 🚀 What is Google Colab (Colaboratory)?

Google Colab is a free online platform provided by Google where you can write and run Python code in your browser.\
It is especially popular for data science, machine learning, and AI projects.

**🔑 Key Features of Google Colab:**

- No installation needed – runs in your web browser.
- Free access to GPU & TPU – useful for AI/ML training.
- Works with Google Drive – you can save and share notebooks easily.
- Supports Jupyter Notebook style – mix code, text, images, and charts in one file.
- Pre-installed libraries – like NumPy, Pandas, TensorFlow, PyTorch, etc.
- Collaboration – multiple people can work on the same notebook (like Google Docs).
- GitHub - you can connect with your GitHub
 

**🖥️ Example: Running Python in Colab**

When you open a Colab notebook, you can write code like this:

### Simple Python code in Google Colab
```
print("Hello from Google Colab!")
```

**And it will run directly in the browser without installing Python on your computer.**

### 🎯 Why use Colab?

Beginners: Learn Python without installing anything.

Students: Do assignments easily.

## 🌐 Languages You Can Work With in Google Colab

By default, Colab is made for Python 🐍 (and that’s what most people use).
But you can also run other languages with some setup:

**1. Directly Supported**

Python (default) → Built-in, no setup required.

**2. With Extra Setup**

Using special packages (like %%bash, %%script, or installing interpreters), you can also run:
- R (with R magic or by installing R kernel)
- Julia (by installing Julia kernel)
- JavaScript (Node.js)
- C / C++ (using g++ compiler inside Colab)
- Bash / Shell scripting (using %%bash)

**3. Other Possibilities**

Since Colab is basically a Linux environment in the cloud, you can install interpreters for many languages (Ruby, Go, Scala, etc.), but it requires manual setup.

**✅ Quick Example in Colab**
### Python (default)
```
print("Hello, Python!")
```

### Bash
```
%%bash
echo "Hello from Bash!"
```

### C++
```
%%writefile hello.cpp
#include <iostream>
using namespace std;
int main() {
    cout << "Hello from C++!";
    return 0;
}
```
```
!g++ hello.cpp -o hello
!./hello
```

**🎯 Summary**

Default language: Python

Easily possible: R, Julia, Bash, C, C++

With extra setup: Many others (Java, Ruby, Go, etc.)

Data Scientists: Train ML models with free GPU power.

Professionals: Share reproducible code with teams.


## Little bit more about CPU, GPU, TPU

### CPU
**🖥️ CPU = Central Processing Unit**
- Often called the “brain of the computer” 🧠.
- It carries out all the instructions given by programs.
- Without a CPU, a computer cannot run.

**🔑 Key Functions of CPU**

1. Fetch – takes instructions from memory.

2. Decode – understands what the instruction means.

3. Execute – acts (calculation, move data, etc.).

4. Store – saves the result back into memory.

**🏗️ Main Parts of CPU**

- ALU (Arithmetic Logic Unit) – does calculations and logic. ➕ ➖ ✖️

- CU (Control Unit) – controls how data moves between memory, CPU, and devices.

- Registers – very small, fast storage inside the CPU.

**🖥️ Examples of CPU in Daily Life**

- Opening Microsoft Word → CPU processes it.

- Watching a video → CPU decodes video data.

- Playing a game → CPU handles logic, while GPU handles graphics.
### GPU
**🎮 GPU = Graphics Processing Unit**

- A GPU is a special computer chip originally designed for graphics and gaming.

- But today, GPUs are also heavily used for machine learning (ML) and deep learning (DL) because they can process thousands of small tasks in parallel.

**🔑 Key Points about GPU**

1. Parallel Processing – Can do many calculations at once.

2. Faster than CPU for tasks like image processing, video rendering, and ML.

3. Used in AI training, gaming, 3D rendering, and cryptocurrency mining.

### TPU
**⚡ TPU = Tensor Processing Unit**

- A TPU is a special computer chip made by Google.

- It is designed specifically for machine learning (ML) and deep learning (DL) tasks.

- Faster than CPU (Central Processing Unit) and often faster than GPU (Graphics Processing Unit) for AI work.

**🔑 Why TPU is Special?**

1. Made for TensorFlow (Google’s ML framework).

2. Handles matrix calculations (which are very common in AI) super fast.

3. Used in Google Colab, so you can train AI models faster for free.

**✅ In short:**\
**TPU = Google’s AI chip to speed up deep learning models.**

**🎯 Example in Google Colab**

**When you go to Runtime → Change runtime type → Hardware accelerator, you can choose:**

**CPU**

**GPU**

**TPU**

**👉 If you select CPU, Colab will give you Google’s Central Processing Unit for your code.
👉 If you select GPU, Colab will give you Google’s Graphics Processing Unit for your code.
👉 If you select TPU, Colab will give you Google’s Tensor Processing Unit for your code.**

**🎯 Easy Way to Remember**

**CPU = Brain of the computer (all-purpose, step by step).**
**GPU = Muscle for graphics & parallel work.**
**TPU = Google’s special AI chip (super-fast for ML).**


| Feature            | **CPU** 🧠                         | **GPU** 🎮                    | **TPU** 🤖                             |
| ------------------ | ---------------------------------- | ----------------------------- | -------------------------------------- |
| Full Form          | Central Processing Unit            | Graphics Processing Unit      | Tensor Processing Unit                 |
| Made For           | General tasks (all-rounder)        | Graphics, parallel tasks      | Machine Learning & AI                  |
| Cores              | Few (2–16) powerful cores          | Thousands of smaller cores    | Special AI cores                       |
| Speed              | Best for single tasks              | Best for parallel tasks       | Best for AI training                   |
| Examples of Use    | Running Windows, MS Word, Browsers | Gaming, Video Editing, AI     | Deep Learning (TensorFlow, Colab)      |
| Cost               | Already inside computer            | Extra hardware (graphic card) | Available mostly on Google Cloud/Colab |
| Daily Life Example | Writing a document ✍️              | Playing PUBG 🎮               | Training ChatGPT-like AI 🤖            |





