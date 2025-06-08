<div align="center">
   <img src="https://github.com/user-attachments/assets/5f875ede-34c9-424f-90a7-c860996c51fb" alt="Tailwind Logo" width="60%" height="20%">
</div>

# Tailwind CSS

This **Repository** documents my my `Notes`, `Learnings`, and `UI_Project` as I progress through a `Tailwind_CSS Bootcamp` to Master **Modern UI development**.<br>

<div align="center">
   
   **📌 Checkout my Post-Bootcamp [`Tailwind_UI Project`](https://github.com/Yashvant-Chhapwale/Scribe_Smart-Notes)** <br>
</div>

---

## About Tailwind_CSS
`Tailwind CSS` is a **`Utility-First CSS Framework`** for rapidly building **Modern** and **Responsive** User_Interfaces.<br>
- `Utility:` A **Utility** is a **Single-Purpose CSS_Class** that applies **Styling** for one specific **Style_Attribute**.
- `Utility-First:` **Tailwind** encourages you to use **Utility_Classes** which are your **First and Main Styling_Method** before using External_CSS or Plugins.
- `CSS_Framework`: **Tailwind** is a **CSS_Framework** that provides a **predefined set of Styles, Utility_Classes, and Conventions** that help you build UIs quickly.

### Features:
- `Utility-First Approach:` The **Utility_Classes** are your First and Main Styling_Method.
- `Responsive Design:` Easily build **UI_layouts that Adapt to different Screen_Sizes** with Mobile-First breakpoints.
- `Component-Friendly:`  Encourages **Reusable UI_Components** without the need to leave HTML.
- `JIT(Just-In-Time) Engine:`  **Utilizes Just-In-Time Compilation** for fast build times and smaller final CSS output. It generates the CSS you need, only when you need it, instead of generating everything up front.
<br>
  
**📌 Visit the [Official_Documentation](https://tailwindcss.com/docs) to know more about `Tailwind_CSS`.**

---

<div align="center">
 <h1>Index</h1>
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
