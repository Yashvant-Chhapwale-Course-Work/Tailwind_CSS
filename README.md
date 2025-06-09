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
- `Customizable:` **Fully Customizable via the `tailwind.config.js` file** for colors, spacing, fonts, and more.
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
| 1.  **Tailwind Installation and Setup**                                                                        | >> [` CHECK CONTENT `](#tailwind-installation-and-setup)                                      |
| **BEGINNER**  
| 2.  **Basic `Layout` Utility_Classes**                                                                         | >> [` CHECK CONTENT `](#basic-layout-utility_classes)                                         |
| 3.  **Custom-Tkinter Window Geometry(Width x Height)**                                                         | >> [` CHECK CONTENT `](#adjusting-custom_tkinter_window-dimensions)                           |
| 4.  **Creating Custom-Tkinter Window Instance (CTk( ))**                                                       | >> [` CHECK CONTENT `](#creating-custom_tkinter_window_instance-CTk)                          |
</div>

---

## Tailwind Installation and Setup
### 1. Using Play_CDN(Content Delivery Network) [QUICKEST METHOD]:
- The `Play CDN` lets you load `Tailwind's Core_Utilities` into your project **without any Build Step**.
- `Without any Build Step:` Normally, with a Full Tailwind_Setup, you’d need `Node_Js`, `npm` (To install Tailwind) and sometimes a Build_Tool like `Vite`. But, with `Play_CDN`, you can skip all of that — **No Configuration**, **No Installation**, **No Compiling**.
- All the **Utility_Classes** are **preloaded** via the CDN Servers!
- It is great for **Prototyping** and **Demos** but `Not Applicable in a Production Environment` as it is **Heavy** (Loads all utilities at once, even if you require a few), **No Customization** (You can’t configure Tailwind themes, colors, etc. via `tailwind.config.js` File), **No JIT** (No Just-In-Time Compiler Used), **No Purging Of Unused Classes**, etc.
- Go to [`Play_CDN Docs`](https://tailwindcss.com/docs/installation/play-cdn).
- **Copy** the `CDN Script` from the Page:
  ```
  <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
  ```
  ![Play_CDN Script](https://github.com/user-attachments/assets/900289e2-7731-437a-b633-f71047743411)<br>
- Paste it inside the `<head> Tag` of your `HTML`:
  ```
  <head>
     <meta charset="UTF-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>Tailwind-Bootcamp</title>

     <!-- Play_CDN Script -->
     <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
  </head>
  ```
- Now you are ready to use `Tailwind's Utility_Classes` directly in your `HTML` without any Setup or Build Process!
<br>

### 2. Using Tailwind_CLI:
- Tailwind CLI is the official Command-Line Interface provided by Tailwind CSS that allows you to:
  - **Compile** your Tailwind CSS from Source to a **usable CSS_File** (typically `output.css`).
  - **Without needing a Build_Tool** (Ex: Vite).
- `Note:` You need to [`Install and Setup Node_Js`](https://nodejs.org/en/download) for this Method.
- Go to [`Tailwind_CLI Docs`](https://tailwindcss.com/docs/installation/tailwind-cli).
- **Copy** and **Run** the `npm Command` from the Page, in your `Terminal`, to install `Tailwind_CSS` and `Tailwind_CLI`:
  ```
  npm install tailwindcss @tailwindcss/cli
  ```
- Next, **Import** `Tailwind_CSS` in you **Main CSS_File** (`style.css`).<br>
  `For Ex:` Suppose **style.css**:
  ```
  @import "tailwindcss";
  ```
- **Run** the `Tailwind_CLI Tool`, to scan your **Project_Files** for **Utility_Classes** and **Build your CSS**, using the following `npx Command`:
  ```
  npx @tailwindcss/cli -i ./path/to/main.css -o ./path/to/output.css --watch
  ```
  - `-i:` It specifies the path to your **Input CSS_File** (`./path/to/main.css` or `./path/to/style.css`).
  - `-o:` It specifies the path where you want to define your **Output CSS_File** (`./path/to/output.css`).
  - `--watch:` Keeps **Watching / Scanning** the Project_Files(`.html`) for changes while you develop.
  - `NOTE:` You need to **Run** the **Above Command** `Each Time you Start your Project` to **Compile** and **Watch** `Tailwind CSS` for changes.
- Add the **newly compiled** `CSS_File` (`output.css`) inside the `<head> Tag` of your `HTML`:
  ```
  <head>
     <meta charset="UTF-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>Tailwind-Bootcamp</title>

     <!-- Linking output.css -->
     <link href="./output.css" rel="stylesheet">
  </head>
  ```
  ![Tailwind_CLI](https://github.com/user-attachments/assets/1d4d70f4-f4f5-48c5-90a3-4c59a6da7e11)<br>
- Now you are all set to use `Tailwind's Utility_Classes` in your Project efficiently!
<br>

### 3. Using Vite:
- `Vite` is a **Modern Build_Tool** and **Development_Server** that dramatically improves the `UI_development (Frontend)` experience.
- **Prerequisites:**
  - You need to [`Install and Setup Node_Js`](https://nodejs.org/en/download) for this Method.
  - You also need to [`Utilize the Vite Build_Tool`](https://vite.dev/guide/), by using the following **Command**:
    ```
    npm create vite@latest my-app --template react
    ```
    After **Executing** the **Command**, Follow the `Guided_Steps` shown in the `Terminal` to Setup `React` using the `Vite Build Tool`.
- Go to [`Tailwind_CLI Docs`](https://tailwindcss.com/docs/installation/tailwind-cli).
- **Copy** and **Run** the `npm Command` from the Page, in your `Terminal`, to install `Tailwind` and `@tailwindcss/vite`:
  ```
  npm install tailwindcss @tailwindcss/vite
  ```
- Next, Add the `@tailwindcss/vite` **Plugin** to your `Vite_Configuration` (i.e, `vite.config.js` or `vite.config.ts` File):<br>
  `For Ex:` Suppose **vite.config.js**:
  ```
  import path from "path";
   import { defineConfig } from "vite";
   import react from "@vitejs/plugin-react";

   // Import @tailwindcss/vite Plugin
   import tailwindcss from "@tailwindcss/vite";

   // https://vite.dev/config/
   export default defineConfig({
     plugins: [react(), tailwindcss()], //Add TailwindCSS to the List_of_Plugins
     resolve: {
       alias: {
         "@": path.resolve("./src"),
       },
     },
   });
  ```
- Next, **Import** `Tailwind_CSS` in you **Main CSS_File** (`index.css`).<br>
  `For Ex:` Suppose **index.css**:
  ```
  @import "tailwindcss";
  ```
- Make sure the `Compiled CSS_File` (`App.css`) is imported inside your `App.jsx` or `App.tsx` File:<br>
  `For Ex:` Suppose **App.jsx**:
  ```
  import "./App.css";
   import { Button } from "./components/ui/button";

   function App() {
     return (
       <>
         <Button>hello</Button>
       </>
     );
   }

   export default App;
  ```
  ![Tailwind_for_Vite](https://github.com/user-attachments/assets/946af695-d2c9-4856-94b9-2c27bbc1bb2e)<br>
- Now you are all set to use `Tailwind's Utility_Classes` in your **Vite: React_Project** efficiently!
<br>

<div align="center">
   
   **`Note:` The `Setup_Steps` in the Above Methods are aligned with the Latest `Tailwind_CSS Version` at the Time, i.e., `Tailwind_CSS v4.1`.**
</div>
<br>
   
---
<br>

## Basic Layout Utility_Classes
The `Layout Classes` define how elements are **displayed**, how they **take up space**, and how they are **positioned** within the `Document Flow (DOM -- Document Object Model)`.
<br>

### Tailwind Spacing_Scale:
- Before diving into the `Layout Utility_Classes`, it's important to First understand the underlying **Measurement Scale** i.e, `Tailwind Spacing_Scale`.
- The `Tailwind Spacing_Scale` provides a **Consistent Set of Spacing Values** used across various **Layout Utility_Classes**.
- These values are added as `-suffix` to the `Layout Utility_Classes` for defining the **Volume** to be applied.

|**Tailwind Spacing_Scale**     |**Rem**             |**Pixels**          |
|-------------------------------|--------------------|--------------------|
|0                              |0                   |0                   |
|0.5                            |0.125rem            |2px                 |
|1                              |0.25rem             |4px                 |
|1.5                            |0.375rem            |6px                 |
|2                              |0.5rem              |8px                 |
|2.5                            |0.625rem            |10px                |
|3                              |0.75rem             |12px                |
|4                              |1rem                |16px                |
|5                              |1.25rem             |20px                |
|6                              |1.5rem              |24px                |
|7                              |1.75rem             |28px                |
|8                              |2rem                |32px                |
|9                              |2.25rem             |36px                |
|10                             |2.5rem              |40px                |
**and so on . . . **
- **`Note:`** You can also **input** `Custom Scale` using `Square_Brackets []` around the `-suffix` Values.<br>
`For Ex:` **w-[50px]**, this specifes the **Width** of the element to be **50px**.   
<br>
<br>

### Element Display_Type:
The `Display Classes` control how an **<HTML> element** is rendered in the `Document Flow (DOM -- Document Object Model)`.
- **`inline`:** **Inline Elements** sit within the **Same Line** as surrounding content and only take up the necessary space required by the content. Hence, they do not permit **Width** and **Height** Configuration in design.
- **`block`:** **Block Elements** start on a **New Line** and take up the **Full Width** available, effectively pushing Subsequent Content to the Next Line.
- **`inline-block`:** **Inline-block Elements** behave like **Inline Elements**, but they also have the **Block-Level characteristics** of being able to configure **Width**, **Height**, and **Margins**.
- **`hidden`:** It is a `Boolean-Attribute` (On / Off), indicating that the **Browser** should **Not Render** the Contents of the Elements.
<br>
<br>

### Element Spacing [Margins and Padding]:
The `Element_Spacing Classes` are used to **Add Space Around or Inside elements**. These are crucial for creating **Readable** and **Visually Balanced** Layouts.<br>
`Tailwind_CSS` provides **Granular_Control** over spacing using `Margin` and `Padding` Classes.
<br>

1. **Margin Classes:**
The `Margin` adds **Space Outside the Element’s Border**, separating it from Neighboring Elements.
- **`m-2`:** Sets **Margin on all Sides** for an Element.
- **`mx-2`:** Sets **Margin along X-axis (i.e, Left and Right)** for an Element.
- **`my-2`:** Sets **Margin along Y-axis (i.e, Top and Bottom)** for an Element.
- **`mt-2`:** Sets **Margin towards Top** for an Element.
- **`mb-2`:** Sets **Margin towards Bottom** for an Element.
- **`ml-2`:** Sets **Margin on the Left SSide** of an Element.
- **`mr-2`:** Sets **Margin on the Right Side** of an Element.
<br>

2. **Padding Classes:**
The `Padding` adds **Space Inside the Element’s Border**, positioning the Content within an Element.
- **`p-2`:** Sets **Padding on all Sides** for an Element.
- **`px-2`:** Sets **Padding along X-axis (i.e, Left and Right)** for an Element.
- **`py-2`:** Sets **Padding along Y-axis (i.e, Top and Bottom)** for an Element.
- **`pt-2`:** Sets **Padding towards Top** for an Element.
- **`pb-2`:** Sets **Padding towards Bottom** for an Element.
- **`pl-2`:** Sets **Padding on the Left SSide** of an Element.
- **`pr-2`:** Sets **Padding on the Right Side** of an Element.<br>
![Margin and Padding](https://github.com/user-attachments/assets/f15df0d0-8722-494c-9462-380d3b9006fc)<br>
<br>

3. **Child-Elements Spacing Utilities:**
The `Child-Elements Spacing Utilities` (also known as `Space-Between Utilities`) are used to **Create Consistent Spacing between Direct Children** of a Parent Container, without manually applying **Margin** to each Child Element.<br>
`Note:` This `Utility_Class` is applied on the `Parent_Element` and not the Children directly.
- **`space-x-5`:** It is used to **Apply Margin on the Left Side of all Children except the First Child** within the Parent_Element.
- **`space-y-5`:** It is used to **Apply Margin towards Top of all Children except the First Child** within the Parent_Element.
<br>
<br>

### Element Sizing:
The `Sizing Classes` control an Element's `width`, `height`, `min/max dimensions`, and how it behaves inside its Container. 
<br>

1. **Width Classes:**
It is used to set the `Width` of an Element.
- **`w-0`:** **Width=0px** or **Width=0%**.
- **`w-1/2`:** **Width=50%**
- **`w-full`:** **Width=100%**
- **`w-10`:** Sets **Custom Width**, using the **Tailwind Spacing_Scale**, for an Element. [**Width=40px**]
- **`w-screen`:** Sets the Element to **Cover the Full_Available_Width** on a Screen. [**Width=100vw** i.e (100 Vertical-Width)]
- **`w-auto`:** Sets the **Width to Automatically Shrink or Grow** based on its Content Size.
<br>

2. **Min/Max-Width Classes:**
It helps to Set a Limit on how **Small** or **Wide** an Element is allowed to get.
- **`min-w-0`:** **Minimum Width=0px** or **Minimum Width=0%**.
- **`min-w-full`:** **Minimum Width=100%**.
- **`min-w-50`:** **Minimum Width=0%**.
- **`max-w-0`:** **Width=50%**
- **`w-full`:** **Width=100%**
- **`w-10`:** Sets **Custom Width**, using the **Tailwind Spacing_Scale**, for an Element. [**Width=40px**]
- **`w-screen`:** Sets the Element to **Cover the Full_Available_Width** on a Screen. [**Width=100vw** i.e (100 Vertical-Width)]
- **`w-auto`:** Sets the **Width to Automatically Shrink or Grow** based on its Content Size.
<br>

3. **Height Classes:**
It is used to set the `Height` of an Element.
- **`h-0`:** **Height=0px** or **Width=0%**.
- **`h-1/2`:** **Height=50%**
- **`h-full`:** **Height=100%**
- **`h-10`:** Sets **Custom Height**, using the **Tailwind Spacing_Scale**, for an Element. [**Height=40px**]
- **`h-screen`:** Sets the Element to **Cover the Full_Available_Height** on a Screen. [**Height=100vh** i.e (100 Vertical-Height)]
- **`h-auto`:** Sets the **Height to Automatically Shrink or Grow** based on its Content Size.
<br>

<br>
<br>

---
<br>

