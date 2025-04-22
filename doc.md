# Search Narwhal Documentation

## Overview
Search Narwhal is a free, open-source browser engine developed by Zohan Haque. It is designed to build custom browsers using Python's Tkinter GUI toolkit. This engine is highly modular and allows developers to create browsers tailored to their specific needs. 

The project is available for download from the GitHub repository at: [ZohanHaqu/searchnarwhal](https://github.com/ZohanHaqu/searchnarwhal). 

### Features
- **Open-source**: Fully free and customizable.
- **Python-based**: Utilizes Python's Tkinter for the GUI and is extendable with Python scripts.
- **Customizable Browsers**: Allows developers to create fully customized browsers by modifying the SDK and example code.
- **SDK and Example Code**: Comes with a Software Development Kit (SDK) and an example browser implementation (`example_browser.py`) to help developers get started.
- **Compiling with PyInstaller**: Easy distribution by compiling the browser with PyInstaller.
- **NSIS Support**: Distribute custom browsers via NSIS (Nullsoft Scriptable Install System) installers.

## Installation

### Prerequisites
Before you start using Search Narwhal, make sure you have the following installed on your machine:
- Python 3.x (preferably the latest version)
- Tkinter (usually included with Python)
- PyInstaller (for compiling the browser into an executable)
- NSIS (for creating installers)

### Setup Guide
1. **Clone the Repository**
   - Clone the Search Narwhal repository to your local machine using the following command:
     ```bash
     git clone https://github.com/ZohanHaqu/searchnarwhal.git
     ```

2. **Install Dependencies**
   - Install the required dependencies using `pip`:
     ```bash
     pip install -r requirements.txt
     ```

3. **Run Example Browser**
   - Navigate to the `example_browser.py` file in the project directory and run it to test the basic functionality of Search Narwhal:
     ```bash
     python example_browser.py
     ```

4. **Compile the Browser with PyInstaller**
   - After customizing your browser, you can compile it into an executable using PyInstaller:
     ```bash
     pyinstaller --onefile example_browser.py
     ```

5. **Creating Installers with NSIS**
   - To distribute your custom browser, you can create an installer using NSIS:
     - Download and install NSIS from [NSIS website](https://nsis.sourceforge.io/Download).
     - Create a `.nsi` script for your browser distribution (see `example_browser.nsi` for an example).

## SDK and Customization

Search Narwhal provides a flexible SDK for building your own browsers. Below are some key components you can customize:

### `example_browser.py`
This file contains the basic implementation of a browser using the Search Narwhal engine. You can modify the following:
- **UI Elements**: Change the layout or add new elements to the interface.
- **Functionality**: Add custom features like bookmarks, settings, etc.
- **Rendering**: Modify how web pages are rendered in the browser.

### `searchnarwhal.py`
The core file that contains the engine's main logic. This file controls:
- **Navigation**: How the browser loads and navigates between web pages.
- **Search Engine**: Set a custom search engine.
- **Request Handling**: Modify how HTTP requests are managed.

### `assets/`
A folder that contains all the resources for the browser, such as:
- Icons
- UI Layouts (using Tkinter)
- Styling (CSS and other media files)

## Building a Custom Browser

To build your custom browser with Search Narwhal:
1. Copy the `example_browser.py` file and rename it to something like `my_browser.py`.
2. Modify the script to adjust the interface and functionality to your needs.
3. If needed, add new Python libraries or dependencies.
4. Run and test your custom browser.
5. Use PyInstaller to compile the browser into an executable.
6. Create an installer with NSIS for distribution.

## FAQ

### How can I contribute to the project?
Contributions to the project are always welcome! You can fork the repository, make your changes, and submit a pull request. Please make sure to write tests for any new features or fixes you add.

### Can I use Search Narwhal for commercial purposes?
Yes, Search Narwhal is released under an open-source license, and you are free to use it for both personal and commercial projects. However, you should review the licensing terms in the repository for any restrictions.

### Are there any performance optimizations I can make?
Yes, the default example browser is a simple proof-of-concept. You can optimize performance by:
- Modifying the rendering engine.
- Using more efficient libraries for specific tasks.
- Reducing memory usage by optimizing the Python code.

## License
Search Narwhal is released under the MIT License. See the `LICENSE` file for more details.

## Contact
For support, issues, or feedback, open an issue in the GitHub repository or contact the maintainers via GitHub.

