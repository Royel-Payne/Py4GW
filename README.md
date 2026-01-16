# Py4GW

**Py4GW** is a Python library designed to enhance the Guild Wars experience by providing tools for automation, scripting, and in-game interactions.
---

## Features

- **Agent Handling**: Manage agents (NPCs, enemies, allies) with ease.
- **Inventory Management**: Automate inventory-related tasks such as item handling and categorization.
- **Pathfinding and Navigation**: Built-in tools for pathfinding and movement.
- **Widgets**: Extensible widgets for customizing user experiences, including travel, titles, and more.
- **Event Hooks**: Hook into game events and create your own custom logic.
- **Multi-Account Support**: Efficiently manage multiple accounts simultaneously.
- **Lightweight and Modular**: Designed to be fast, modular, and easy to extend.

---

## 🚀 Getting Started

### **Prerequisites**

- Python 3.13.0 32-bit [link](https://www.python.org/downloads/release/python-3130/) (other versions could causes GW Client crashes)
- Guild Wars client

### **Installation**

1. Clone the repository:
   ```bash
   git clone https://github.com/apoguita/Py4GW.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Py4GW
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## 📂 Directory Structure

```
Py4GW/
├── Addons/                     # Add-on extensions (e.g., GWBlackBOX.dll)
├── Bots/                       # Automation bot scripts
├── DEMO/                       # Demo scripts demonstrating library usage
├── Examples/                   # Example scripts and templates for learning
├── HeroAI/                     # Hero AI automation and logic
├── Py4GWCoreLib/               # Core library for Guild Wars automation
├── Widgets/                    # Widgets for in-game interactions
│   ├── Config/                 # Widget configuration files
│   ├── Data/                   # Widget data files
│   └── *.py                    # Individual widget scripts
├── docs/                       # Documentation files
├── fonts/                      # Font resources
├── stubs/                      # Type hint files for Python development
├── Styles/                     # UI style configurations
├── templates/                  # Template configurations
├── Textures/                   # Image and texture resources
├── Legacy code and tests/      # Archived code and test scripts
├── Py4GW.dll                   # Main DLL for the project
├── Py4GW.ini                   # Configuration file
├── Py4GW_widget_manager.py     # Widget manager script
├── Py4GW_LauncherCompact.py    # Compact launcher script
└── requirements.txt            # Python dependencies
```

---

## 📥 How to Download

1. Go to the [Releases Page](https://github.com/apoguita/Py4GW/releases/tag/Official).
2. Download the files under "Assets."
3. Extract them to your preferred directory.

---

## 🤝 Contributing

We welcome contributions from the community! Here’s how you can get involved:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes and push the branch.
4. Submit a pull request for review.

### Stop tracking log/configuration files

If you want want to stop tracking local changes to the log and configuration files used by Py4GW you can use the following commands to temporarly remove them from the worktree.

```bash
git update-index --skip-worktree Py4GW_injection_log.txt
git update-index --skip-worktree Py4GW.ini
git update-index --skip-worktree Py4GW_Launcher.ini
```

You can then verify that the files are correctly skipped by running this command that should output the list of skipped files: 

```bash
git ls-files -v | grep "^S"
S Py4GW.ini
S Py4GW_Launcher.ini
S Py4GW_injection_log.txt
```

To re-enable local tracking of the files run the following commands: 

```bash
git update-index --no-skip-worktree Py4GW_injection_log.txt
git update-index --no-skip-worktree Py4GW.ini
git update-index --no-skip-worktree Py4GW_Launcher.ini
```