<div align="center">
   <img src="https://github.com/user-attachments/assets/5f875ede-34c9-424f-90a7-c860996c51fb" alt="Tailwind Logo" width="60%" height="250%">
</div>

# Tailwind CSS

This **Repository** documents my my `Notes`, `Learnings`, and `UI_Project` as I progress through a `Tailwind_CSS Bootcamp` to Master **Modern UI development**.<br>

<div align="center">
   
   **📌 Checkout my Post-Bootcamp [`Tailwind_UI Project`](https://github.com/Yashvant-Chhapwale/Scribe_Smart-Notes)**
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
- `Component-Friendly:` Encourages **Reusable UI_Components** without the need to leave HTML.
- `JIT(Just-In-Time) Engine:` **Utilizes Just-In-Time Compilation** for fast build times and smaller final CSS output. It generates the CSS you need, only when you need it, instead of generating everything up front.
  <br>

<div align="center">
   
   **📌 Visit the [Official_Documentation](https://tailwindcss.com/docs) to know more about `Tailwind_CSS`.**
</div>

---

<div align="center">
 <h1>Index</h1>
</div>

<div align="center">
 
| TITLE                                                                                                                                           | SECTION_LINK                                                                                  |
|-------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| 1.  **Tailwind Version Selection**                                                                                                              |  [` 🔗CONTENT `](#tailwind-version-selection)                                                |
| 2.  **Tailwind Installation and Setup**                                                                                                         |  [` 🔗CONTENT `](#tailwind-installation-and-setup)                                           |
| 3.  **Tailwind_Version Verification**                                                                                                           |  [` 🔗CONTENT `](#tailwind_version-verification)                                             |
| 4.  **Tailwind_CSS VS_Code Extension**                                                                                                          |  [` 🔗CONTENT `](#tailwind_css-vs_code-extension)                                            |
| [**BEGINNER**](#beginner---level)                                                                                                                                                                                                               |
| 5.  **Basic `Layout` Utility_Classes**                                                                                                          |  [` 🔗CONTENT `](#basic-layout-utility_classes)                                              |
| 6.  **`Typography` Utility_Classes**                                                                                                            |  [` 🔗CONTENT `](#typography-utility_classes)                                                |
| 7.  **Element `Shadows` Utility_Classes**                                                                                                       |  [` 🔗CONTENT `](#element-shadows-utility_classes)                                           |
| 8.  **Tailwind `Backgrounds` and `Colors`**                                                                                                     |  [` 🔗CONTENT `](#tailwind-backgrounds-and-colors)                                           |
| [**INTERMEDIATE**](#intermediate---level)                                                                                                                                                                                                       |
| 9.  **Advanced `Layout` Utility_Classes: [`flex`](#flexbox-layout), [`grid`](#grid-layout)**                                                    |  [` 🔗CONTENT `](#advanced-layout-utility_classes)                                           |
| 10. **`Responsive` Layout_Build**                                                                                                               |  [` 🔗CONTENT `](#responsive-layout_build)                                                   |
| 11. **Tailwind's `Dark Mode` Support**                                                                                                          |  [` 🔗CONTENT `](#tailwinds-dark-mode-support)                                               |
| 12. **Tailwind's `Variant Prefixes`**                                                                                                           |  [` 🔗CONTENT `](#tailwinds-variants)                                                        |
| [**ADVANCED**](#advanced---level)                                                                                                                                                                                                               |
| 13. **`Transformations`**                                                                                                                       |  [` 🔗CONTENT `](#transform-utilities)                                                       |
| 14. **`Transitions` & `Animations`**                                                                                                            |  [` 🔗CONTENT `](#transition-and-animation-utilities)                                        |
| 15. **Customizing Tailwind_Utilities with `tailwind.config.js`** [`Update v4: (CSS-First Configuration)`](#tailwind_v4-css-first-configuration) |  [` 🔗CONTENT `](#customizing-tailwind-with-tailwindconfigjs)                                |

</div>

---

## Tailwind Version Selection
- Visit the **Tailwind_CSS** [**`Docs`**](#https://tailwindcss.com/docs) Page.
- Select the **Required** `Tailwind_Version` from the **Version_Dropdown**.
  ![`Version_Dropdown`](https://github.com/user-attachments/assets/32b916da-dbf5-432b-b734-4b8002eef299)<br>
- The `Docs` will provide appropriate Information and Installation Guide with respect to the selected `Tailwind_Version`.
<br>

---
<br>

## Tailwind Installation and Setup

### 1.Using Play_CDN(Content Delivery Network) [QUICKEST METHOD]:
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
  <br>
  <br>

### 2.Using Tailwind_CLI:
- Tailwind CLI is the official Command-Line Interface provided by Tailwind CSS that allows you to:
  - **Compile** your Tailwind CSS from Source to a **usable CSS_File** (typically `output.css`).
  - **Without needing a Build_Tool** (Ex: Vite).
- `Note:` You need to [`Install and Setup Node_Js`](https://nodejs.org/en/download) for this Method.
- Go to [`Tailwind_CLI Docs`](https://tailwindcss.com/docs/installation/tailwind-cli).
- **Copy** and **Run** the `npm Command` from the Page, in your `Terminal`, to install `Tailwind_CSS` and `Tailwind_CLI`:
  ```
  npm install tailwindcss@latest @tailwindcss/cli@latest
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
  <br>
  <br>

### 3.Using Vite:
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
  npm install tailwindcss@latest @tailwindcss/vite@latest
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

## Tailwind_Version Verification
- Open your `Terminal` or `Command_Prompt`.
- Paste the following **CCommand** in your `Terminal` to verify which `Tailwind_Version` you're using:
  ```
  npx tailwindcss -v
  ```
  ![`npx tailwindcss -v`](https://github.com/user-attachments/assets/ddf45185-ef2a-422b-98b4-df8e7eef43f5)<br>
<br>
   
---
<br>

## Tailwind_CSS VS_Code Extension
- You can **Install** the following `Extension` in VS_Code for proper **formatting and ease** in `Tailwind_Code`. 
![Tailwind_CSS IntelliSense](https://github.com/user-attachments/assets/1b9ca91a-0b94-490c-aaa1-016b945dcfba)<br>
<br>
   
---
<br>
<div align="center">
   
   ### BEGINNER - LEVEL
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

| **Tailwind Spacing_Scale** | **Rem**  | **Pixels** |
| -------------------------- | -------- | ---------- |
| 0                          | 0        | 0          |
| 0.5                        | 0.125rem | 2px        |
| 1                          | 0.25rem  | 4px        |
| 1.5                        | 0.375rem | 6px        |
| 2                          | 0.5rem   | 8px        |
| 2.5                        | 0.625rem | 10px       |
| 3                          | 0.75rem  | 12px       |
| 4                          | 1rem     | 16px       |
| 5                          | 1.25rem  | 20px       |
| 6                          | 1.5rem   | 24px       |
| 7                          | 1.75rem  | 28px       |
| 8                          | 2rem     | 32px       |
| 9                          | 2.25rem  | 36px       |
| 10                         | 2.5rem   | 40px       |

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

1. **Margin Classes:** <br>
   The `Margin` adds **Space Outside the Element’s Border**, separating it from Neighboring Elements.

- **`m-2`:** Sets **Margin on all Sides** for an Element.
- **`mx-2`:** Sets **Margin along X-axis (i.e, Left and Right)** for an Element.
- **`my-2`:** Sets **Margin along Y-axis (i.e, Top and Bottom)** for an Element.
- **`mt-2`:** Sets **Margin towards Top** for an Element.
- **`mb-2`:** Sets **Margin towards Bottom** for an Element.
- **`ml-2`:** Sets **Margin on the Left Side** of an Element.
- **`mr-2`:** Sets **Margin on the Right Side** of an Element.
  <br>

2. **Padding Classes:** <br>
   The `Padding` adds **Space Inside the Element’s Border**, positioning the Content within an Element.

- **`p-2`:** Sets **Padding on all Sides** for an Element.
- **`px-2`:** Sets **Padding along X-axis (i.e, Left and Right)** for an Element.
- **`py-2`:** Sets **Padding along Y-axis (i.e, Top and Bottom)** for an Element.
- **`pt-2`:** Sets **Padding towards Top** for an Element.
- **`pb-2`:** Sets **Padding towards Bottom** for an Element.
- **`pl-2`:** Sets **Padding on the Left Side** of an Element.
- **`pr-2`:** Sets **Padding on the Right Side** of an Element.<br>
  ![Margin and Padding](https://github.com/user-attachments/assets/f15df0d0-8722-494c-9462-380d3b9006fc)<br>
  <br>

3. **Child-Elements Spacing Utilities:** <br>
   The `Child-Elements Spacing Utilities` (also known as `Space-Between Utilities`) are used to **Create Consistent Spacing between Direct Children** of a Parent Container, without manually applying **Margin** to each Child Element.<br>
   `Note:` This `Utility_Class` is applied on the `Parent_Element` and not the Children directly.

- **`space-x-5`:** It is used to **Apply Margin on the Left Side of all Children except the First Child** within the Parent_Element.
- **`space-y-5`:** It is used to **Apply Margin towards Top of all Children except the First Child** within the Parent_Element.
  <br>
  <br>

### Element Dividers:

The `Divider Class` is used to **Add `Borders / Dividers` between Adjacent Child_Elements inside a Container**. It is useful when you want `Internal_Dividers` **without adding borders manually** to Each Child.

- **`divide-x-5`:** Adds `Vertical Dividers`**(Here, Weight=20px)** between `Continuous_Elements (Along X-axis)`.
- **`divide-y-5`:** Adds `Horizontal Dividers`**(Here, Weight=20px)** between `Stacked_Elements (Along Y-axis)`.
- **`divide-x-reverse`:** It reverses the `Side` on which `Vertical Dividers` appear when using `divide-x`. Normally, `divide-x` adds a `Left_Border` to all Elements except the First. With `divide-x-reverse`, it instead adds the `Right_Border` to all except the Last Element.
- **`divide-y-reverse`:** It reverses the `Side` on which `Horizontal Dividers` appear when using `divide-y`. Normally, `divide-y` adds a `Top_Border` to all Elements except the First. With `divide-y-reverse`, it instead adds the `Bottom_Border` to all except the Last Element.
  <br>
  <br>

### Element Sizing:

The `Sizing Classes` control an Element's `width`, `height`, `min/max dimensions`, and how it behaves inside its Container.
<br>

1. **Width Classes:** <br>
   It is used to set the `Width` of an Element.

- **`w-0`:** **Width=0px** or **Width=0%**.
- **`w-1/2`:** **Width=50%**
- **`w-full`:** **Width=100%**
- **`w-10`:** Sets **Custom Width**, using the **Tailwind Spacing_Scale**, for an Element. [**Width=40px**]
- **`w-screen`:** Sets the Element to **Cover the Full_Available_Width** on a Screen. [**Width=100vw** i.e (100 Vertical-Width)]
- **`w-auto`:** Sets the **Width to Automatically Shrink or Grow** based on its Content Size.
  <br>

2. **Min/Max-Width Classes:** <br>
   It helps to Set a Limit on how **Small** or **Wide** an Element is allowed to get.<br>
   `Note:` These Classes only help to **Set a Limit** but **do not Resize the Element** (beyond the set boundaries) when the Screen_Size Changes.

- **`min-w-0`:** **Minimum-Width=0px** or **Minimum-Width=0%**.
- **`min-w-full`:** **Minimum-Width=100%**.
- **`min-w-50`:** Sets a **Custom Minimum-Width**, using the **Tailwind Spacing_Scale**, for an Element. [**Minimum-Width=200px**]
- **`max-w-0`:** **Maximum-Width=0px** or **Maximum-Width=0%**.
- **`max-w-full`:** **Maximum-Width=100%**.
- **`max-w-50`:** Sets a **Custom Maximum-Width**, using the **Tailwind Spacing_Scale**, for an Element. [**Maximum-Width=200px**]
  <br>

3. **Height Classes:** <br>
   It is used to set the `Height` of an Element.

- **`h-0`:** **Height=0px** or **Width=0%**.
- **`h-1/2`:** **Height=50%**
- **`h-full`:** **Height=100%**
- **`h-10`:** Sets **Custom Height**, using the **Tailwind Spacing_Scale**, for an Element. [**Height=40px**]
- **`h-screen`:** Sets the Element to **Cover the Full_Available_Height** on a Screen. [**Height=100vh** i.e (100 Vertical-Height)]
- **`h-auto`:** Sets the **Height to Automatically Shrink or Grow** based on its Content Size.
  <br>

4. **Min/Max-Height Classes:** <br>
   It helps to Set a Limit on how **Short** or **Tall** an Element is allowed to get.<br>
   `Note:` These Classes only help to **Set a Limit** but **do not Resize the Element** (beyond the set boundaries) when the Screen_Size Changes.

- **`min-h-0`:** **Minimum-Height=0px** or **Minimum-Height=0%**.
- **`min-h-full`:** **Minimum-Height=100%**.
- **`min-h-50`:** Sets a **Custom Minimum-Height**, using the **Tailwind Spacing_Scale**, for an Element. [**Minimum-Height=200px**]
- **`max-h-0`:** **Maximum-Height=0px** or **Maximum-Height=0%**.
- **`max-h-full`:** **Maximum-Height=100%**.
- **`max-h-50`:** Sets a **Custom Maximum-Height**, using the **Tailwind Spacing_Scale**, for an Element. [**Maximum-Height=200px**]
  <br>

5. **Shorthand Class (`size`):** <br>
   Starting from `Tailwind v3.2+`, you can use the `size` **Shorthand_Class**, to simultaneously set `Width` and `Height` for an Element.

- **`size-10`:** Simultaneously sets the **Width** and **Height** of an Element. (**Width=40px** and **Height=40px**)
  <br>
  <br>

### Element Border:

The `Border Classes` control an **Element's Border_Attributes** including `width (thickness)`, `style`, and `radius`.
<br>

1. **Border Width:** <br>
   It control how `Thick` the **Border** can be.

- **`border`:** Adds a **Default(1px) Border** to the Element.
- **`border-0` or `border-none`:** **Removes Border** from the Element.
- **`border-2`:** Sets a **Custom Border-Width**, using the **Tailwind Spacing_Scale**, for an Element. [**Border=8px**]
- **`border-x-2`:** Sets **Border along X-axis (i.e, Left and Right)** for an Element.
- **`border-y-2`:** Sets **Border along Y-axis (i.e, Top and Bottom)** for an Element.
- **`border-t-2`:** Sets **Border towards Top** for an Element.
- **`border-b-2`:** Sets **Border towards Bottom** for an Element.
- **`border-l-2`:** Sets **Border on the Left Side** of an Element.
- **`border-r-2`:** Sets **Border on the Right Side** of an Element.
  <br>

2. **Border Style:** <br>
   It helps to Set a `Pattern`/`Design` for the **Border**.

- **`border-solid`:** Default Solid Line. (────────────────)
- **`border-dashed`:** Dashed Line. (— — — — — — — —)
- **`border-dotted`:** Dotted Line. (· · · · · · · ·)
- **`border-double`:** Double Line. (═══════════════)
  <br>

3. **Border Radius:** <br>
   It is used to make an **Element's_Corners** `Rounded`.

- **`rounded`:** Set the **Default Roundedness (i.e, 0.25rem)** for an Element's Corners.
- **`rounded-full`:** Makes the Element's Border **Fully Rounded**.
- **`rounded-sm`:** Set the Border_Radius to **Small_Radius (i.e, 0.125rem or 2px)**.
- **`rounded-md`:** Set the Border_Radius to **Medium_Radius (i.e, 0.375rem or 6px)**.
- **`rounded-lg`:** Set the Border_Radius to **Large_Radius (i.e, 0.5rem or 8px)**.
- **`rounded-xl`:** Set the Border_Radius to **Extra-Large_Radius (i.e, 0.75rem or 12px)**.
- **`rounded-2xl`:** **Border-Radius=1rem or 16px**.
- **`rounded-2xl`:** **Border-Radius=1.5rem or 24px**.<br>
  **and so on. . .**
  <br>
  <br>

### Element Outline:

The `Outline Classes` control the **Style** of an `Element's Outline` which appears when an **Element** is `Focused`.
<br>

1. **Outline Width:** <br>
   It control how `Thick` the **Outline** can be.

- **`outline`:** Adds a **Default(1px) Solid Outline** to the Element.
- **`outline-none` or `border-none`:** **Removes Outline** from the Element.
- **`outline-1`:** Sets a **Custom Outline-Width**, using the **Tailwind Spacing_Scale**, for an Element. [**Outline=4px**]
- **`outline-2`:** Sets a **Custom Outline-Width**, using the **Tailwind Spacing_Scale**, for an Element. [**Outline=8px**]<br>
  **and so on . . .**
  <br>

2. **Outline Style:** <br>
   It helps to Set a `Pattern`/`Design` for the **Outline**.

- **`outline-solid`:** Default Solid Line. (────────────────)
- **`outline-dashed`:** Dashed Line. (— — — — — — — —)
- **`outline-dotted`:** Dotted Line. (· · · · · · · ·)
- **`outline-double`:** Double Line. (═══════════════)
  <br>

3. **Outline Offset:** <br>
   It is used to `Add Space` between an **Element's Outline** and its **Border_Edges**.

- **`outline-offset-0`:** **Default/No_Spacing** between the **Outline** and the **Border_Edges**.
- **`outline-offset-1`:** Sets a **Custom Spacing** between the **Outline** and the **Border_Edges**. [**Outline-Offset=4px**]
- **`outline-offset-2`:** Sets a **Custom Spacing** between the **Outline** and the **Border_Edges**. [**Outline-Offset=8px**]
  **and so on. . .**<br>
  ![`outline-offset`](https://github.com/user-attachments/assets/803ff6e5-8753-453e-8fd8-33c42853f48e)<br>
  <br>
  <br>

### Element Box_Sizing:

The `Box_Sizing Classes` define how the **Total Width and Height of an Element are calculated**, specifically, whether `Padding and Borders` are `Included Inside` or `Added Outside` the `Width`/`Height`.

- **`box-border`:** It tells the **Browser** to **Include the Element's Borders and Padding** when you give it a `Height` or `Width`.<br>
  `For Ex:` Suppose an Element has class="box-border size-32 border-4 p-4" i.e, Size(Width and Height)=128px, Border=16px, Padding=16px<br>
  ![box-border](https://github.com/user-attachments/assets/4c31aa79-f1bd-44b7-98fd-1f961fbfb93e)<br>
  Then, you can observe that the **Size** i.e **Width & Height** also accounts for fitting the **Border & Padding Dimensions** for an Element.
- **`box-content`:** It tells the **Browser** to **Add Borders and Padding on Top of an Element's specified Width or Height**.<br>
  `For Ex:` Suppose an Element has class="box-content size-32 border-4 p-4" i.e, Size(Width and Height)=128px, Border=16px, Padding=16px<br>
  ![box-content](https://github.com/user-attachments/assets/52faaaaa-9f17-4689-b053-6efe8fdbe7c1)<br>
  Then, you can observe that the **Size** i.e **Width & Height** only accounts for the **Content** of the Element excluding the **Border & Padding Dimensions**.
  <br>
  <br>
  <br>

### Element Flow_Control:

The `Flow_Control Classes` control how Elements **Flow Inside their Containers and Relate to Other Elements** within the `DOM (Document Object Model)`.<br>
They are **responsible** for controlling the **Positioning** of the Elements.
These `Utility_Classes` are essential for **Building Layouts**, **ToolTips**, **Modals**, **Floating Elements**, and more.
<br>

1. **Container Class:** <br>

- The `Container Class` i.e, `container` is used t0 **Set a Responsive, Centered, and Padded Wrapper** for your content.<br>
- `Note:` It does not **Center** the content itself, it only manages the **Positioning** for the **Outer_Division/Wrapper**.
- It automatically adjusts its `Max-Width` at each `Breakpoint` as follows:
  - `sm`: Small_Screen Breakpoint (`640px`).
  - `md`: Medium_Screen Breakpoint (`768px`).
  - `lg`: Large_Screen Breakpoint (`1024px`).
  - `xl`: Extra-Large_Screen Breakpoint (`1280px`).
- This helps in creating a `Responsive Interface`.
- **`For Ex:`**
  ```
  <div class="container mx-auto py-15">
      <p class="text-3xl text-blue-600 font-bold">
        I am a Container!
      </p>
  </div>
  ```
  <br>

2. **Inset Classes:** <br>
   `Inset` (also knowsn as `Offset`) refers to the **Distance Between an Element and the Edges of its Containing Block**.<br>
   The `Inset Classes` control **how far a Positioned Element is Moved from its Reference Edges**, viz. `Top`, `Right`, `Bottom`, and `Left`.<br>
   `Note:` These **Classes** only only apply when the Element is using a `relative`, `absolute`, `fixed`, or `sticky` Position.

- **`top-2`:** **Moves the Element Down** from the `Top_Edge`.
- **`bottom-2`:** **Moves the Element Up** from the `Bottom_Edge`.
- **`left-2`:** **Moves the Element Right** from the `Left_Edge`.
- **`right-2`:** **Moves the Element Left** from the `Right_Edge`.
- **`inset-2`:** **Offsets the Element** by a Uniform Distance (**8px**) **from all Four Sides**.
- **`inset-x-2`:** **Offsets the Element from the `Left` and `Right` Edges simultaneously.**
- **`inset-y-2`:** **Offsets the Element from the `Top` and `Bottom` Edges simultaneously.**<br>
  `Negative_Inset Classes ` (`Negative_Offsets`) allow you to **Pull an Element in the Opposite Direction** from where it's **Normally Positioned**.
- **`-top-2`:** **Pulls the Element Up** from its normal positioning.
- **`-bottom-2`:** **Pulls the Element Down** from its normal positioning.
- **`-left-2`:** **Pulls the Element Towards Left** from its normal positioning.
- **`-right-2`:** **Pulls the Element Towards Right** from its normal positioning.
  <br>
  <br>
  
3. **Position Classes:** <br>
   The `Position Classes` in control **how an Element is Positioned** within the `Document_Flow` or `Relative to its Parent`.

- **`static`:** It is the **Default Position_Style** for Elements. The `Static_Elements` follows the `Normal Document_Flow`. We cannot apply `Inset_Classes` to Elements with `Static_Positioning`, however `Padding` & `Margins` work as expected.<br>
  `For Ex:`
  ```
  <div>
     <h2>Static Positioning</h2>
     <div class="flex flex-row justify-center items-center p-10 border-2 border-gray-600">
        <div class="bg-red-500 text-white p-20 m-2 rounded-lg font-bold">
           Red Box
        </div>
        <div class="static top-10 left-10 bg-green-500 text-white p-20 m-2 rounded-lg font-bold">
           Green Box
        </div>
        <div class="bg-blue-500 text-white p-20 m-2 rounded-lg font-bold">
           Blue Box
        </div>
      </div>
  </div>
  ```
  ![`static`](https://github.com/user-attachments/assets/746a092f-806e-438f-9e42-13cd0eab91f4)<br>
  As you can Observe, the `top-10` and `left-10` **Classes** are not working and the `Green Box` follows the `Normal Document_Flow`.
  <br>
  <br>
  
- **`relative`:** The **Element** is **Positioned Relative to its Normal Position**. The **Element** follows the `Normal Document_Flow`, but you can use the `Inset Classes` to further **nudge it around**.<br>
  `For Ex:`
  ```
  <div>
     <h2>Relative Positioning</h2>
     <div class="flex flex-row justify-center items-center p-10 border-2 border-gray-600">
        <div class="bg-red-500 text-white p-20 m-2 rounded-lg font-bold">
           Red Box
        </div>
        <div class="relative top-10 left-10 bg-green-500 text-white p-20 m-2 rounded-lg font-bold">
           Green Box
        </div>
        <div class="bg-blue-500 text-white p-20 m-2 rounded-lg font-bold">
           Blue Box
        </div>
      </div>
  </div>
  ```
  ![`relative`](https://github.com/user-attachments/assets/3bb3dda8-292f-4b23-a47c-50a402dd4966)<br>
  As you can Observe, the **Element** follows the `Normal Document_Flow` (Red Box >> Green Box >> Blue Box), but it also utilizes the `top-10` and `left-10` classes to further position itself unlike the `Static Element`.
  <br>
  <br>
  
- **`absolute`:** The **Element** is **Positioned Relative to the nearest Positioned Ancestor(Parent)** (Ancestors are basically Parent_Elements utilizing Position_Classes such as `relative`,`absolute`,`fixed`,etc not including `static`).If there are **No** `Positioned_Ancestors` then the Element positions itself `Relative` to the `<HTML> Element`.<br>
  `For Ex:`
  ```
  <div>
     <h2>Absolute Positioning</h2>
     <div class="relative flex flex-row justify-center items-center p-10 border-2 border-gray-600">
        <div class="bg-red-500 text-white p-20 m-2 rounded-lg font-bold">
           Red Box
        </div>
        <div class="absolute top-10 left-10 bg-green-500 text-white p-20 m-2 rounded-lg font-bold">
           Green Box
        </div>
        <div class="bg-blue-500 text-white p-20 m-2 rounded-lg font-bold">
           Blue Box
        </div>
      </div>
  </div>
  ```
  ![`absolute`](https://github.com/user-attachments/assets/9cd00fbc-d95a-4103-ad2c-f5db268dc943)<br>
  As you can Observe, the `absolute` Element i.e, **Green Box** positions itself at `top-10` and `left-10` Insets **Relative** to the `relative` Parent i.e, **Outer_Div with Gray_border**.
  <br>
  <br>
  
- **`fixed`:** The Element is **Positioned Relative to the Viewport (Browser_Window)**. It stays **Fixed** in the **Same Place** even when **Scrolling**.<br>
  `For Ex:`
  ```
  <div class="fixed bottom-10 right-10 bg-green-500 text-white p-16 m-2 rounded-lg font-bold">
     This is Fixed Box
  </div>
  ```
  ![`fixed`](https://github.com/user-attachments/assets/8ef395f4-cd42-4c79-847c-fc23f2c6c64d)<br>
  As you can Observe, the **Green Box** remains `fixed` at `bottom-10` and `right-10`, on the **Visible Screen (Viewport)**, even when **Scrolling**.
  <br>
  <br>
  
- **`sticky`:** The Element is treated as `relative` until it reaches a **Defined Scroll_Position** (Threshold -- `top`.`bottom`,`left`,`right`), after which it behaves like a `fixed` Element. Basically, it **Scrolls** until it `sticks` to a **Defined Position** and then stays `fixed` on that position.<br>
  `For Ex:`
  ```
  <div>
     <h2>Sticky Positioning</h2>
     <div class="flex flex-col justify-center items-center p-10 border-2 border-gray-600">
        <div class="bg-red-500 text-white p-20 m-2 rounded-lg font-bold">
           Red Box
        </div>
        <div class="sticky top-5 bg-green-500 text-white p-20 m-2 rounded-lg font-bold">
           Green Box
        </div>
        <div class="bg-blue-500 text-white p-20 m-2 rounded-lg font-bold">
           Blue Box
        </div>
      </div>
  </div>
  ```
  `Initial Position:`<br>
  ![`sticky` >> Initial Position](https://github.com/user-attachments/assets/c881e7d9-e246-43d7-9f72-1941d50dd9a6)<br>
  `After Scrolling Down:`<br>
  ![`sticky` >> After Scrolling-Down](https://github.com/user-attachments/assets/33b09a2b-5815-4d16-b303-4241a1e20eb4)<br>
  As you can Observe, **initially** the **Green Box** follows the `Normal Document_Flow`, but on **scrolling down** as soon as the **Green Box** is at a distance of `20px`(5 -- Tailwind Spacing_Scale) from the **Top_Side** i.e, `top-5` it becomes `fixed`, even **overlaps** the **Blue Box**.
  <br>
  <br>
  
4. **z-index Classes:** <br>
   The `z-index` controls the **Stacking order of Elements** on the **Z-axis** (`front`-to-`back`). Basically, it controls which Element appears on **Top** when **Overlapping**.<br>

- **`z-0`:** **Default Stacking_Level**, i.e, every Element on the Same Plane.
- **`z-10`, `z-20`, `z-30` and so on:** **Higher Stacking_Levels** i.e, Greater the `-suffix` Value higher the Stacking_Level.<br>
  `For Ex:` Element with `z-30` overlaps Element with `z-10`.
- **`z-auto`:** Uses the **Browser’s Default Stacking Configuration**.
  <br>
  <br>
  
5. **Float Classes:** <br>
   The `float` **Classes** are used to **`float` Elements to the Left or Right**, inside a container, making **Other Content Wrap around them**.

- **`float-left`:** **Floats** the Element to the `Left_Side` within a **Container** or **<div>**, allowing other content to **Flow** or **Wrap** around it.<br>
  `For Ex:`

  ```
  <div class="p-10 mx-100 border-2 border-gray-600">
     <div class="float-left w-[200px] h-[150px] p-15 m-2 bg-blue-400 text-white text-center">
        Float-Left
     </div>
     <p class="margin-x-10 text-lg">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Blanditiis
        dolor odio maxime quis fugiat, laboriosam iusto voluptatibus
        incidunt corrupti modi reiciendis impedit cum dolore temporibus
        harum. Vel voluptas numquam nostrum enim commodi quisquam! Labore
        sit numquam et porro provident corporis, hic ullam ex quo voluptas!
        Delectus exercitationem, deleniti reprehenderit explicabo beatae
        dicta repellat ipsam aspernatur praesentium dignissimos deserunt
        dolorum eligendi. Minima laborum maiores quos mollitia numquam sequi
        cupiditate quasi provident, iste quaerat veniam quis harum porro
        eveniet ipsam, cumque voluptatum animi neque aperiam temporibus
        sint. Sapiente eius porro alias, dolore tenetur eum. Voluptates
        sequi neque dolores quo ab, repellendus, voluptate magni reiciendis
        fugiat dicta iure, provident blanditiis aperiam sapiente deserunt
        voluptas ut est? Dolores necessitatibus laudantium ea veniam odit.
        Ad optio animi vel provident. Corrupti ad at, facere asperiores
        obcaecati porro, laboriosam molestias ipsam architecto incidunt
        sequi exercitationem voluptatem rerum.
     </p>
  </div>
  ```

  ![`float-left`](https://github.com/user-attachments/assets/c93777db-03e6-402b-82d5-5b6dae12558f)<br>
  As Observed, the `Float-Left` Element is aligned towards `Left_Side` within the Outer (Parent) Container, while the `<p> (Paragraph` Element Wraps around it from the `Right_Side`.
  <br>
  <br>
  
- **`float-right`:** **Floats** the Element to the `Right_Side` within a **Container** or **<div>**, allowing other content to **Flow** or **Wrap** around it.<br>
  `For Ex:`
  ```
  <div class="p-10 mx-100 border-2 border-gray-600">
     <div class="float-right w-[200px] h-[150px] p-15 m-2 bg-blue-400 text-white text-center">
        Float-Right
     </div>
     <p class="margin-x-10 text-lg">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Blanditiis
        dolor odio maxime quis fugiat, laboriosam iusto voluptatibus
        incidunt corrupti modi reiciendis impedit cum dolore temporibus
        harum. Vel voluptas numquam nostrum enim commodi quisquam! Labore
        sit numquam et porro provident corporis, hic ullam ex quo voluptas!
        Delectus exercitationem, deleniti reprehenderit explicabo beatae
        dicta repellat ipsam aspernatur praesentium dignissimos deserunt
        dolorum eligendi. Minima laborum maiores quos mollitia numquam sequi
        cupiditate quasi provident, iste quaerat veniam quis harum porro
        eveniet ipsam, cumque voluptatum animi neque aperiam temporibus
        sint. Sapiente eius porro alias, dolore tenetur eum. Voluptates
        sequi neque dolores quo ab, repellendus, voluptate magni reiciendis
        fugiat dicta iure, provident blanditiis aperiam sapiente deserunt
        voluptas ut est? Dolores necessitatibus laudantium ea veniam odit.
        Ad optio animi vel provident. Corrupti ad at, facere asperiores
        obcaecati porro, laboriosam molestias ipsam architecto incidunt
        sequi exercitationem voluptatem rerum.
     </p>
  </div>
  ```
  ![`float-right`](https://github.com/user-attachments/assets/2578495b-8a38-441e-8f0f-11a23baccf1f)<br>
  As Observed, the `Float-Right` Element is aligned towards `Right_Side` within the Outer (Parent) Container, while the `<p> (Paragraph` Element Wraps around it from the `Left_Side`.
  <br>
- **`float-none`:** **Removes Float Property** from an Element.
  <br>
  <br>

6. **Clear Classes:** <br>
   The `clear` **Classes** are used to **Prevent an element from Wrapping around the `Floating_Elements`**. They are used in **Conjunction** with the `float` **Classes**.

- **`clear-left`:** **Prevents** the Elements from being **Positioned next to Elements Floating on the Left_Side**.<br>
  `For Ex:`
  ```
   <div class="p-10 mx-100 border-2 border-gray-600">
      <div class="float-left w-[200px] h-[150px] p-15 m-2 bg-blue-400 text-white text-center">
         Float-Left
      </div>
      <p class="clear-left margin-x-10 text-lg">
         Lorem, ipsum dolor sit amet consectetur adipisicing elit. Blanditiis
         dolor odio maxime quis fugiat, laboriosam iusto voluptatibus
         incidunt corrupti modi reiciendis impedit cum dolore temporibus
         harum. Vel voluptas numquam nostrum enim commodi quisquam! Labore
         sit numquam et porro provident corporis, hic ullam ex quo voluptas!
         Delectus exercitationem, deleniti reprehenderit explicabo beatae
         dicta repellat ipsam aspernatur praesentium dignissimos deserunt
         dolorum eligendi. Minima laborum maiores quos mollitia numquam sequi
         cupiditate quasi provident, iste quaerat veniam quis harum porro
         eveniet ipsam, cumque voluptatum animi neque aperiam temporibus
         sint. Sapiente eius porro alias, dolore tenetur eum. Voluptates
         sequi neque dolores quo ab, repellendus, voluptate magni reiciendis
         fugiat dicta iure, provident.
      </p>
   </div>
  ```
  ![`clear-left`](https://github.com/user-attachments/assets/65fadd20-03e8-4faa-815c-9a0803e93817)<br>
  As Observed, the `<p> Paragraph` Element which initially wrapped around the `Float-Left` Element, now starts on the **Next_Line** after the `Float-Left` Element.
  <br>
  <br>
  
- **`clear-right`:** **Prevents** the Elements from being **Positioned next to Elements Floating on the Right_Side**.<br>
  `For Ex:`
  ```
  <div class="p-10 mx-100 border-2 border-gray-600">
     <div class="float-right w-[200px] h-[150px] p-15 m-2 bg-blue-400 text-white text-center">
        Float-Right
     </div>
     <p class="clear-right margin-x-10 text-lg">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Blanditiis
        dolor odio maxime quis fugiat, laboriosam iusto voluptatibus
        incidunt corrupti modi reiciendis impedit cum dolore temporibus
        harum. Vel voluptas numquam nostrum enim commodi quisquam! Labore
        sit numquam et porro provident corporis, hic ullam ex quo voluptas!
        Delectus exercitationem, deleniti reprehenderit explicabo beatae
        dicta repellat ipsam aspernatur praesentium dignissimos deserunt
        dolorum eligendi. Minima laborum maiores quos mollitia numquam sequi
        cupiditate quasi provident, iste quaerat veniam quis harum porro
        eveniet ipsam, cumque voluptatum animi neque aperiam temporibus
        sint. Sapiente eius porro alias, dolore tenetur eum. Voluptates
        sequi neque dolores quo ab, repellendus, voluptate magni reiciendis
        fugiat dicta iure, provident.
     </p>
  </div>
  ```
  ![`clear-right`](https://github.com/user-attachments/assets/e15c10f1-48c1-442c-b4ca-0927076e5b23)<br>
  As Observed, the `<p> Paragraph` Element which initially wrapped around the `Float-Right` Element, now starts on the **Next_Line** after the `Float-Right` Element.
  <br>
  <br>
  
- **`clear-both`:** **Prevents** the Element from being **Positioned next to Elements Floating on Either_Side**, effectively forcing it below all `Floating_Elements`.
- **`clear-none`:** **Removes Clear Property** from an Element.
  <br>

---

<br>

## Typography Utility_Classes

The `Typography Classes` control the **appearance**, **alignment**, **spacing**, and **styling** of `Text` within your `UI`.
<br>

### Text Size:

The `Text-size Classes` control how **Large** or **Small** the Text appears.

- **`text-xs`:** **Extra-Small Text_Size**. Used for `Extra-Small Labels`.
- **`text-sm`:** **Small Text_Size**. Used for `Captions`, `Secondary Text`, etc.
- **`text-base`:** **Default Normal Text_Size**. Used as `Default Body_Text`.
- **`text-lg`:** **Large Text_Size**. Used as `Slightly Larger Body_Text`.
- **`text-xl`:** **Extra-Large Text_Size**. Used for `Headings or Sub-Headings`.
- **`text-2xl`:** **Double Extra-Large Text_Size**. Used for `Headings or Sub-Headings`.
  **and so on . . .**
  <br>
  <br>

### Text Alignment:

The `Text-Alignment Classes` control **how `Inline_Content (like text, <a>, <p>, etc)` are aligned** within its **Parent Container/Element**.

- **`text-left`:** **Aligns Text to the `Left_Side`** within the Parent Container/Element.
- **`text-right`:** **Aligns Text to the `Right_Side`** within the Parent Container/Element.
- **`text-center`:** **Aligns Text to the `Center`** of the Parent Container/Element.
- **`text-start`:** **Aligns Text to the `Start` of the `Writing_Direction`**, Left in Left-To-Right & Right in Right-To-Left.
- **`text-end`:** **Aligns Text to the `End` of the `Writing_Direction`**, Right in Left-To-Right & Left in Right-To-Left.
- **`text-justify`:** **Text is aligned with both the `Left and Right Edges`** of the Container/Element, creating a Clean `Block_of_Text`.
  <br>
  <br>

### Font Weight:

The `Font-Weigth Classes` control how `Bold` or `Light` your Text appears.

- **`font-thin`(100px):** **Extremely Light** (hairline/lightest).
- **`font-extralight`(200px):** **Extra Light**.
- **`font-light`(300px):** **Light**.
- **`font-normal`(400px):** **Regular (Default)**.
- **`font-medium`(500px):** **Slightly Bold**.
- **`font-semibold`(600px):** **Semi_Bold**.
- **`font-bold`(700px):** **Bold**.
- **`font-extrabold`(800px):** **Extra Bold**.
- **`font-black`(900px):** **Ultra Bold** (heaviest).
  <br>
  <br>

### Italic Style:

The `Italic-Style Classes` are used to **Toggle** `Italic_Styling` on Text.

- **`italic`:** Renders the text in `italic` style.
- **`non-italic`:** Removes `italic` styling from the text.
  <br>
  <br>

### Text Transform:

The `Text-Transform Classes` applies `Case_Transformation Styles` and controls `Capitalization` of the **Text_Elements**.

- **`uppercase`:** Transforms all Letters to `Uppercase`.
- **`lowercase`:** Transforms all Letters to `Lowercase`.
- **`capitalize`:** It is used to `Capitalize` the **First_Letter** of each word.
- **`normal-case`:** It **Removes** any `Text-Transform` Styling.
  <br>
  <br>

### Text Decoration:

The `Text-Decoration Classes` are used to **Add** or **Remove** Visual_Styles like `underlines`, `strike-through`, etc. for the **Text_Elements**.

- **`underline`:** Adds an `underline` **below** the Text.
- **`line-through`:** Adds a `Line` through the **Middle** of Text.
- **`overline`:** Adds a `Line` **Above** the Text.
- **`no-underline`:** It **Removes** all `Text_decoration`.
  <br>

1. **Text-Decoration Style:** <br>
   It helps to Set a `Pattern`/`Design` for the **Text-Decoration**.

- **`decoration-solid`:** Default Solid Line. (────────────────)
- **`decoration-dashed`:** Dashed Line. (— — — — — — — —)
- **`decoration-dotted`:** Dotted Line. (· · · · · · · ·)
- **`decoration-double`:** Double Line. (═══════════════)
- **`decoration-wavy`:** Wavy Line, resembles pattern of the Waves. (~~~~~~~~~~~~~)
  <br>

2. **Text-Decoration Thickness:** <br>
   It helps to Control the `Thickness ` of the **Text-Decoration**.

- **`decoration-0`:** **Removes** the Decoration completely.
- **`decoration-1`:** Decoration-Width = 4px (`Thin`).
- **`decoration-2`:** Decoration-Width = 8px (`Default` / `Medium`).
- **`decoration-4`:** Decoration-Width = 16px (`Thick`).
  **and so on . . .**
  <br>
  <br>

### Letter Spacing:

The `Letter-Spacing Classes` control the **`Horizontal Space` between Characters** in a **Text_Element**.

- **`tracking-tighter`(-0.05em):** **Extremely Reduced** Letter_Spacing.
- **`tracking-tight`(-0.025em):** **Slightly Reduced** Letter_Spacing.
- **`tracking-normal`(0em):** Browser's **Default Normal** Letter_Spacing.
- **`tracking-wide`(0.025em):** **Slightly More** Letter_Spacing.
- **`tracking-wider`(0.05em):** Increased **Noticeable** Letter_Spacing.
- **`tracking-widest`(0.1em):** Applies **Maximum Space** between Characters.
  <br>
  <br>

### Line Height:

The `Line-Height Classes` control the `Vertical_Spacing` between **Lines** in a **Text_Element**.

- **`leading-none`(1):** **No Extra_Spacing** between the Lines. (**Tightest**)
- **`leading-tight`(1.25):** **Slightly Tighter_Spacing** between the Lines.
- **`leading-snug`(1.375):** **Slightly Looser_Spacing** between the Lines.
- **`leading-normal`(1.5):** Browser's **Normal** Line_Height with **Comfortable** distance. (**Default**)
- **`leading-relaxed`(1.625):** **Very Loose_Spacing** between the Lines.
- **`leading-loose`(2):** **Extremely Loose_Spacing** between the Lines. (**Maximum Line_Height**)
  <br>

---

<br>

## Element Shadows Utility_Classes

The `Shadow Classes` are used to **apply `Shadows` to Elements and Contents**, giving them **Depth** and **Elevating them Visually**.
<br>

### Box_Shadows:
- **`shadow`:** Applies **Default/Base_Elevation Shadows** to the Elements.
- **`shadow-sm`:** Applies **Small Subtle Shadows** to the Elements.
- **`shadow-md`:** Applies **Medium Shadows** to the Elements.
- **`shadow-lg`:** Applies **Large/Deeper Shadows** to the Elements.
- **`shadow-xl`:** Applies **Extra-Large Shadows** to the Elements.
- **`shadow-2xl`:** Applies **Prominent/Double Extra-Large Shadows** to the Elements.
  **and so on . . .**
- **`shadow-inner`:** Applies **Inset_Shadows** to the Elements. The `Inset_Shadows` create the **Illusion** of a **Shadow appearing within an Element**, rather than Extending Outwards.
<br>
<br>

### Text_Shadows [Introduced with Tailwind_v4.1]: 
- **`text-shadow-2xs`:** Applies **Doubly Extra-Subtle Shadows** to the Elements.
- **`text-shadow-xs`:** Applies **Extra-Subtle Shadows** to the Elements.
- **`text-shadow`:** Applies **Default/Base_Elevation Shadows** to the Elements.
- **`text-shadow-sm`:** Applies **Small Subtle Shadows** to the Text Content.
- **`text-shadow-md`:** Applies **Medium Shadows** to the Text Content.
- **`text-shadow-lg`:** Applies **Large/Deeper Shadows** to the Text Content.<br>
  **`For Ex:`**<br>
  ```
  <h1
     class="text-shadow-lg text-shadow-gray-300 text-center text-fuchsia-500 text-4xl"
  >
     Hello
  </h1>
  ```
  ![`text-shadow`](https://github.com/user-attachments/assets/b4b24d30-29dd-4c52-acdd-8bdddd534ff8)<br>
<br>

---

<br>

## Tailwind Backgrounds and Colors

- `Tailwind_CSS` provides a powerful **Set of Utility_Classes** to handle `Text-Colors`, `Background-Colors`, `Border-Colors` and more.<br>
- It uses a `Systematic Naming_Convention` for applying `Colors` to **Text**, **Backgrounds**, **Borders** and other elements. This convention follows the format of:

  ```
  <element class=" {attribute_name}-{color}-{shade} "
      [CONTENT]
   </element>
  ```

   <div align="center">
   
   **OR**
   </div>

  ```
  {attribute_name}-{color}-{shade}
  ```

- `Tailwind` includes `17 Core Color_Families`, each with `Shades` ranging from **50 (Lightest)** to **950 (Darkest)**.  
  <br>

### Core Color_Families ({color} Suffix):

`Tailwind` includes **17** `Core Color_Families`

- **Black & White:** `white`, `black`. These colors dont have any `Shade_Suffix`.
- **Neutral & Grays:** `slate`, `gray`, `zinc`, `neutral`, `stone`.
- **Warm Tones:** `red`, `orange`, `amber`, `yellow`, `lime`.
- **Warm Tones:** `green`, `emerald`, `teal`, `cyan`, `sky`, `blue`, `indigo`, `violet`, `purple`, `fuchsia`, `pink`, `rose`.
  <br>
  <br>

### Shades ({shade} Suffix):

Each `Color_Family` consists of `Shades` ranging from `50 (Lightest)` to `950 (Darkest)`.

- Shade_Suffixes: `50`, `100`, `200`,`300`, `400`, `500`, `600`, `700`, `800`, `900`, `950`.
  <br>
  <br>

### Basic Utility_Class Prefixes {Attributes} for applying Colors:

Following is a `Collective_List` of some **Basic** `Utility_classes`, which can be used as `Prefixes`, to apply Colors to the same `Utility_Classes`.

- **`text-{color}-{shade}`:** Used to apply `Color_Shades` to `Text-Content`.
- **`bg-{color}-{shade}`:** Used to apply `Background Color` to various `<HTML>` Elements.
- **`border-{color}-{shade}`:** Used to apply `Color_Shades` to `Element-Borders`.
- **`shadow-{color}-{shade}`:** Used to apply `Color_Shades` for `Element-Shadows`.
- **`decoration-{color}-{shade}`:** Used to apply `Color_Shades` to `Text-Decorations` (`underline`, `line-through`, etc.)
- **`placeholder-{color}-{shade}`:** Used to apply `Color_Shades` to `Input_Placeholders`.
- **`divide-{color}-{shade}`:** Used to apply `Color_Shades` to `Dividing_Borders` between Childrens.
  <br>
  <br>

### Backgorund Colors:

`Tailwind` uses the prefix `bg-` to apply **Background_Color** to any `<HTML>` Element.

- It uses the format:
  ```
   class = "bg-{color}-{shade}"
  ```
- Some `<HTML>` **Elements** which can utilize this property are as follows:
  - **`<div>`**
  - **`<section>`**
  - **`<header>`**
  - **`<main>`**
  - **`<footer>`**
  - **`<article>`**
  - **`<span>`**
  - **`<p>`**
  - **`<label>`**
  - **`<input>`**
  - **`<buttom>`**, **and so on . . .**
- **`For Ex:`**
  ```
  <div class="bg-blue-400 p-5 rounded">
     <img src="https://picsum.photos/200/300" alt="" />
  </div>
  ```
  <br>
  <br>

### Backgorund Gradient:

`Tailwind` provides **Special** `Utility Classes` to apply `Background_Gradients` easily without writing **Custom CSS**.

- It uses the format:
  ```
   class = "bg-gradient-to-DIRECTION from-{color}-{shade} to-{color}-{shade}"
  ```
- **`bg-gradient-to-DIRECTION`:** Enables the Background_Gradient and sets the `Direction` of the Gradient.<br>
  The `Directions` are as follows:
  - `bg-gradient-to-t`: Sets `direction` of **Gradient** from `Bottom → Top`.
  - `bg-gradient-to-b`: Sets `direction` of **Gradient** from `Top → Bottom`.
  - `bg-gradient-to-r`: Sets `direction` of **Gradient** from `Left → Right`.
  - `bg-gradient-to-l`: Sets `direction` of **Gradient** from `Right → Left`.
  - `bg-gradient-to-tr`: Sets `direction` of **Gradient** from `Bottom-Left → Top-Right`.
  - `bg-gradient-to-tl`: Sets `direction` of **Gradient** from `Bottom-Right → Top-Left`.
  - `bg-gradient-to-br`: Sets `direction` of **Gradient** from `Top-Left → Bottom-Right`.
  - `bg-gradient-to-bl`: Sets `direction` of **Gradient** from `Top-Right → Bottom-Left`.
- **`from-{color}-{shade}`:** Specifies the `Starting Color_Shade` for the **Gradient**.
- **`to-{color}-{shade}`:** Specifies the `Ending Color_Shade` for the **Gradient**.
- **`For Ex:`**
  ```
  <div class="bg-gradient-to-b from-blue-400 to-blue-900 p-5 rounded">
     <img src="https://picsum.photos/200/300" alt="" />
  </div>
  ```
  <br>
  <br>

### Accent Colors:

The `Accent Color` **Utility** is used to style the **Color** of `Form_Elements` like: `Checkboxes` (`<input type="checkbox"/>`), `Radio` Buttons (`<input type="radio"/>`), `Range` Inputs (`<input type="range"/>`), `Progress` Bar (`<progress>`), etc.

- It follows the format:
  ```
  class = "accent-{color}-{shade}"
  ```
- `For Ex:`
  ```
  <label class="text-pink-500 font-semibold text-center">
    <input class="accent-pink-500" type="checkbox" checked />
    Tick It
  </label>
  ```
     <div>
        <img src="https://github.com/user-attachments/assets/5fd26542-5dd2-45ac-9c67-565793b467e1" alt="Unchecked Checkbox" width="150px" height="50px">
        <img src="https://github.com/user-attachments/assets/e97e1a30-cdda-46f8-b551-0a9dfcfdbfe2" alt="Checked Checkbox" width="150px" height="50px">
     </div>
  <br>
  <br>

### Caret Color:

The `Caret` is the `Blinking_Cursor`/`Input_Cursor` that appears inside Editable Fields (like `<input`, `<textarea>`, etc).<br>
`Tailwind` allows you to **Customize** the **Color** of this `Blinking_Cursor` by utilizing the `caret` Class.

- It uses the format:
  ```
  class = "caret-{color}-{shade}"
  ```
- **`For Ex:`**
  ```
  <div class="text-center">
     <textarea
     class="caret-pink-500 placeholder-pink-500 w-full h-full"
     placeholder="Enter Your Text Here"
     ></textarea>
  </div>
  ```
     <div>
        <img src="https://github.com/user-attachments/assets/7bd5de12-8fb5-4d50-a345-a97051598e9e" alt="Empty Input" width="200px" height="65px">
        <img src="https://github.com/user-attachments/assets/e288653f-ebd0-455f-b14f-628d3e8475da" alt="Blinking_Cursor Input" width="200px" height="65px">
     </div>
  <br>
  <br>

### Outline Color:

The `outline-color` property defines the **Color** of the `Outline` drawn around an **Element** (Ex: `<input/>`, `textarea>`, etc) when it is `Focused`.

- It uses the format:
  ```
  class = "outline-{color}-{shade}"
  ```
- **`For Ex:`**
  ```
  <div class="text-center">
     <textarea
     class="outline-pink-500 caret-pink-500 placeholder-pink-500 w-full h-full"
     placeholder="Enter Your Text Here"
     ></textarea>
  </div>
  ```
  ![`outline-color`](https://github.com/user-attachments/assets/1824d1fe-0543-4a41-8603-6209acafb9e8)<br>
<br>

---
<br>
<div align="center">
   
   ### INTERMEDIATE - LEVEL
</div>
<br>
 
---
<br>

## Advanced Layout Utility_Classes

`Tailwind_CSS` offers a **Powerful Set of `Advanced Layout_Classes`** that help you to Build `Responsive`, `Flexible`, and `Dynamic` **UI_Structures**.<br>
These **Classes** extend the **Core Layout_System** using Utilities for `flexbox`, `grid`, etc, enabling you to design **Complex_Layouts** with **Minimal Effort**.
<br>
<br>

### Flexbox Layout:

`Flexbox` is a **Powerful `1-dimensional` Layout_System** that allows you to create **Complex** and **Responsive** Layouts either `row-wise (Horizontal)` or `column-wise (Vertical)`.

- **`flex`:** Enables `Flexbox` **Layout** for an Element.
- **`inline-flex`:** Makes the **Element** `Flex` as well as `Inline`.
  <br>

1. **Flex Direction:** <br>
   It **defines** the `Direction` in which **Flex_Items** are placed inside a `Flex_Container`.

- **`flex-row` (Default):** Items are placed `Horizontally` from `Left-To-Right (LTR)`. It is the `Default_Direction` followed by **Flex_Items**.
- **`flex-row-reverse`:** It **reverses** the `Order` of Items placed `Horizontally` i.e, makes it `Right-To-Left (RTL)`.
- **`flex-col`:** Items are stacked `Vertically` from `Top-To-Bottom (TTB)`.
- **`flex-col-reverse`:** It **reverses** the `Order` of Items stacked `Vertically` i.e, makes it `Bottom-To-Top (BTT)`.
  <br>

2. **Flex Wrap:** <br>
   It **Controls** whether **Flex_Items** should Stay in a **`Single_Line` or `Wrap` onto `Multiple_Lines`** when there isn't enough space in the `Flex_Container`.

- **`flex-nowrap` (Default):** By `Default`, the Items `Stay on One_Line` and may **Shrink**.
- **`flex-wrap`:** Items `Wrap` to the **Next_Line** if needed.
- **`flex-wrap-reverse`:** It **Reverses** the `Order` in which **Flex_Items** `Wrap` to the **Next_Line**, i.e from `Bottom-To-Top` or `Right-To-Left`.
  <br>

3. **Flex Grow/Shrink (`Flex_Item Property`):** <br>
   It **Controls** how a **Flex_Item** behaves when there is **Extra or Insufficient Space** in a `Flex_Container`. It allows the **Flex_Items** to `grow` or `shrink` to **Fill** or **Adjust** in the available **Space**.

- **`grow`:** Allows the Item to `grow` to fill the **Space**.
- **`grow-0`:** It Prevents the Item from `growing`.
- **`grow-<number>`:** It helps **Flex_Items** to `grow` **Proportionally** based on their `Growth_Factor`.<br>
  **`For Ex:`**
  ```
  <div class="flex gap-5 mx-5 py-10 text-center">
     <div class="size-14 grow-3 bg-purple-500 text-white">01</div>
     <div class="size-14 grow-7 bg-blue-400 text-white">02</div>
     <div class="size-14 grow-3 bg-purple-500 text-white">03</div>
  </div>
  ```
  ![`grow`>>Laptop](https://github.com/user-attachments/assets/69742b0e-79a9-42f8-bc9b-4d74b1f8d775)<br>
  ![`grow`>>Mobile(L)](https://github.com/user-attachments/assets/85ca03b9-db44-4d37-b2b9-a048ef5cac3d)<br>
  As Observed, the **Flex_Items** `grow` and occupy **Space** proportional to their `Growth_Factor`.<br>
- **`shrink`:** Allows the Item to `shrink` if required.
- **`shrink-0`:** It Prevents the Item from `shrinking`.
- **`shrink-<number>`:** It helps **Flex_Items** to `shrink` **Proportionally** based on their `Shrink_Factor`.<br>
  **`For Ex:`**
  ```
  <div class="flex gap-5 mx-5 py-10 justify-center text-center">
     <div class="w-50 h-20 shrink-0 bg-purple-500 text-white">01</div>
     <div class="w-50 h-20 shrink-7 bg-blue-400 text-white">02</div>
     <div class="w-50 h-20 shrink-0 bg-purple-500 text-white">03</div>
  </div>
  ```
  ![`shrink`>>Laptop](https://github.com/user-attachments/assets/d85547a4-87d0-4fa3-856e-4ebd49c350a1)<br>
  ![`shrink`>>Mobile(L)](https://github.com/user-attachments/assets/11c2ddb7-14a2-4b0c-8944-93b760c25671)<br>
  As Observed, the **Flex_Items** `shrink` and occupy **Space** proportional to their `Shrink_Factor`. Also, `Note` that the **Flex_Items** with property `shrink-0` do not `shrink` at all.<br>
  <br>

4. **Flex Basis (`Flex_Item Property`):** <br>
   The `flex-basis` property sets the `Initial_Size` of **Flex_Items** before the remaining **Space** is distributed.

- **`basis-<number>`:** It **Sets the `Initial Size` of Flex_Items** based on the `Tailwind Spacing_Scale`.<br>
  **`For Ex:`**
  ```
  <div class="flex gap-5 mx-5 py-10 text-center">
     <div class="size-14 basis-64 bg-purple-500 text-white">01</div>
     <div class="size-14 basis-64 bg-blue-400 text-white">02</div>
     <div class="size-14 basis-128 bg-purple-500 text-white">03</div>
  </div>
  ```
  ![`basis-<number>`](https://github.com/user-attachments/assets/ac48c790-78b6-4b9d-b859-bcdafcc37ecd)<br>
- **`basis-xs`:** **Extra-Small** Sizing.
- **`basis-sm`:** **Small** Sizing.
- **`basis-md`:** **Medium** Sizing.
- **`basis-lg`:** **Large** Sizing.
- **`basis-xl`: **Extra-Large\*\* Sizing.
- **`basis-2xl` and so on:** **Double Extra-Large** Sizing.<br>
  **`For Ex:`**
  ```
  <div class="flex gap-5 mx-5 py-10 text-center">
     <div class="size-14 basis-xs bg-purple-500 text-white">01</div>
     <div class="size-14 basis-sm bg-blue-400 text-white">02</div>
     <div class="size-14 basis-md bg-purple-500 text-white">03</div>
     <div class="size-14 basis-lg bg-purple-500 text-white">04</div>
  </div>
  ```
  ![`basis-<number>`](https://github.com/user-attachments/assets/1c766f06-8c5f-4aee-be88-0a2541c9a7f0)<br>
  <br>

5. **Justify Content (`Flex_Item Property`)[Horizontal Alignment]:** <br>
   It defines how **Flex_Items** are `Aligned/Spaced Horizontally` inside the `Flex_Container`.

- **`justify-start`:** Align **Items** to the `Left_Side`.
- **`justify-center`:** Align **Items** to the `Center`.
- **`justify-end`:** Align **Items** to the `Right_Side`.
- **`justify-between`:** `Space_Between` the **Items**.<br>
- **`justify-around`:** `Space_Around` the **Items**.<br>
- **`justify-evenly`:** `Equal_Spacing` **between** & **around** the **Items**.<br>

6. **Align Items (`Flex_Item Property`)[Vertical Alignment]:** <br>
   It **aligns** the entire `Grid` (all `rows` or `columns`) `Vertically` inside the `Grid_Container` when there is **Extra_Space**.

- **`items-start`:** Packs **Items** towards the `Top`.
- **`items-center`:** Align **Items** to the `Center`.
- **`items-end`:** Packs **Items** towards the `Bottom`.
- **`items-stretch`:** Stretches the **Items** to **Fill the Space** `Vertically`.
- **`items-baseline`:** Aligns **Flex_Items** along their `Text_Baselines`, typically useful when **Items** have different `Font-sizes` or `Vertical_Padding`.<br>
  **`For Ex:`**
  ```
  <div class="h-[200px] flex gap-5 mx-5 justify-evenly items-end py-10 text-center">
     <div class="bg-purple-500 text-white p-4">01</div>
     <div class="bg-blue-400 text-white p-4">02</div>
     <div class="bg-purple-500 text-white p-4">03</div>
     <div class="bg-blue-400 text-white p-4">04</div>
     <div class="bg-purple-500 text-white p-4">05</div>
     <div class="bg-blue-400 text-white p-4">06</div>
  </div>
  ```
  ![`justify-evenly` & `items-end`](https://github.com/user-attachments/assets/cee2370d-54b2-4f78-927e-f62d3b19168b)<br>
  As Observed, the `justify-evenly` property distributes the `Flex-Items` proportionally ensuring `Equal_Spacing` **around & between** them, meanwhile the `items-end` property aligns the `Flex-Items` towards the `Bottom` of the `Flex_Container`.<br>
  <br>
  <br>
  <br>

### Grid Layout:

`Grid` is a **Powerful `2-dimensional` Layout_System** that allows you to create **Complex** and **Responsive** Layouts using `Rows` and `Columns`.

- **`grid`:** Enables `Grid` **Layout** for an Element.
- **`inline-grid`:** It makes the `Grid_Container` **behave** like an `Inline_Element`.
- **`grid-rows-<number>`:** Defines a given `<number>` of `Explicit Rows` within a `Grid_Container`.
- **`grid-cols-<number>`:** Defines a given `<number>` of `Equal-Width Columns`.<br>
  **`For Ex:`**
  ```
  <div class="grid grid-rows-2 grid-cols-3 gap-5 mx-5 py-10 justify-center text-center">
     <div class="bg-purple-500 text-white p-10">01</div>
     <div class="bg-blue-400 text-white p-10">02</div>
     <div class="bg-purple-500 text-white p-10">03</div>
     <div class="bg-blue-400 text-white p-10">04</div>
     <div class="bg-purple-500 text-white p-10">05</div>
     <div class="bg-blue-400 text-white p-10">06</div>
  </div>
  ```
  ![`grid` Layout](https://github.com/user-attachments/assets/a9675254-b4c6-4e02-b049-9c7f31fb8e17)<br>
  The above `Snippet` clearly demonstrates how `Grid_Layout` works.<br>
  `Note` that the **Grid_Items** automatically `Stretch to Fill the Entire Grid_Cell`, resulting in a **Clean** and **Uniform** Layout without the need for **Specifying** `Width` and `Height`, unlike `Flexbox`.<br>
  <br>

1. **Grid Direction:** <br>
   It **defines** the `Direction` in which **Flex_Items** are placed inside a `Flex_Container`.

- **`grid-flow-row`:** It **places** items `Row-by-Row`.
- **`grid-flow-row-dense`:** **Packs** Items Tightly in `Row` direction.<br>
  **`For Ex:`**
  ```
  <div class="grid grid-rows-3 grid-flow-row grid-cols-3 gap-5 mx-5 py-10 justify-center text-center">
     <div class="bg-purple-500 text-white p-10">01</div>
     <div class="bg-blue-400 text-white p-10">02</div>
     <div class="bg-purple-500 text-white p-10">03</div>
     <div class="bg-blue-400 text-white p-10">04</div>
     <div class="bg-purple-500 text-white p-10">05</div>
     <div class="bg-blue-400 text-white p-10">06</div>
  </div>
  ```
  ![`grid-flow-row`](https://github.com/user-attachments/assets/efcb09a9-f7b9-4caf-8872-d3c81682d62d)<br>
- **`grid-flow-col`:** It **places** items `Column-by-Column`.
- **`grid-flow-col-dense`:** **Packs** Items Tightly in `Column` direction.<br>
  **`For Ex:`**
  ```
  <div class="grid grid-rows-3 grid-flow-col grid-cols-3 gap-5 mx-5 py-10 justify-center text-center">
     <div class="bg-purple-500 text-white p-10">01</div>
     <div class="bg-blue-400 text-white p-10">02</div>
     <div class="bg-purple-500 text-white p-10">03</div>
     <div class="bg-blue-400 text-white p-10">04</div>
     <div class="bg-purple-500 text-white p-10">05</div>
     <div class="bg-blue-400 text-white p-10">06</div>
  </div>
  ```
  ![`grid-flow-col`](https://github.com/user-attachments/assets/7172bc99-f6ec-457d-bbbc-1e01dd5e992d)<br>  
  <br>

2. **Grid_Item Span (`Grid_Item Property`):** <br>
   It lets you **Control** how many `columns` or `rows` a **Grid_Item** should cover, giving you `precise control` over the **Layout**.

- **`row-span-<number-of-rows>`:** Specifies how many `rows` a **Grid_Item** should **Span** across.<br>
  **`For Ex:`**
  ```
  <div class="grid grid-rows-3 grid-flow-col grid-cols-3 gap-5 mx-5 py-10 justify-center text-center">
     <div class="row-span-2 bg-purple-500 text-white p-10">01</div>
      <div class="bg-blue-400 text-white p-10">02</div>
      <div class="bg-purple-500 text-white p-10">03</div>
      <div class="row-span-2 bg-blue-400 text-white p-10">04</div>
      <div class="row-span-2 bg-purple-500 text-white p-10">05</div>
      <div class="bg-blue-400 text-white p-10">06</div>
  </div>
  ```
  ![`row-span-<number>`](https://github.com/user-attachments/assets/c4e6bd3f-0997-4a68-b491-7036114adb8d)<br>
- **`col-span-<number-of-rows>`:** Specifies how many `columns` a **Grid_Item** should **Span** across.<br>
  **`For Ex:`**
  ```
  <div class="grid grid-rows-3 grid-flow-row grid-cols-3 gap-5 mx-5 py-10 justify-center text-center">
     <div class="col-span-2 bg-purple-500 text-white p-10">01</div>
      <div class="bg-blue-400 text-white p-10">02</div>
      <div class="bg-purple-500 text-white p-10">03</div>
      <div class="col-span-2 bg-blue-400 text-white p-10">04</div>
      <div class="col-span-2 bg-purple-500 text-white p-10">05</div>
      <div class="bg-blue-400 text-white p-10">06</div>
  </div>
  ```
  ![`col-span-number`](https://github.com/user-attachments/assets/761a62de-6fc6-4287-982b-bd59abc532e2)<br>
  <br>

3. **Justify Items (`Grid_Item Property`)[Horizontal Alignment]:** <br>
   It **aligns** items `Horizontally` (along the `Row_Axis`) inside their own `Grid_Cells`.

- **`justify-items-start`:** Align Items to the `Left_Side` within a `Grid_Cell`.
- **`justify-items-center`:** Align Items to the `Center` of a `Grid_Cell`.
- **`justify-items-end`:** Align Items to the `Right_Side` within a `Grid_Cell`.
- **`justify-items-stretch`(Default):** `Stretch` the Items to **Fill** the `Grid_Cell`. It is the `Default` **Item_Alignment** followed in a `Grid_Layout`.<br>
  The `justify-self-<alignment>` property is used to **Align** an **individual** `Grid_Item` or the **whole** `Grid_Container` in `Horizontal` Alignment.<br>
  It can be used for **Overriding** the `Global justify-items` **Setting** for Specific Items.
- **`justify-self-auto`:** **Inherits** `Alignment` from the Container.
- **`justify-self-start`:** Align Items/Container to the `Left_Side`.
- **`justify-self-center`:** Align Items/Container to the `Center`.
- **`justify-self-end`:** Align Items/Container to the `Left_Side`.
- **`justify-self-stretch`:** `Stretch` the Items/Container to **Fill** the available **Space**.<br>
  **`For Ex:`**
  ```
  <div class="grid grid-cols-3 justify-itemms-stretch gap-5 mx-5 py-10 text-center">
     <div class="bg-purple-500 text-white p-4">01</div>
     <div class="justify-self-center bg-blue-400 text-white p-4">02</div>
     <div class="bg-purple-500 text-white p-4">03</div>
     <div class="bg-blue-400 text-white p-4">04</div>
     <div class="bg-purple-500 text-white p-4">05</div>
     <div class="bg-blue-400 text-white p-4">06</div>
  </div>
  ```
  ![`justify-items-<alignment>`](https://github.com/user-attachments/assets/2a944fd9-99ac-49ef-8fee-36daaae2ff9f)<br>
  <br>

4. **Align Content (`Grid_Item Property`)[Vertical Alignment]:** <br>
   It **aligns** the entire `Grid` (all `rows` or `columns`) `Vertically` inside the `Grid_Container` when there is **Extra_Space**.

- **`content-start`:** Packs `rows` towards the `Top`.
- **`content-center`:** Aligns `rows` to the `Center` of the `Grid_Container`.
- **`content-end`:** Packs `rows` towards the `Bottom`.
- **`content-between`:** Distribute the `rows` (towards `Top` as well as `Bottom`) with `Space_Between`.
- **`content-around`:** Ensures `Even_Spacing` around each `row`.
- **`content-evenly`:** `Equal_Spacing` **between** & **around** the `rows`.<br>
  **`For Ex:`**
  ```
  <div class="w-200 h-80 grid grid-cols-3 gap-5 justify-self-end content-between mx-5 py-10 text-center">
     <div class="bg-purple-500 text-white p-4">01</div>
     <div class="bg-blue-400 text-white p-4">02</div>
     <div class="bg-purple-500 text-white p-4">03</div>
     <div class="bg-blue-400 text-white p-4">04</div>
     <div class="bg-purple-500 text-white p-4">05</div>
     <div class="bg-blue-400 text-white p-4">06</div>
  </div>
  ```
  ![`content-between`](https://github.com/user-attachments/assets/6d69292d-0e6b-498e-80ed-38ff10b4d4f8)<br>
  As Observed, the `justify-self-end` property shifts the `Grid_Container (Width=200)` towards the `Right_Side`, and the `content-between` property distributes the `rows` towards `Top` and `Bottom` with `Space_Between`.<br>
  <br>
  <br>
  <br>

### Gap Classes:

The `gap` **Utilities** are used to **Control Spacing** between **Items** in `Flexbox` and `Grid` **Layouts**.

- **`gap-0`:** **No Space** between Items.
- **`gap-2`, `gap-4`, `gap-8` and so on:** Inserts **Spacing** between Items based on `Tailwind Spacing_Scale`.
- **`gap-x-5`:** Controls `Horizontal-Spacing` or `Gap between Columns`.
- **`gap-y-5`:** Controls `Vertical-Spacing` or `Gap between Rows`.
  <br>
  <br>

### Item Order:

The `order` **Utilities** let you **Rearrange** the `Visual_Order` of **Items** inside a `flex` or `grid` **Container**, **without changing** the Actual `<HTML>` Structure.

- **`order-none`:** All items strictly follow the `Default Order` or the `DOM_Structure`.
- **`order-first`:** The Item is always ranked as `First` and **Placed Before All Other Elements**.
- **`order-last`:** The Item is always ranked as `Last` and **Placed After All Other Elements**.
- **`order-<number>`:** Sets a `Custom Order_Value` for the **Items**. The Higher the `<number>` Value, the more **priority** an **Item** gets while `Ordering`.<br>
  **`For Ex:`**
  ```
  <div class="grid grid-cols-4 gap-5 mx-5 py-10 text-center">
     <div class="order-last bg-purple-500 text-white p-4">Block-A</div>
     <div class="order-2 bg-blue-400 text-white p-4">Block-B</div>
     <div class="order-1 bg-blue-400 text-white p-4">Block-C</div>
     <div class="order-first bg-purple-500 text-white p-4">Block-D</div>
  </div>
  ```
  ![`order`](https://github.com/user-attachments/assets/29de4d5e-b21b-4f76-9faf-dc3f9afe757a)<br>
  As Observed, the `Block-D` and `Block-A` are ranked `last (i.e, 4th)` and `first (i.e, 1st)` respectively, meanwhile the `Block-C` and `Block-B` are ranked as `1 (i.e, 2nd)` and `2 (i.e, 3rd)` respectively after `Block-D` ehich has the Highest_Order Priority/Ranking.
  <br>

---

<br>

## Responsive Layout_Build

`Tailwind_CSS` supports `Responsive Designs` that automatically **adapt** to **different** `Screen_Sizes`, from **Mobile Phones** to **Large Desktops**.<br>
It follows a `Mobile-First Approach`, where **Styles** apply to the `Smallest Screen (Mobiles)` **First** by default, and are **Overridden** on `Larger Screens (Desktops)` using various `Breakpoint-Prefixes`.<br>
<br>

### Responsive Breakpoints:

The `Responsive Breakpoints` / `Screen-Width Breakpoints` define the **Screen-Widths** at which your `Layout` or `Styles` **should change** to accommodate different device sizes.

- **`sm:`:** It represents `Small_Screens` (i.e, `Mobiles`). [ **`Min-Screen_Width = 640px`** i.e, for Screens with **Width Equal to 640px or Greater** ]
- **`md:`:** It represents `Medium_Screens` (i.e, `Tablets`). [ **`Min-Screen_Width = 768px`** i.e, for Screens with **Width Equal to 768px or Greater** ]
- **`lg:`:** It represents `Large_Screens` (i.e, `Laptops`). [ **`Min-Screen_Width = 1024px`** i.e, for Screens with **Width Equal to 1024px or Greater** ]
- **`xl:`:** It represents `Extra-Large_Screens` (i.e, `Desktops`). [ **`Min-Screen_Width = 1280px`** i.e, for Screens with **Width Equal to 1280px or Greater** ]
- **`2xl:`:** It represents `Doubly Extra-Large_Screens` (i.e, `Smart_TVs`). [ **`Min-Screen_Width = 1536px`** i.e, for Screens with **Width Equal to 1536px or Greater** ] <br>
  **and so on . . .** <br>

  **`For Ex:`** <br>
  For `lg:` i.e, **Screen-Width Equal to 1024px or Greater**:<br>
  ![`lg:`](https://github.com/user-attachments/assets/06f72a75-a33d-4034-9689-d775e389a3f1)<br>
  <br>

  For `md:` i.e, **Screen-Width Equal to 768px or Greater** & **Screen-Width Falls Below 1024px**: <br>
  ![`md:`](https://github.com/user-attachments/assets/d5d7cc4a-c58e-4d68-81f9-2e5c52866664)<br>
  <br>

  For `Default (Mobile-First Orientation)` i.e, **Screen-Width Falls Below 768px**: <br>
  ![`screen-width < 768px`](https://github.com/user-attachments/assets/aeb26124-d159-4f0f-bf78-76a8dabca2fb)<br>
  <br>
  <br>

---
<br>

## Tailwind's Variants:
- A `variant:` **Prefix** is added before a `Utility_Class` to apply that **Style** in a **Specific State**, **Screen_Size** (`sm:`, `md:`, `lg:`, `xl:`) or **Context**.<br>
- It allows developers to **apply Styles Conditionally**.
<br>

### State_Based Variants:
The `State_Based Variants` are **Prefixes** that apply **Styles** when an Element is in a **Specific Interactive or Form-related State**.
- **`hover:`:** Triggers Transformation when the **Element is Hovered** with a Mouse.
- **`focus:`:** Triggers Transformation when the **Element is Selected (Focused)** with a Mouse.
- **`active:`:** Triggers Transformation when the **Element is Clicked or Tapped** with a Mouse.
- **`visited:`:** Triggers Transformation for a **Link which has already been Visisted**.
- **`disabled:`:** Triggers Transformation for a **Disabled Element** using the `disabled` Utility.
- **`checked:`:** Triggers Transformation when a **Checkbox or Radio_Button is Clicked / Checked**.
- **`focus-within:`:** Triggers Transformation When any **Child within the Element is Selected (Focused)**.
<br>
<br>

### Group Variants:
The `group` utility lets you apply **Styles** to **Child_Elements** based on the State (`hover`, `focus`, etc.) of a **Parent_Container**.
- **`group-hover:`:** Triggers Transformation for **Children** when the **Parent_Element is Hovered** with a Mouse.
- **`group-focus:`:** Triggers Transformation for **Children** when the **Parent_Element is Selected (Focused)** with a Mouse.
- **`group-active:`:** Triggers Transformation for **Children** when the **Parent_Element is Clicked or Tapped** with a Mouse.
- **`group-disabled:`:** Triggers Transformation for the **Children** of a **Disabled Parent_Element**.
- **`group-aria-expanded:`:** Triggers Transformation for the **Children** when a **Parent_Dropdown is Expanded**.
<br>
<br>

### Peer Variants:
The `peer` utility allows you to **Style** an Element based on the **State of a Sibling Input or Checkbox**.
- **`peer`:** It allows an Element to act as a **State Reference** for other **Sibling_Elements**.
- **`peer-hover:`:** Triggers Transformation when the **Peer_Element is Hovered** with a Mouse.
- **`peer-focus:`:** Triggers Transformation when the **Peer_Element is Selected (Focused)** with a Mouse.
- **`peer-disabled:`:** Triggers Transformation for the **Sibling** of a **Disabled Peer_Element**.
- **`peer-checked:`:** Triggers Transformation when a **Peer_Element is Clicked / Checked**.
- **`peer-placeholder-shown:`:** Triggers Transformation when the **Placeholder for a Peer_Input is Visible**.
- **`peer-aria-expanded:`:** Triggers Transformation for the Siblings when **Peer_Dropdown is Expanded**.
<br>

---
<br>

## Tailwind's Dark Mode Support:

- The `dark:` prefix is a `Variant` in **Tailwind** that allows you to **apply/modify different styles** when `Dark_Mode` is Active.<br>
- **`Scenario:`** Turning **Light** Background `Darker` and simultaneously modifying `Darker` Text/Content to a **Lighter** format.
- `<HTML>` Implementation:
  ```
  <section class="w-[100vw] h-[100vh] flex items-center justify-center dark:bg-gray-950">
      <div
        class="px-20 py-10 bg-amber-200 text-gray-700 dark:bg-blue-950 dark:text-white rounded-xl"
      >
        <h1 class="text-5xl text-center">Hello, Dark Mode!</h1>
      </div>
  </section>
  ```
- **`Light_Mode:`**<br>
  ![`Light_Mode`](https://github.com/user-attachments/assets/2c2e22d6-d6b6-4d21-a4f5-49fed1ff6577)<br>
- **`Dark_Mode:`**<br>
  First, Switch to `Dark_Mode` **Theme** in your Browser:<br>
  ![`Browser Theme_Settings`](https://github.com/user-attachments/assets/f2146cc1-34ba-4d24-96dc-2aa84f439d1b)<br>
  Observe, how Tailwind Supports the above `Scenario` using `dark:` Variants,<br>
  ![`Dark_Mode`](https://github.com/user-attachments/assets/4669fc71-61e5-420e-8dd4-656602955b08)<br>
<br>
<br>

---
<br>
<div align="center">
   
   ### ADVANCED - LEVEL
</div>
<br>
 
---
<br>

## Transform Utilities
The `Transform` Utilities are **declarative classes** that let you **Animate** or **Change the Appearance** of Elements without writing Custom CSS.<br>
They are generally used with `Variants` such as `hover:`, `focus:`, etc for **Adding Subtle Visual_Effects** to the Elements.<br>
<br>
<br>

### Scale:
The `scale` utility **Resizes an Element Visually**, either **Enlarging (Zoom In)** or **Shrinking (Zoom Out)**, without affecting the `Layout` around the Element.<br>
- **`scale-{amount}`:** Scales both **Width and Height** equally i.e, **Resizes the Element along both Axes** simultaneously.
- **`scale-x-{amount}`:** Scales only **Width** of an Element i.e, **Resizes the Element along X-Axis**.
- **`scale-y-{amount}`:** Scales only **Height** of an Element i.e, **Resizes the Element along Y-Axis**.
<br>
<br>

### Rotate:
The `rotate` utility **Rotates an Element Clockwise or Counter-Clockwise** by a specific degree, without affecting the `Layout` around the Element.<br>
- **`rotate-{degree}`:** Rotates/Spins an Element in **Clockwise direction along Z-Axis**.
- **`-rotate-{degree}`:** Rotates/Spins an Element in **Anti-Clockwise direction along Z-Axis**.
- **`rotate-x-{degree}`:** Rotates/Spins an Element in **Clockwise direction along X-Axis**.
- **`-rotate-x-{degree}`:** Rotates/Spins an Element in **Anti-Clockwise direction along X-Axis**.
- **`rotate-y-{degree}`:** Rotates/Spins an Element in **Clockwise direction along Y-Axis**.
- **`-rotate-y-{degree}`:** Rotates/Spins an Element in **Anti-Clockwise direction along Y-Axis**.
<br>
<br>

### Translate:
The `translate` utility **Shifts (Moves) an Element Horizontally or Vertically** without changing its Position in the `Document_Flow (i.e, DOM)`.<br>
- **`translate-{amount}`:** Moves the Element towards **Right-Hand as well as Downward Direction**.
- **`-translate-{amount}`:** Moves the Element towards **Left-Hand as well as Upward Direction**.
- **`translate-x-{amount}`:** Moves the Element towards **Right-Hand Direction** (i.e, along `Positive X-Axis`).
- **`-translate-x-{amount}`:** Moves the Element towards **Left-Hand Direction** (i.e, along `Negative X-Axis`).
- **`translate-y-{amount}`:** Moves the Element in **Downward Direction** (i.e, along `Negative Y-Axis`).
- **`-translate-y-{amount}`:** Moves the Element in **Upward Direction** (i.e, along `Positive Y-Axis`).
<br>
<br>

### Skew:
The `skew` utility **applies a Diagonal Slant** to an Element, without affecting the `Layout` around the Element.<br>
- **`skew-{amount}`:** Slants the Element towards **Right as well as Downward Direction**.
- **`-skew-{amount}`:** Slants the Element towards **Left as well as Upward Direction**.
- **`skew-x-{amount}`:** Slants the Element towards **Right** (i.e, along `Positive X-Axis`).
- **`-skew-x-{amount}`:** Slants the Element towards **Left** (i.e, along `Negative X-Axis`).
- **`skew-y-{amount}`:** Slants the Element in **Downward Direction** (i.e, along `Negative Y-Axis`).
- **`-skew-y-{amount}`:** Slants the Element in **Upward Direction** (i.e, along `Positive Y-Axis`).
<br>
<br>

### Origin:
The `origin` utility defines the **Pivot Point** for Transformations like `scale`, `rotate`, `skew`, etc.<br>
**`Pivot Point:`** The `Pivot` is the `Central-Axis of Motion` for an Object. Think of it as a `Nail` or `Pin` that you place somewhere on an **Object**, which when you `rotate` or `scale`, moves around that `Pin`.<br>
- **`origin-{position}`:** Relocates the `Axis of Motion` to the **Specified Position**.<br>
  `Note:` Replce the `{position}` with the desired **Position** such as `center`, `left`, `right`, `top`, `bottom`, `top-left`, `bottom-right` and so on. . .<br>
<br>
<br>

### Transform Style:
This **Utility** determines how `Child_Elements` are **rendered** in `3D_Space` i.e, whether they should maintain their **individual 3D Positions** or be **flattened** into the plane of the parent. <br>
- **`transform-flat`:** Children **do not preserve** `3D_Space` and **appear** in a `2D_Plane`, as if **Flattened**.<br>
- **`transform-3d`:** Children **maintain** their `3D Positioning`, allowing for proper **3D Rendering** and **Nested Transforms**.<br>
<br>
<br>

### Backface_Visibility [3D-Transform Utility]: 
The `backface` utility determines **whether the `Back Side` of an Element is Visible** when it is **Rotated** in `3D_Space`. <br>
- **`backface-hidden`:** The **Backside is not Shown**, it remains invisible even when an Element is Flipped.
- **`backface-visible`:** The **Backside is Visible** even when the Element is Rotated.
<br>
<br>

### Perspective [3D-Transform Utility]:
The `perspective` utility defines the **Distance Between the Viewer and the Element** in `3D_Space`.
- **`perspective-none`:** **Disables all 3D Perspective** (Flat Look). Useful when you want **No 3D Distortion**.
- **`perspective-dramatic`:** **Very_Close Perspective**, Creates Strong & Exaggerated 3D Rotation.
- **`perspective-near`:** 	Provides a **Close-Up View**, Noticeable but not too Overwhelming.
- **`perspective-normal`:** It gives a **Balanced 3D_Effect**, ideal for most UI_Cards or 3D_Hover Interactions.
- **`perspective-midrange`:** It makes 3D_movement Smoother and more Realistic.
- **`perspective-distant`:** Gives a **Far-Away Effect**, barely any Distortion, great for Subtle_Depth.
<br>
<br>

### Perspective_Origin [3D-Transform Utility]:
The `perspective-origin` defines the **Point_of_View** from which you see a `3D_Transformed` Element.
- **`perspective-origin-{position}`:** Relocates the `3D Point_of_View` to the **Specified Position**.<br>
  `Note:` Replce the `{position}` with the desired **Position** such as `center`, `left`, `right`, `top`, `bottom`, `top-left`, `bottom-right` and so on. . .<br>
<br>
<br>

---
<br>

## Transition and Animation Utilities
`Tailwind_CSS` provides a rich set of `Transition` and `Animation` **Utilities** to help you create **Smooth Visual_Effects** with minimal effort.
<br>
<br>

### transition-{property}:
The `transition-{property}` utility determines which `CSS Properties` will **Animate**  in a **Clean & Consistent Way** when their **Values** Change.
- **`transition-all` or `transition`:** Applies **Transitions** to `All Animatable CSS_Properties`.
- **`transition-colors`:** Applies **Transitions** only to `Color-related Properties` like `bg-color`, `border-color`, `text-color`, etc.
- **`transition-opacity`:** Limits **Transitions** to the `Opacity Property`.
- **`transition-shadow`:** Applies **Transitions** only to the `Shadow Properties` such as `Box_Shadow (shadow)`, `text-shadow`, etc.
- **`transition-transform`:** Enables **Transitions** on `Transformation-related Properties` like `scale`, `rotate`, `translate`, `skew`, etc.
<br>
<br>

### duration:
The `duration` utility controls **how long** a `Transition` or `Animation` takes to **Complete**.
- **`duration-{time}`:** It Sets the `Time` taken by a transition to Complete, in `milliseconds (ms)`.
- **`duration-0`:** No Animation delay (**No Animations** & **Instant Change**).
- **`duration-200`:** Ideal Animation Delay for most **UI Hover_Effects**. 
- **`duration-300`:** Ensures **Smooth, Polished Transitions**.
- **`duration-1000` (1 sec):** Used for **Dramatic Transitions** or StoryTelling.
<br>
<br>

### ease-{type} [Timing-Function]:
The `ease` utility controls the `Acceleration Curve` of a **Transition** or **Animation**.<br>
It determines how **fast** or **slow** the **Animation** moves at different **Stages (such as start, end, etc.)**.<br>
- **`ease-linear`:** Transition is performed at a **Constant Speed** from Start to End.
- **`ease-in`:** The Transition **Starts Slow**, then **Speeds Up towards the End**.
- **`ease-out`:** The Transition **Starts Fast**, then **Slows Down towards the End**.
- **`ease-in-out`:** The Transition **Starts & Ends Slowly**, and only **Transitions Faster in the Period Between**.<br>
<br>

The Above `Timing-Functions` can be Explained uing the following `Cubic-Bezier Curves`:<br>
<div>
   <img src="https://github.com/user-attachments/assets/641e022f-07e2-4e17-ac66-574566520fe4" alt="Tailwind Logo" width="29.9%">
   <img src="https://github.com/user-attachments/assets/2884e645-39fa-47c1-8221-f597cec4729d" alt="Tailwind Logo" width="30.2%">
   <img src="https://github.com/user-attachments/assets/e6dbc65f-8ae7-4673-9738-4ea17cfef3c4" alt="Tailwind Logo" width="30%">
   <img src="https://github.com/user-attachments/assets/2697941a-d94d-4b7a-87ca-acc593123ef3" alt="Tailwind Logo" width="29.9%">
</div>
<br>
<br>

### delay:
The `delay` utility defines **how long to Wait** before Initiating a `Transition` or `Animation`.<br>
- **`delay-{time}`:** It Defines the `Waiting_Time` after which a Transition Begins, in `milliseconds (ms)`.
- **`delay-0`:** **No Delay** for Transitions i.e, the Transition Animations begin instantaneously.
- **`delay-75`:** Slight Pause for **Subtle Effects**.
- **`delay-100`:** Slight Pause commonly used for **Cascading UI**.
- **`delay-150`:** Noticeable Pause for **Staggered Effects**.
<br>
<br>

### Animations:
The `animate` utility lets you apply `Motion Effects` to `<HTML>` Elements. <br>
- **`animate-none`:** **No Animations** are applied to an Element. 
- **`animate-spin`:** **Spins** the Element continuously.
- **`animate-ping`:** Makes an Element **Scale and Fade-Out** like a `Radar_Ping` or `Ripple_of_Water`.
- **`animate-pulse`:** Smooth & Gentle **Fade In & Out Animation Loop** on an Element. 
- **`animate-bounce`:** Makes an Element **Bounce Up and Down** continuously.
<br>
<br>

---
<br>

## Customizing Tailwind with "tailwind.config.js"

`Tailwind_CSS` is **Highly Customizable**.<br>
You can tailor it to fit your **System_Design** by **Configuring** your own `colors`, `spacing`, `fonts`, `screens (breakpoints)`, `utilities`, and so on . . ., using the `tailwind.config.js` File.<br>

**`Note:`** You need `Tailwind_v3.4.17` or **earlier** to use `tailwind.config.js` for Customizations.<br>
As of `Tailwind_v4+`, this method is considered **deprecated** in favor of a [`CSS-first Configuration`](#) approach.
<br>

### tailwind.config.js Structure (Syntax):
- `Basic Structure` of `tailwind.config.js` **File** can be given as follows:<br>
  ```
  // tailwind.config.js

  /** @type {import('tailwindcss').Config} */
  module.exports = {
     content: [],       // 1. Content_Files (i.e, where Utility_Classes have been implemented) to be Scanned (Ex: './index.html')
     theme: {
        extend: {},      // 2. Theme Customizations Here (colors, fonts, etc.)
     },
     plugins: [],       // 3. Additional Plugin_Support 
  }
  ```
- Its `Core_Sections` are as follows:
  - [`content`](#content-block)
  - [`theme`](#theme-block) [`Note:` This is just one of the types of the `Extends-Block` but is **most commonly used**. Other Types include: `variants`, `plugins`, `corePlugins`, `plugins`, `content`, etc.]
  - [`plugins`](#plugins-block)
<br>
<br>

### Content Block:
- It is an `Array` which **Lists the Files** where `Tailwind` must look for `Class_Names`.
- It helps to **Purge** `Unused Styles (Classes))` in **Production** by scanning only Specified_Files.
- It supports:
  - **Extensions:**  `.html`, `.js`, `.ts`, `.jsx`, `.tsx`, `.vue`, etc.
  - **Glob Patterns:**  `Glob_Patterns` are like **Smart Symbols within File_Paths**  that help **Match** the `File_Names` or `File_Paths`.<br>
    (**Ex:** `'./**/*.{html, js}'` which means Scan all `.html` and `.js` **Files**(`/*{html, js}`) in the Current_Folder(where `tailwind.config.js` File is Stored)(`./`) & Sub-Folders(`/**`) of the Project.)<br>
- **`For Ex:`** <br>
  Suppose a File Structure:
  ```
  src/
   ├── index.html
   ├── contact.html
   ├── pages/
   │   └── about.html
  ```
  <br>
  
  Then `Content_Block` can be **Configured** as:
  ```
  // Using Absolute Paths:
  content: [
    './src/index.html',
    './src/contact.html',
    './src/pages/about.html',
  ],
  ```
  <div align="center">

     **OR**
  </div>

  ```
  // Using Glob Patterns:
  content: ['./src/**/*.html'],
  ```
  This Pattern will Scan all `.html` Files in the `src` Folder and its Sub-Folders for `Tailwind's Utility_Classes`.<br>
<br>
<br>

### Theme Block:
- The `Theme Block` is the **Heart of Customization** in `Tailwind_CSS`.
- It lets you **define** the `System_Design` used throughout your Project, including `colors`, `fonts`, `spacing`, `breakpoints` and more.
- Some Common Customizations are as follows:
  - `colors`: Lets you **define** the **Custom** `text`, `background`, or `border` **Colors**.
  - `spacing`: Add **Custom** `padding`, `margin`, `gap`, etc. (Spacing_Scale usually follows `rem`)
  - `fontFamily`: Define **Custom** `Font Family`.
  - `breakpoints`: **Customize** the `Responsive Breakpoints`.
  - `borderRadius`: Set **Custom** `Border Roundedness` Sizes.
  - `boxShadow`: Add **Custom** `Shadow Styles`.
  - `fontSize`: Add **Custom** `Font Sizes`.
  - `zIndex`: **Customize** the Element's `Stacking Order`.
  - `maxWidth`: Add **Custom** `Maximum Element_Widths`.
- **`For Ex:`** <br>
  Consider the following **Sample**:
  ```
  // Theme Block
  theme: {
     extend: {
        colors: {
           primary: "#1e40af",
           secondary: "#f59e0b",
        },
        spacing: {
           fullWidth: "100vw",
           fullHeight: "100vh",
        },
        fontFamily: {
           heading: ["Nunito", "sans-serif"],
           subheading: ["Ubuntu", "sans-serif"],
        },
        screens: {
           sm: "480px",
           md: "768px",
           lg: "1024px",
           xl: "1280px",
        },
        borderRadius: {
           huge: "1rem",
           curve: "2rem",
        },
        boxShadow: {
           soft: "0 4px 6px rgba(0, 0, 0, 0.1)",
           strong: "0 8px 10px rgba(0, 0, 0, 0.3)",
           deep: "0 10px 15px rgba(0, 0, 0, 0.4)",
        },
     },
  },
  ```
  <br>

  `<HTML> Implementation` of these **Customizations:**
  ```
  <section class="w-fullWidth h-fullHeight flex items-center justify-center bg-secondary">
     <div class="text-center p-8 rounded-huge bg-white">
        <h1 class="text-secondary text-4xl font-heading mb-4">Custom Theme</h1>

        <p class="text-lg font-subheading mb-6">
          This section showcases how to configure and customize Tailwind CSS
          using <span class="font-semibold text-primary">tailwind.config.js</span>
        </p>

        <button
          class="px-6 py-2 bg-primary text-white font-subheading rounded-curve hover:shadow-deep transition-ease-in-out duration-300">
          Get Started
        </button>
     </div>
  </section>
  ```
  <br>

   Dont Forget to **Add Links for the Font-Families within the `<HEAD>` Tag** or the `Font-Family Customizations` won't work:
  ```
  <head>
     <meta charset="UTF-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <link href="./output.css" rel="stylesheet" />

     <!-- Google_Fonts Links-->
     <link rel="preconnect" href="https://fonts.googleapis.com" />
     <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
     <link
        href="https://fonts.googleapis.com/css2?family=Nunito:ital,wght@0,200..1000;1,200..1000&family=Ubuntu&display=swap"
        rel="stylesheet"
     />
     <link
        href="https://fonts.googleapis.com/css2?family=Ubuntu&display=swap"
        rel="stylesheet"
     />
  </head>
  ```
  ![`Theme_Block` Customizations Output](https://github.com/user-attachments/assets/da2a2952-c989-47ac-8a24-1af518f71491)<br>
<br>
<br>

### Plugins Block:
- The `Plugins Block` is used to **Extend** `Tailwind's Functionality` by adding **Custom Utilities**, **Components** or **Importing Third-party / Community Tailwind_Plugins**.
- Some Common `Plugin_Functions` are as follows:
  - `addUtilities()`: It **Registers New Utility_Styles**, which are typically `Single-Purpose Classes`. 
  - `addComponents()`: It **Registers New Component_Styles**, which are often a `Collections of Utilities/Styles`.
  - `addBase()`: **Add** `Base_Element Styles` i.e, defines Styles for Base_Elements (Ex: `<h1>`, `<button>`, etc.)
  - `addVariant()`: It **Registers** `Custom_Variants`, allowing you to **Create New State-Based Styles**.
  - `theme()`: **Accesses** values from the `Theme_Configuration` i.e, `Theme_Block`.
  - `config()`: **Accesses** values from the `Tailwind_Configuration` i.e, `tailwind.config.js`. 
- `addUtilities()`: <br>
  This Functiom **Registers New Utility_Styles**, which are typically `Single-Purpose Classes`.<br>
  It is used to define **Individual Utility_Classes** with `Single-Purpose CSS_Styles`.<br>
  **`For Ex:`**
  Adding a `text-shadow` Utility_Class,
  ```
  // Plugin Block
  plugins: [
     function ({ addUtilities }) { // It is Shorthand for destructuring extracting only the needed "addUtilities" helper from "Tailwind's Plugin_Context Object i.e, helper" passed to your Plugin_Function.
        const newUtilities = {     // Defines the Custom New "text-shadow" Utilities.
           '.text-shadow': {
              textShadow: '2px 2px 4px rgba(255, 0, 0, 0.3)',
           },
           '.text-shadow-none': {
              textShadow: 'none',
           },
        };
  
        addUtilities(newUtilities, ['responsive', 'hover']);
        // This Registers the New Utility_Classes within the "newUtilities" Variable with Tailwind.
        // The Second Argument ['responsive', 'hover'] tells Tailwind to generate "responsive" and "hover" Variants,
        // Hover Variant >> `hover:text-shadow`
        // Responsive Variant >> `md:text-shadow`
     },
  ],
  ```
- `addComponents()`: <br>
  This Function **Registers New Component_Styles**, which are often a `Collections of Utilities/Styles`.<br>
  Unlike `addUtilities()` Function, it used to define **Reusable `.class` Based Components** that `Group Multiple CSS_Styles` together.<br>
  **`For Ex:`**
  Adding a Custom `btn-glass` Component,
  ```
  // Plugin Block
  plugins: [
     function ({ addComponents, theme }) { // It is Shorthand for destructuring and extracting only the needed "addComponents", "theme" helpers from "Tailwind's Plugin_Context Object i.e, helper" passed to your Plugin_Function. 
        const buttons = {      // Defines the Custom New "btn-primary" Component and its "hover" Variant.
           ".btn-primary": {
              padding: "0.5rem 1rem",
              borderRadius: theme("borderRadius.curve"),
              backgroundColor: theme("colors.primary"),
              color: "#ffffff",
              backdropFilter: "blur(10px)",
              boxShadow: theme("boxShadow.soft"),
              transition: "all 0.3s ease-in-out",
              transform: "scale(1)",
           },
           ".btn-primary:hover": {
              boxShadow: theme("boxShadow.strong"),
              transform: "scale(1.05)",
           },
        };
  
        addComponents(buttons); // This Registers the New Components within the "buttons" Variable with Tailwind.      
     },
  ],
  ```
- `addBase()`: <br>
  The `addBase()` is a method used to **Inject `Base(Global) Styles`**.<br>
  It performs tasks such as **Resetting element's Default_Styles**, **Styling Fonts** or **Modifying `<HTML>` Tags**.<br>
  **`For Ex:`**
  Modifying the `<h1>`, `<p>` and `<span>` Tags for **Heading and Subheading** Effect,
  ```
  // Plugin Block
  plugins: [
     function ({ addBase, theme }) { // It is Shorthand for destructuring and extracting only the needed "addBase", "theme" helpers from "Tailwind's Plugin_Context Object i.e, helper" passed to your Plugin_Function. 
      const base = { // Modifies the 'h1', 'p' and 'span' Base_Elements.
        h1: {
          color: theme("colors.secondary"),
          fontFamily: theme("fontFamily.heading"),
          fontSize: "2rem",
        },
        p: {
          color: "#000000",
          fontFamily: theme("fontFamily.subheading"),
          fontSize: "1.2rem",
        },
        span: {
          color: theme("colors.primary"),
          fontWeight: "bold",
        },
      };

      addBase(base); // This Registers the Modified_Styles for the Base_Elements within the "base" Variable with Tailwind.
    },
  ],
  ```
- `addVariant()`:<br>
  The `addVariant()` is a method used to **define `Custom Class_Variants`**, like `hover:`, `focus:`, or **Custom_Variants** (Ex: `child:`).
  **`For Ex:`**
  Creating a **Custom_Variant** `child-hover` which **tracks and modifies** the **Children** within a **Parent_Element**,
  ```
  // Plugin Block
  plugins: [
     function ({ addVariant }) {  // It is Shorthand for destructuring and extracting only the needed "addVariant" helper from "Tailwind's Plugin_Context Object i.e, helper" passed to your Plugin_Function. 
      addVariant("child-hover", "&:hover > *"); //  This Registers the Custom_Variant with Tailwind.
    },
  ],
  ```
  `Note:` The `addVariant()` Function also utilizes **Glob_Patterns** to identify Elements/Childrens.<br>
  The `&` indicates the `Parent_Element`, `:hover` instructs Tailwind to generate `Hover_Variants`, `> *` identifies all the `Children` within the **Parent_Element**.<br>
  Here the **Glob_Pattern** basically means `Generating Hover(:hover) Variants for all Childrens(> *) under Parent_Element(&)`.<br>
- `theme()`: <br>
  The `theme()` Function is a `helper` provided in **Plugins** (like `addUtilities()`, `addComponents()`, `addBase()`, etc.) to access your `Tailwind_Config Values` declared inside the `Theme_Block`.<br>
  It follows the following `Syntax`:<br>
  ```
  theme("path.to.theme_variable")
  ```
- `config()`: <br>
  The `config()` Function is a `helper` which allows you to **Access** your entire `Tailwind_Config` (unlike `theme()` which only provides access to values under **Theme_Block**).<br>
  It provides access to `Config_Values` such as:
     - `theme`
     - `variant`
     - `corePlugins`
     - `darkMode`, etc.<br>
     <br>
     
  It follows the `Syntax`:<br>
  ```
  config("path.to.config_variable")
  ```
  **`For Ex:`**<br>
  |**config('path')**                                       |**Result / Value**                              |
  |---------------------------------------------------------|------------------------------------------------|
  |`config('theme.colors.primary')`                         |`#1e40af`                                       |
  |`config('variants.backgroundColor')`                     |`['hover', 'focus']`                            |
  |`config('corePlugins.float')`                            |`false`                                         |
  |`config('darkMode')`	                                    |`'class'`                                       |
- Adding `Third-Party Plugins`: <br>
  You can easily **Add** `Third-party Plugins` inside your `tailwind.config.js` using the `plugins` **Array**.
  It mainly involves `Two Steps`:
     - `Download` the required Tailwind Plugins: <br>
       **`Command Prompt:`**
       ```
       npm install @tailwindcss/forms @tailwindcss/typography
       ```
     - **Add** it to the **plugins_Array** using `require()`: <br>
       **`tailwind.config.js:`**
       ```
       plugins: [
          require('@tailwindcss/forms'),
          require('@tailwindcss/typography'),
       ],
       ```
  <br>
  
- Integrated (Combined) `<HTML> Implementation` for above **Plugins**:
  ```
  <section class="w-fullWidth h-fullHeight flex items-center justify-center bg-secondary">
     <div class="text-center p-8 rounded-huge bg-white">
        <h1 class="text-shadow mb-4">Custom Theme</h1>

        <p class="mb-6">
          This section showcases how to configure and customize Tailwind CSS
          using <span>tailwind.config.js</span>
        </p>

        <div
          class="child-hover:scale-105 child-hover:bg-secondary child-hover:transition-all child-hover:duration-300 flex justify-center items-center space-x-5 my-5"
        >
          <div class="p-8 bg-primary rounded-huge"></div>
          <div class="p-8 bg-primary rounded-huge"></div>
          <div class="p-8 bg-primary rounded-huge"></div>
        </div>

        <button class="btn-primary btn-primary:hover">Get Started</button>
     </div>
  </section>
  ```
  ![`Plugins_Block`](https://github.com/user-attachments/assets/cd387fec-e98d-4282-997b-daefa5332090)<br>
<br>
<br>
<br>

## Tailwind_v4 CSS-First Configuration:
The `CSS-first Configuration` is the New **Customization Approach** introduced with `Tailwind_CSS v4+`.<br>
It allows you to **define** your `System_Design` directly in your `CSS_File`, instead of **Configuring** everything in `tailwind.config.js`.
<br>

Some `Benefits` are as follows:
- **`Faster Development:`** You can now set your **Custom_Styles** (like `colors`, `fonts`, `sizes`) directly in a `CSS_File` using `Config_Variables`.<br>
  Improves **maintainability of `CODE`** as the **Customizations** are now maintained under an individual `CSS_File`.<br>
- **`Customization using Native CSS Features:`** **Tailwind** now supports **Modern CSS_Features** like `@theme`, `@layer`, etc., directly in your **Stylesheet** for **Customizations**.
- The **`Content_Block is now handled Automatically`**. You no longer need to manually specify the **Files**, which implement the `Utility_Classes`, inside the `Content Block` within `tailwind.config.js` while using `Tailwind_v4+` (i.e, **CSS-first Configuration**). 
<br>

### CSS-first Configuration Structure:
- `Basic Structure` of the Main `CSS` **File** can be given as follows:<br>
  ```
  @import "tailwindcss";
  @plugin <plugin_name>;
  
  :root {
  }

  @theme {
  }
  
  @layer {
  }
  ```
  <div align="center">
     
     **OR**
  </div>
  
  ```
  @import "tailwindcss";
  @plugin <plugin_name>;

  :root {
  }

  @theme {
  }
  
  @layer base{
  }

  @layer components{
  }

  @layer utilities{
  }
  ```
- Its `Core_Sections` are as follows:
  - [`:root`](#root-block)
  - [`@theme`](#theme)
  - [`@layer`](#layer) 
  - [`@plugin`](#plugin)
<br>
<br>

### :root Block:
- The `:root` is a **CSS_Selector** that targets the **Highest-Level Element** in the `DOM (Document Object Model)`, essentially the `<HTML>` Element.
- It is used to define `CSS Custom_Properties (--variables)` that can be accessed anywhere in the **CSS_File** using the `var()` Method.
- The `:root` selector applies to the **Entire Document** i.e, **Define Once and Use Anywhere** throughout the **CSS_File**. This makes it easier to manage `Custom_Styling` at a `Global_Level`.
- **`For Ex:`**
  ```
  :root {
     --primary: #1e40af;
     --secondary: #f59e0b;
  }
  ```
  These `CSS_Variables` cannot be directly used as `Utility_Classes` but can be passed as **Values** [using `val()` Method] to `Custom Utility_Classes` within `@theme` or `@apply` Blocks.
<br>
<br>

### @theme:
- The `@theme` lets you **define** the `System_Design` used throughout your Project, including `colors`, `fonts`, `spacing`, `breakpoints` and more..
- It lets you **manipulate** and **create** `Custom Utilities` for **Tailwind's Utility_Classes**.
- It also lets you access these `Utilities` as `Custom_Variables` using the `var()` **Method**.
- **`For Ex:`**
  ```
  @theme {
     --color-p: var(--primary);
     --color-s: var(--secondary);
     --color-avocado-100: oklch(0.99 0 0);
     --color-avocado-200: oklch(0.98 0.04 113.22);
     --color-avocado-300: oklch(0.94 0.11 115.03);
  
     --spacing-fullWidth: 100vw;
     --spacing-fullHeight: 100vh;
  
     --radius-curve: 2rem;
     --radius-huge: 1rem;

     --shadow-soft: 0 4px 6px rgba(0, 0, 0, 0.1);
     --shadow-strong: 0 8px 10px rgba(0, 0, 0, 0.3);
     --shadow-deep: 0 10px 15px rgba(0, 0, 0, 0.4);
  
     --breakpoint-sm: 100px;
     --breakpoint-md: 480px;
     --breakpoint-lg: 750px;
     --breakpoint-xl: 1000px;
  
     --font-heading: "Nunito", sans-serif;
     --font-subheading: "Ubuntu", sans-serif;-primary: #1e40af;
  }
  ```
  You can also Observe that, the `Custom CSS_Variables` defined in `:root` are being accessed by **Utilities** defined in `@theme` using the `var()` method.
<br>
<br>

### @layer:
- The `@layer` is a **special directive** used to add your own `Custom CSS` into Tailwind's Build.
- It is used to **Group** `Custom CSS` into one of `Tailwind’s Internal Style_Layers` (`base`, `utilities`, `components`) for proper ordering and purging.
<br>

- **`@layer base`:**<br>
  It is used to define **Default Styles** for `<HTML>` Tags.
  ```
  @layer base {
     body {
       font-family: var(--font-heading);
     }

     h1 {
       font-size: 2.25rem;
       font-weight: 200;
       color: var(--secondary);
     }

     p {   
       font-size: 1.2rem;
       font-family: var(--font-subheading);
     }

     span {
       font-weight: 800;
       color: var(--primary);
     }
  }
  ```
- **`@layer utilities`:**<br>
  It is used to define **Custom Utility_Classes** which are basically `Single-Purpose Utilities` i.e, they define a **Set of CSS_Properties** to achieve a Specific **Styling_Effect**.<br>
  `Note:` Use of `Multiple-Properties` for a `Single_Utility` is **Allowed**, it is **Recommended** to keep each `Utility` focused on a `Single Property` for better **clarity**, **consistency**, and **maintainability**.
  ```
  @layer utilities {
     .text-shadow {
       text-shadow: 0 2px 4px rgba(255, 0, 0, 0.4);
     }

     /* Set of CSS_Properties to achieve a Specific Hover-Effect for Child_Elements */
     .child-hover > *:hover {
       transform: scale(1.05);
       background-color: var(--secondary);
       transition: ease-in-out 0.3s;
     }
  }
  ```
- **`@layer components`:**<br>
  It is used to define **Reusable UI_Components**. These are **Larger**, **Multi-property** Classes that group together `Utility_Styles` into a single, easy-to-use Class_Name.<br>
  It also facilitates the use of `@apply`, allowing you to **Combine** multiple **Tailwind's** `Utility_Classes` into a Single `Custom_Class`. 
  ```
  @layer components {
     .btn-primary {
        @apply px-5 py-2 rounded-curve bg-p text-white shadow-soft duration-300;
     }

     .btn-primary:hover {
        @apply bg-s shadow-strong scale-105;
     }
  }
  ```
<br>
<br>

### @plugin:
- The `@plugin` is used to **Extend** `Tailwind's Functionality` by adding **Custom Utilities**, **Components** or **Importing Third-party / Community Tailwind_Plugins**.
- It is declared at **Start** of the `CSS_File` after `@import "tailwindcss";` Line.
- Similar to [`Plugins Block`](#plugins-block) it supports various functions such as `addUtilities()`, `addComponents()`, `addBase()`, etc for this purpose.
- It also doesn't need the `require()` method to Import Plugins.
- **`For Ex:`**
  ```
  @plugin "new.plugin";
  ```
<br>

  Integrated (Combined) `<HTML> Implementation` for above **CSS-First Customiations**:
  ```
  <section class="w-fullWidth h-fullHeight flex items-center justify-center bg-s">
     <div class="text-center p-8 rounded-huge bg-white shadow-md">
        <h1 class="mb-4 text-shadow">Custom Theme</h1>

        <p class="mb-6">
          This section showcases how to configure and customize Tailwind CSS
          using <span>tailwind.config.js</span>
        </p>

        <div
          class="child-hover:scale-105 child-hover child-hover child-hover flex justify-center items-center space-x-5 my-5"
        >
          <div class="p-8 bg-p rounded-huge duration-300"></div>
          <div class="p-8 bg-p rounded-huge duration-300"></div>
          <div class="p-8 bg-p rounded-huge duration-300"></div>
        </div>

        <button class="btn-primary btn-primary:hover">Get Started</button>
     </div>
  </section>
  ```
  ![`CSS-First Config`](https://github.com/user-attachments/assets/8af3a37b-2cf8-4132-a5d2-4f8ed80f922b)<br>
<br>
<br>

---

