![GitHub](https://img.shields.io/badge/GitHub-Profile-black): [mk197d](https://github.com/mk197d)

# TexEtch

TexEtch is a Visual Studio Code extension designed to convert diagrams drawn in [draw.io](https://app.diagrams.net/) into text format. This text format can be easily integrated into your code base to provide better explanations and documentation for your code.

## Features

- **Diagram to Text Conversion**: Convert complex diagrams from draw.io into readable text format.
- **Seamless Integration**: Easily integrate the converted text into your codebase to enhance documentation. Option to put the produced output at the top of the code block or alongside the code block.
- **Support for Multiple Diagram Types**: Handles a variety of diagram types and structures.

## Installation

The extension can be installed from Visual Studio Code Marketplace.

## Usage
1. Open the draw.io website or application and create a file containing your desired diagram.
2. Navigate to File -> Export as -> XML and download the file.
![Step 1](https://github.com/mk197d/TexEtch/blob/main/Step1.png)
3. In Visual Studio Code, open the command palette by pressing Ctrl+Shift+P (Windows/Linux) or Cmd+Shift+P (macOS).
4. Type TexEtch and select the corresponding command.
5. An Open Dialog box will appear, prompting you to select the required .xml file.
6. After selecting the file, a text input box will appear to take in the comment characters used for the language in use or any string of your choice. Leave empty for no extra characters.
![Walkthrough 1](https://github.com/mk197d/TexEtch/blob/main/walkthrough1.mp4)
    - To put the generated text at top of a code snippet -> put the cursor on the line just above the block.
    <div style="display: flex; align-items: center;">
      <img src="https://github.com/mk197d/TexEtch/blob/main/above_b.png" alt="Above_b" width="100%">
      <img src="https://github.com/mk197d/TexEtch/blob/main/above_a.png" alt="Above_a" width="100%">
    </div>
    - To put the generated text alongside the code -> select the code block.
    <div style="display: flex; align-items: center;">
      <img src="https://github.com/mk197d/TexEtch/blob/main/along_b.png" alt="Along_a" width="100%">
      <img src="https://github.com/mk197d/TexEtch/blob/main/along_a.png" alt="Along_b" width="100%">
    </div>


## Supported Figures

- **Horizontal and Vertical lines**: Line, Dashed Line, Dotted Line, Directional and Bidirectional Connector and Arrow.
![Lines](https://github.com/mk197d/TexEtch/blob/main/Lines2.png)

- **Circle and Ellipse**
<div style="display: flex; align-items: center;">
  <img src="https://github.com/mk197d/TexEtch/blob/main/Circle.png" alt="Circle" width="25%">
  <img src="https://github.com/mk197d/TexEtch/blob/main/Ellipse.png" alt="Ellipse" width="50%">
</div>

- **Text**
    - Use text size as **11** in the draw.io editor to match the exact ratio of figures and text in the final output.
    - Avoid copying text from sources with colorful text to prevent disperancies in the output.
    - Leave enough space on the boundaries of text box, so that text can appear in same format.

- **Rectangle** 

**Caution**
Please don't use arrows which originate directly from figures like shown below:<br>
![notArrow](https://github.com/mk197d/TexEtch/blob/main/notArrow.png)

**Support for slanted lines, curves and other figures coming soon in future versions**

## Examples

- Drawing stacks in architecture code.<br>
  **BEFORE**<br>
  ![ex2b](https://github.com/mk197d/TexEtch/blob/main/ex2b.png) 
  **AFTER**<br>
  ![ex2a](https://github.com/mk197d/TexEtch/blob/main/ex2a.png) 

- Initializing classes with many fields.<br>
  **BEFORE**<br>
  ![ex3b](https://github.com/mk197d/TexEtch/blob/main/ex3b.png) 
  **AFTER**<br>
  ![ex3a](https://github.com/mk197d/TexEtch/blob/main/ex3a.png)

- Algorithm on arrays<br>
  ![ex1](https://github.com/mk197d/TexEtch/blob/main/ex1.png)

- Just for fun..<br>
  ![ex5](https://github.com/mk197d/TexEtch/blob/main/ex5.png)
