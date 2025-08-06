```
I want to build a **Smart Tambola Web App** using **Next.js**, **Tailwind CSS**, and **ShadCN UI utilities**.

### ⚙️ Development Guidelines:

- Do **not** apply any custom colors or theming. I will use **TweakCN** later to style the UI.
    
- Use **ShadCN components** where applicable.
    
- The design should be **responsive**, support **dark mode**, and include **smooth animations** using **Framer Motion** or other relevant libraries.
    
- Maintain a **clear separation of frontend and backend**. I will use two separate prompts to generate each. This prompt is for the **frontend** only.
    

---

### 🎫 1. Tambola Ticket Generator:

- Generate valid **Tambola (Housie)** tickets with the following structure:
    
    - Each ticket is a **9x3 grid** (9 columns, 3 rows).
        
    - Each **row must have exactly 5 numbers** and **4 blank spaces**.
        
    - Columns have specific number ranges:
        
        - Column 1 → 1–10
            
        - Column 2 → 11–20
            
        - Column 3 → 21–30
            
        - …
            
        - Column 9 → 81–90
            
    - No number should repeat in the ticket.
        
    - Allow **generation of multiple tickets at once** (e.g., 6 tickets on one screen).
        
    - Use animation when revealing a ticket.
        

---

### 🔢 2. Random Number Picker:

- Randomly draw numbers between **1 and 90** with **no repetition**.
    
- Visually **display the current number** using an animated pop-up.
    
- Maintain and show a **history log** of all previously drawn numbers.
    
- Use **voice announcements** for picked numbers (e.g., "Fifty-five") using browser-based speech synthesis APIs.
    

---

### 💫 3. Animated, Interactive UI:

- Include animations for:
    
    - Ticket reveal
        
    - Number drawing
        
    - Win celebration (e.g., confetti or flashing highlight)
        
- The UI should be clean, modern, and **entirely theme-agnostic** (no hardcoded colors).
    

---

### 🧠 Data Modeling (Schemas):

Provide frontend-compatible TypeScript interfaces or schemas for:

- A Tambola Ticket
    
- Ticket Grid Cell (number or blank)
    
- Number Picker History
    
- Ticket Batch (if generating 6 at once)
    

---

**NOTE:**  
This prompt is only for the **frontend**
```