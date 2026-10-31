# Graph Plotting Calculator (OCR NEA Project)
## Overview
A comprehensive, Python-based desktop graphing calculator and data analysis tool developed as an OCR Computer Science Non-Exam Assessment (NEA). Designed specifically for high school and university students studying mathematics and science, the software replicates key features of industry-standard tools (like Desmos and GeoGebra) while remaining lightweight, user-friendly, and offline-accessible.

## Key Features
- Cartesian Graphing (X-Y Mode):
    * Allows user to input equations in terms of x or y, include functions like f(x), g(x), h(x)
    * Full support for advanced mathematics: Trigonometric functions (with Radian/Degree toggles), logarithms, exponentials, and modulus/absolute values (|x|)
    * Automated root, x/y intercept calculatons, and derivative-based Tangent/Normal line generation
- Scatter Plotting & Data Analysis (X-Y Table Mode):
    * Multi-column table input supporting dual y-value columns (y1, y2) for data comparison
    * Automated regression models for Line of Best Fit (Linear, Quadratic, Cubic, Exponential) and direct scatter line connection
- Interactive UI & On-screen Keyboard:
    * Built using Tkinter with dynamic, scrollable entry fields that auto-expand upon user input
    * Fully integrated virtual on-screen keyboard featuring mathematical symbols, Greek characters ($\pi$)
    * Collapsible/animatable keyboard tray to maximise workspace visibility
- Customisation & Export Utilities:
    * Real-time grid scaling, coordinate pan/zoom features, and dynamic axis labelling
    * Custom RGB line colouring and style formatting (solid, dotted, dashed, dash-dot)
    * Session persistence via CSV file serialisation (save/retrieve functions and coordinates) and chart exportation as image files

## Tech Stack & Libraries 
- Language: Python
- GUI Framework: Tkinter (Custom frames, canvases, scrollbars, and menubuttons)
- Graph Rendering: Matplotlib (Embedded via FigureCanvasTkAgg and navigation toolbars)
- Mathematical Processing & Parsing: SymPy & NumPy (Symbolic calculus, algebra solving, matrix handling, and array-based coordinate mapping)
- Data Storage: CSV

## System Design & Development Methodology
- Methodology: Developed iteratively using an Agile Framework, breaking down requirements into independent phases (UI Design, Input handling, Equation Processing, Advanced Features, and File Persistence)
- Architecture: Component-driven separation of concerns fefaturing dynamic widget management, exception-driven error handling for invalid user syntax, and Object-Oriented state tracking.

## Project Structure & Phases 
1. **Phase 1 (User Interface)**: Structural layout setup, frame partitioning, and Matplotlib canvas embedding
2. **Phase 2(Input system)**: Custom MenuBar integration, dynamic text-box row creation, and event-driven keyboard binding
3. **Phase 3 (Equation Processing & Output)**: SymPy/NumPy backend integration, custom domain/range graphing panels, and analytical tangent/normal vector derivation
4. **Phase 4 (Table Processing & Coordinates)**: Scatter data mapping, automated CSV parsing, and vector calculations.
5. **Phase 5 (On-Screen Keyboard & Animations)**: Virtual symbol layout, focus tracking, and smooth toggle animations
6. **Phase 6 (Advanced Features)**: Dynamic axis auto-anchoring, pan/drag grid logic, RGB color routing, and custom line styles
7. **Phase 7 (Store, Retrieve & Reset)**: State preservation via CSV export/import modules and application memory clearing

## Future Improvement
- Integration calculation features to compute the area under a curve
- Direct equation-to-table projection mapping based on user feedback
