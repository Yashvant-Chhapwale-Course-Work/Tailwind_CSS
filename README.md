<div align="center">
   <img src="https://github.com/user-attachments/assets/832d3d55-c593-478d-8b81-4e6dabdeb172" alt="Scribe Logo" height="200">
</div>

# Tailwind CSS

This repository simulates a development **roadmap** for creating a "Custom_Tkinter" Application namely, **Scribe_Smart Notes**.

<div align="center">
   
   **📌 For more information on "Scribe_Smart Notes" visit our [Page](https://github.com/Yashvant-Chhapwale/Scribe_Smart-Notes)** <br>
   **📌 Click [`Download`](https://github.com/Yashvant-Chhapwale/Scribe_Smart-Notes/releases) to start using "Scribe_Smart Notes"**
</div>

---

## About Custom-Tkinter
CustomTkinter is a modern **GUI library for Python** that enhances Tkinter with a sleek, customizable look using themes, rounded corners, and improved widgets. It is built on top of Tkinter but offers a more modern design with dark mode support.

### Features:
- `Theming_Support:` Light, Dark, and System themes.
- `Custom_Widgets:` Includes modern buttons, sliders, and checkboxes.
- `Rounded_Corners and Hover_Effects:` Aesthetic improvements over standard Tkinter.
- `Built-in Colors & Styling:` Easily customizable UI elements.
- `Scalability:` Responsive UI that adapts to different screen sizes.
  <br>
  
**📌 Visit the [Documentation](https://customtkinter.tomschimansky.com/) to know more about `Custom_Tkinter`.**

---

<div align="center">
 <h1>Development RoadMap</h1>
</div>

<div align="center">
 
| TITLE                                                                                                          | SECTION_LINK                                                                                  |
|----------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| 1.  **Creating a Python Virtual Environment**                                                                  | >> [` CHECK CONTENT `](#creating-a-python-virtual-environment)                                |
| 2.  **Installing and Importing required Modules for the Application**                                          | >> [` CHECK CONTENT `](#installing-and-importing-required-modules)                            |
| 3.  **Custom-Tkinter Window Themes**                                                                           | >> [` CHECK CONTENT `](#custom_tkinter-window-themes)                                         |
| 4.  **Custom-Tkinter Window Geometry(Width x Height)**                                                         | >> [` CHECK CONTENT `](#adjusting-custom_tkinter_window-dimensions)                           |
| 5.  **Creating Custom-Tkinter Window Instance (CTk( ))**                                                       | >> [` CHECK CONTENT `](#creating-custom_tkinter_window_instance-CTk)                          |
| 6.  **Set Application Logo i.e, Window Icon**                                                                  | >> [` CHECK CONTENT `](#setting-window-icon)                                                  |
| 7.  **Custom-Tkinter Frames and Scrollable-Frames**                                                            | >> [` CHECK CONTENT `](#creating-custom_tkinter-frames-and-scrollable_frames)                 |
| 8.  **Displaying Text and Images using Custom-Tkinter Labels**                                                 | >> [` CHECK CONTENT `](#creating-custom_tkinter-labels-for-displaying-text-and-images)        |
| 9.  **Custom-Tkinter Buttons and Segmented-Buttons**                                                           | >> [` CHECK CONTENT `](#creating-custom_tkinter-buttons-and-segmented_buttons)                |
| 10. **Custom-Tkinter Check_Box and Combo_Box**                                                                 | >> [` CHECK CONTENT `](#creating-custom_tkinter-check_box-and-combo_box)                      |
| 11. **Custom-Tkinter Switch and Slider**                                                                       | >> [` CHECK CONTENT `](#creating-custom_tkinter-switch-and-slider)                            |
| 12. **Custom-Tkinter Entry and Text_Box**                                                                      | >> [` CHECK CONTENT `](#creating-custom_tkinter-entry-and-text_box)                           |
| 13. **Custom-Tkinter Widget Attributes_List**                                                                  | >> [` CHECK CONTENT `](#listing-custom_tkinter-widget-attributes)                             |
| 14. **Manipulating Widget Attributes at Runtime using `.configure()`**                                         | >> [` CHECK CONTENT `](#manipulating-attributes-using-configure--method)                      |
| 15. **Widget Layout Methods (`Pack`, `Place` and `Grid`)**                                                     | >> [` CHECK CONTENT `](#widget-layout-methods-pack-place-and-grid)                            |
| 16. **Creating a Tabbed Interface using Tkinter's Notebook Widget**                                            | >> [` CHECK CONTENT `](#creating-a-tabbed-interface-using-ttknotebook-)                       |
| 17. **Styling Tkinter's Notebook Widget using Style() Function**                                               | >> [` CHECK CONTENT `](#styling-ttknotebook--using-ttkstyle--function)                           |
| 18. **Packaging a Python Script into an EXE using PyInstaller**                                                | >> [` CHECK CONTENT `](#packaging-a-python-script-into-a-standalone-exe-using-pyinstaller)    |
</div>

---

## Creating a Python Virtual Environment
### 1. Ensure Python is Installed:
- **For ` Windows ` Systems:** <br>
     Ensure Python is installed by running the following **prompt**:
     ```
     python --version
     ```
- **For ` Linux / MacOS ` Systems:** <br>
     Ensure Python is installed by running the following **prompt**:
     ```
     python3 --version
     ```
<br>

### 2. Create a Virtual Environment:
- **For ` Windows ` Systems:** <br>
     Create a `Virtual Environment` in Python by running the following **prompt**:
     ```
     python -m venv myenv
     ```
- **For ` Linux / MacOS ` Systems:** <br>
     Create a `Virtual Environment` in Python by running the following **prompt**:
     ```
     python3 -m venv myenv
     ```
<br>

### 3. Activate the Virtual Environment:
- **For ` Windows ` Systems:** <br>
     `Activate` the `Virtual Environment` in Python by running the following **prompt**:
     ```
     # For Command Prompt:
     myenv\Scripts\activate

     # For Powershell:
     myenv\Scripts\Activate.ps1
     ```
- **For ` Linux / MacOS ` Systems:** <br>
     `Activate` the `Virtual Environment` in Python by running the following **prompt**:
     ```
     source myenv/bin/activate
     ```
<br>

### 4. Deactivate the Virtual Environment:
- **For ` Windows ` Systems:** <br>
     After use, `Deactivate` the `Virtual Environment` in Python by running the following **prompt**:
     ```
     deactivate
     ```
- **For ` Linux / MacOS ` Systems:** <br>
     After use, `Deactivate` the `Virtual Environment` in Python by running the following **prompt**:
     ```
     deactivate
     ```
     
---
