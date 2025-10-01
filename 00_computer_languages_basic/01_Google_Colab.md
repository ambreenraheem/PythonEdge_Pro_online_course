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
