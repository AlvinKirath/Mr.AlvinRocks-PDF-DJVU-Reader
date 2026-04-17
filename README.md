### **🚀 The V3 "Precision Engine" (Performance Updates)**
* **Dirty Rect Rendering**: The rendering engine now uses a "Smart Dirty Rect" system. Instead of refreshing the whole canvas, it only repaints the tiny zone where your pen moves, eliminating drawing lag even on massive 4K documents.
* **Aggressive RAM Hard-Lock**: Added a 128MB hard-cap on Qt’s internal image cache and implemented `fitz.TOOLS.store_shrink` calls on every page turn. This slashes RAM usage and prevents the "memory creep" crashes common in traditional readers.
* **O(1) Jump Navigation**: Page jumping now uses direct mathematical coordinate mapping instead of iterative loops, enabling instantaneous navigation through 2,000+ page files.
* **Startup Diagnostics**: A new pre-flight dependency check ensures you have `PyMuPDF` and `PySide6` installed, providing clear native Windows error messages if anything is missing.

### **✨ New Feature Highlights**
* **Polygon Lasso Tool**: Move beyond rectangles. Use the freehand lasso (Right-Click) to select complex groups of ink strokes or extract irregular image regions at 3x resolution.
* **Native Quality Image Slicing**: Implemented a "NATIVE QUALITY FIX" for pasting. The app now slices original high-res pixel buffers into your notes, ensuring text stays razor-sharp even when zoomed in 400%.
* **Integrated Text Tool**: You can now insert and position high-res text notes directly onto any document or blank canvas.
* **Session Restoration**: A one-click "Restore Session" button on the Home Tab instantly re-opens all your previous tabs, restoring your exact page, zoom, and rotation state.
* **Silent Background Loading**: You can now right-click documents on the Home Dashboard to "Silent Open" them in the background without losing your current focus.
* **Dynamic Ink Scaling**: Ink thickness now automatically normalizes based on the document’s true pixel resolution—ensuring your pen feels identical whether you’re on a low-res scan or a 4K vector PDF.

### **🎨 UI/UX & Quality of Life**
* **Edge-to-Edge Fit**: Rebuilt the "Fit to Width" logic to eliminate "dogshit" side gaps, providing a true edge-to-edge reading experience.
* **Precision Eraser**: Added a minimalist crosshair eraser cursor and improved stylus interpolation for buttery-smooth, high-speed erasing.
* **Non-Destructive Workflows**: The eraser now operates on an "event-based" system, allowing you to Undo/Redo entire erase strokes rather than just individual points.
* **Expanded Dashboard**: The Home Tab now tracks up to 8 Frequently Read and 8 Recent documents with high-efficiency background thumbnail generation.

### **🔧 Professional Shortcuts**
* **S** - Continuous Scrolling Mode (Edge-to-Edge)
* **D** - Single Page Mode (Fit to Window)
* **F** - Toggle Fullscreen
* **Ctrl + Drag** - Instant High-Res Region Copy
* **Right-Click (Hold)** - Lasso Selection Mode
* **Space** - Toggle Toolbar visibility in Focus Mode

### **🛠️ Setup**
1.  **Clone**: `git clone https://github.com/AlvinKirath/Mr.AlvinRocks-Reader.git`
2.  **Dependencies**: `pip install PySide6 PyMuPDF`
3.  **Run**: `python PDFViewer.py`

**Pro-Tip**: For the best experience on Windows, convert the script to an `.exe` using Inno Setup or PyInstaller to set it as your system's default PDF/DjVu handler.
