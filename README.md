# ScreenPDF (AutoPDF Screen Printer)

Python-based automated utility to take multiple sequential screenshots of a selected screen area and convert them into a single PDF document. This project is a Python recreation of the [plainprinter](https://github.com/plainlab/plainprinter) tool.

## Features

- **Select Printing Area**: Draw a red rectangle over a transparent overlay to select the screen area you want to screenshot.
- **Select Next Button**: Position your mouse over the "Next" page button and press `s` to save the click coordinate.
- **Configurable Click Delay**: Set a delay (in seconds) between capturing a page and clicking the next button to allow contents to load properly.
- **Total Clicks**: Choose how many screenshots you want to take.
- **Auto-Export to PDF**: Compiles all screenshots directly into a single PDF file of your choice.

## Prerequisites

- Python 3.8 or above
- Windows OS (recommended, uses OS-specific keyboard hooks and screen grab functions)

## Installation & Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/irfanrobot/ScreenPDF.git
   cd ScreenPDF
   ```

2. **Create a Virtual Environment**:
   ```bash
   python -m venv venv
   ```

3. **Activate the Virtual Environment**:
   - On Windows CMD:
     ```cmd
     .\venv\Scripts\activate
     ```
   - On Windows PowerShell:
     ```powershell
     .\venv\Scripts\Activate.ps1
     ```

4. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Run the Application**:
   ```bash
   python main.py
   ```
2. Click **Select Printing Area**: Drag your mouse to draw a box around the area you want to scan/screenshot.
3. Click **Select Next Button**: Place your mouse pointer over the "Next" button of the document/webpage you are capturing, and press the `s` key on your keyboard to lock the position.
4. Set the **Click Delay (seconds)** and **Total Clicks**.
5. Click **Start & Save to PDF**:
   - Choose where to save your output PDF file.
   - The application will automatically take screenshots, click the next button, wait, and repeat until done.
   - Once completed, your PDF will be generated at the selected location.

## License

This project is licensed under the MIT License.
