# InfoNest


**InfoNest** allows you to interact with your documents locally, ensuring complete privacy. It supports various open-source models and embeddings, providing a versatile and secure solution for document-based conversations.

## 🚀 Features
- Utmost privacy with complete local data processing.
- Versatile model support (HF, GPTQ, GGML, GGUF).
- Diverse embeddings.
- Chat history in a session.
- API for building RAG applications.
- Graphical interface options.
- Multi-platform support (GPU, CPU, MPS).


<details>
<summary>📐 Setup Instuctions:</summary>

### 1. Clone the Repository
```sh
git clone https://github.com/PromtEngineer/InfoNest.git
cd InfoNest
```

### 2. Create and Activate a Conda Environment

```sh
conda create -n InfoNest python=3.10.0
conda activate InfoNest
```
### 3. Install Dependencies

```sh
pip install -r requirements.txt
```

### 4. Install LlamaCpp-Python for Model Support
 
```sh
CMAKE_ARGS="-DLLAMA_CUBLAS=on" FORCE_CMAKE=1 pip install llama-cpp-python --no-cache-dir
```

</details>


<details>
<summary> 🧑‍💻 Usage: </summary>


### 🗣️ Ask questions to your documents using Terminal

Run the following command:
```sh
python run_InfoNest.py --device_type [cpu|mps|cuda]
```
Type your queries when prompted. 

### 💡 NOTE:

Modify ```constant.py``` to set your desired model

### ✅ Use the Graphical User Interface

Start the API server by running the following command:
```sh
python run_InfoNest_API.py
```

In another terminal, run the GUI:
```sh
cd InfoNestUI
python InfoNestUI.py
```

</details>

<details>
<summary> 📚 References: </summary>

### Fix Cuda Extensions Issue:
First, I uninstalled

```pip uninstall auto-gptq```

Then, simply reinstall it from source

```pip install "git+https://github.com/PanQiWei/AutoGPTQ.git@v0.4.2" ```

</details>
