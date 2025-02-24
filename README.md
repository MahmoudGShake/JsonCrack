# JsonCrack 📊

**JsonCrack** is a Python package that **visualizes JSON as a vertical graph** to help developers understand complex JSON structures easily.

---

## 🚀 Features
💚 **Convert JavaScript-style JSON** (`null`, `true`, `false`) → Python (`None`, `True`, `False`)  
💚 **Generate vertical graph visualization** of JSON data  
💚 **Automatically detects OS** to display the graph (`Windows`, `Mac`, `Linux`)  
💚 **No need for a web interface**—runs locally  

---

## 📚 Installation

1. **Install Graphviz** (required for rendering graphs):
   - **Windows**: Download and install from [Graphviz website](https://graphviz.gitlab.io/download/)
   - **Mac**:  
     ```sh
     brew install graphviz
     ```
   - **Linux** (Debian/Ubuntu):
     ```sh
     sudo apt install graphviz
     ```

2. **Install JsonCrack**:
   ```sh
   pip install JsonCrack
   ```

---

## 🔥 Quick Start

### **1⃣ Convert JavaScript-style JSON to Python**
```python
from JsonCrack.Cracker import JSON

js_data = '''
{
    "name": "Alice",
    "active": true,
    "address": null
}
'''

# Convert JS JSON to Python format
json_obj = JSON(js_data)
python_json = json_obj.convert_js_to_python()
print(python_json)
```
**🟢 Output:**
```python
{'name': 'Alice', 'active': True, 'address': None}
```

---

### **2⃣ Visualize JSON Data**
```python
json_obj.visualize(display=True)
```
📌 **This will open a PNG file displaying the JSON structure as a vertical graph.**  

---

### **3⃣ Convert & Visualize in One Step**
```python
json_obj = JSON(js_data)
json_obj.convert_js_to_python()
json_obj.visualize(display=True)
```

---

## 🛠 Development

1. **Clone the repository**:
   ```sh
   git clone https://github.com/yourusername/JsonCrack.git
   cd JsonCrack
   ```
2. **Install dependencies**:
   ```sh
   pip install -r requirements.txt
   ```
3. **Install package in editable mode**:
   ```sh
   pip install -e .
   ```

---

## 👥 Contributing

We welcome contributions! 🎉

1. Fork the repository  
2. Create a new branch (`git checkout -b feature-branch`)  
3. Make your changes  
4. Commit and push (`git commit -m "Added new feature" && git push origin feature-branch`)  
5. Create a pull request  

---

## 🐝 License

**MIT License** - Free to use and modify. See [LICENSE](LICENSE) for details.

---

## 💡 Future Improvements
🚧 **Planned features**:
- [ ] **Interactive web-based visualization**  
- [ ] **More export formats (SVG, PDF, JSON Tree)**  
- [ ] **Better error handling for invalid JSON**  

---

## 🌟 Show Your Support

🌟 **Star this repository** on [GitHub](https://github.com/yourusername/JsonCrack) if you find it useful!  
💬 Feel free to open issues for **bug reports & feature requests**.  

---

**Happy Coding! 🚀**

