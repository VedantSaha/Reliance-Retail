# 🏷️ Reliance Retail Sticker Generator

The **Reliance Retail Sticker Generator** is a web-based application developed using **React** and **TypeScript** that allows users to dynamically generate **custom product stickers in PDF format**.  
This project was designed to **simplify and automate the product labeling process** in retail environments, ensuring consistency, speed, and ease of use without requiring any manual design tools.

---

## 🧠 Project Overview

In retail operations, generating price and product stickers is often a repetitive and time-consuming task.  
This app was created to provide a **fully automated and customizable solution** that can generate **print-ready sticker sheets** based on user input.

Users can enter product details — such as product name, MRP, and number of copies — and the application instantly creates a **formatted sticker layout**, compiles it into a PDF, and prepares it for printing.

The system automatically handles:
- Layout management (14 stickers per page)
- Multi-page creation if total stickers exceed one page
- Integration of the product list table in the same PDF
- PDF download without leaving or refreshing the page

This enables employees or store managers to create hundreds of product stickers efficiently within minutes.

---

## 🎯 Objectives

- To **automate** the product labeling process for retail use.
- To **reduce manual effort** and eliminate errors in repetitive sticker generation.
- To **generate consistent, professional-grade PDF outputs** using browser-based technologies.
- To **enable dynamic sticker customization** without hardcoding any product details.

---

## ⚙️ Key Functionalities

1. **Dynamic Data Input**
   - Accepts multiple product entries from the user interface.
   - Each entry includes product name, MRP, and number of copies.
   - Automatically calculates the total number of stickers needed.

2. **Automatic Sticker Layout**
   - Arranges 14 stickers per page in a clean grid format.
   - Generates additional pages automatically when more stickers are required.

3. **PDF Generation**
   - Uses `html2canvas` to capture sticker elements as images.
   - Combines these images using `jsPDF` into a downloadable, print-ready PDF.
   - Includes the product table (with user inputs) in the same document for reference.

4. **Instant Export**
   - Generates the PDF directly on the same page — no navigation or backend server required.
   - Ensures real-time feedback and minimal delay.

5. **Fully Dynamic System**
   - All sticker content (product name, MRP, etc.) is generated based on user input.
   - No constants or hardcoded values are used — making it scalable and reusable for any retail product line.

---

## 🛠️ Technology Stack

| Technology | Role |
|-------------|------|
| **React + TypeScript (TSX)** | Component-based UI and logic implementation |
| **html2canvas** | Converts on-screen elements into images for PDF creation |
| **jsPDF** | Generates downloadable PDFs from captured elements |
| **Tailwind CSS** | Handles styling and responsive layout |
| **Vite** | Fast bundler and development environment |

---

## 🧩 Workflow Summary

1. **User Input Phase** – The user enters all required product details in a form.  
2. **Data Processing Phase** – The app calculates total stickers, organizes the layout, and prepares preview containers.  
3. **Rendering Phase** – `html2canvas` captures each sticker area as an image snapshot.  
4. **PDF Compilation Phase** – `jsPDF` compiles all snapshots and the table into a single PDF document.  
5. **Output Phase** – The PDF is immediately downloaded or previewed by the user.

---

## 💡 Example Use Case

Suppose a store manager at Reliance Retail needs to generate stickers for 10 different products, each with varying quantities.  
Instead of manually creating and printing each label, the manager simply:
1. Inputs product names, MRPs, and quantities in the web app.
2. Clicks **Generate PDF**.
3. Instantly receives a multi-page PDF file containing all the stickers and the product table — ready to print.

This eliminates repetitive formatting, manual calculations, and human errors, while maintaining professional visual consistency.

---

## 📋 Potential Enhancements

- Add **company logo or branding** automatically to each sticker.
- Support **CSV or Excel upload** for bulk product import.
- Integrate **barcode or QR code generation** for inventory tracking.
- Provide **preview mode** before generating the final PDF.
- Include **print settings customization** (margins, sticker size, layout).
- Offer **dark mode** or brand-specific color themes.

---

## 🧠 Learning Outcomes

- Hands-on experience with **React + TypeScript** for dynamic web applications.  
- Integration of **html2canvas** and **jsPDF** for front-end PDF generation.  
- Understanding **layout management and DOM rendering** for precise PDF output.  
- Implementation of **state-based UI logic** for handling multiple user inputs dynamically.  
- Experience in **optimizing client-side performance** for graphics-heavy operations.

---
