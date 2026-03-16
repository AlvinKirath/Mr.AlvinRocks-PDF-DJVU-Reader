# Mr.AlvinRocks-PDF-DJVU-Reader
A high-performance, feature-rich PDF &amp; Document reader with advanced annotation, infinite notes, and ultra-fast DjVu support.
That's a bold way to put it! Here is the revised Mr.AlvinRocks' PDF/DJVU Reader README. It includes the updated installation instructions and a very clear "Default App" directive for those who want a seamless experience.

📑 Mr.AlvinRocks' PDF/DJVU Reader
⚠️ DISCLAIMER: This entire application was built from scratch in just four days. Alvin, the lead architect, began this project with zero formal background in Computer Science. By leveraging advanced Artificial Intelligence as a collaborative partner, this project serves as a testament to what is possible when human intent meets AI execution.

🌟 Why is this the best PDF option?
Most PDF readers are "Passive". They let you look, but they make it hard to work. Mr.AlvinRocks' Reader is an "Active" environment. It bridges the gap between a document viewer and a digital journal, allowing you to harvest information from PDFs and organize it in a high-res, infinite canvas without ever leaving the app.

🚀 Key Feature Breakdown
1. High-Performance Hybrid Engine
Lazy-Loading DjVu Core: Unlike traditional readers that crash while loading 500MB DjVu files, our engine renders only the active viewport. It utilizes a custom C++ integration with DjVuLibre for lightning-fast page flipping.

Universal Format Support: Natively handles PDF, DjVu, EPUB, XPS, CBZ, and all major image formats (WebP, TIFF, JPEG).

Adaptive Geometry: Specifically tuned for all displays. Whether you are on a 720p TV or a 4K monitor, our QTimer layout synchronization ensures your "Fit Page" and "Continuous" modes are pixel-perfect every time.

2. The "Lossless Snap" Ecosystem
3x High-Res Snapping: Stop taking blurry screenshots. Our Snap tool reaches into the PDF source code to extract regions at 3x their native resolution.

Instant Journaling: "Snap-to-Note" functionality automatically opens a Blank Note tab and pastes your selection at high quality, allowing for instant annotation and study.

Infinite Verticality: Our Blank Notes use an "Auto-Expand" engine. As you reach the bottom of your note, the canvas automatically grows, giving you a limitless space to write and paste.

3. Professional Presentation & Markup
Pulsing Laser Pointer: A presentation-grade tool with a mathematical "glow" animation that makes remote sharing and screen recording more engaging.

Lasso Tool (Polygon Selection): Move beyond rectangles. Select complex groups of ink strokes or specific image regions with a free-hand lasso.

Pressure-Sensitive Ink: Native support for stylus pressure and hardware erasers, providing a pen-on-paper feel.

Text-Aware Highlighting: A smart toggle that lets you "paint" highlights that automatically snap to the underlying PDF text layers.

4. Advanced Navigation & UI
Multi-Tab Session Memory: The app remembers exactly where you left off. Every document's zoom level, rotation, dark mode state, and specific page number are saved to the Windows Registry automatically.

Background Search Indexing: Search 2,000+ page documents without the UI freezing. We use processEvents() threading to keep the app responsive while a real-time progress bar tracks your search results.

Split-View Mode: Read two different parts of the same document (or two different files) side-by-side in a single window.

🎨 Professional Shortcuts (The Speed Workflow)
S - Continuous Scrolling Mode (Fit to Width)

D - Single Page Mode (Fit to Window)

F - Fullscreen (Focus Mode)

Space - Toggle UI visibility while in Fullscreen

I / A / V - Instant switch between Pen, Highlighter, and View tools.

Ctrl + B - Toggle Sidebar (Bookmarks and Thumbnails)

🛠️ Installation & Setup
Clone the Repo: git clone https://github.com/AlvinKirath/Mr.AlvinRocks-Reader.git

Install Dependencies: pip install PySide6 PyMuPDF

Run: python PDFViewer.py

⚙️ Pro-Tip for Default App usage: If you want to use this as your default reader for PDF and DjVu files, you should convert the Python script into an executable (.exe) using a tool like Inno Setup. Windows requires an executable file to reliably set a program as the "Default App" in your system settings.
