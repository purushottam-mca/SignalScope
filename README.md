## SignalScope

**SignalScope** is a high-performance desktop application designed for visualizing, analyzing, and persisting multi-series waveform data. It bridges the gap between raw CSV data and interactive visual insights by providing a smooth zoom/pan experience and a persistent annotation system.

---

### Project Vision
To build a lightweight yet powerful tool that allows users to:
1. Load multiple complex waveforms simultaneously.
2. Navigate through massive datasets with fluid performance.
3. Map and save custom labels/annotations to a local database for repeated analysis.

### Tech Stack (Planned)
*   **Language:** Python 3.x
*   **GUI Framework:** PySide6 (Qt for Python)
*   **Styling:** QSS (Qt Style Sheets)
*   **Plotting Engine:** PyQtGraph (for high-performance rendering)
*   **Data Handling:** Pandas & NumPy
*   **Persistence:** SQLite3

### Roadmap

#### Phase 1: Core Foundation (In Progress)
- [ ] Basic UI Layout with PySide6.
- [ ] CSV Data Parsing using Pandas.
- [ ] Integration of PyQtGraph for primary plotting.
- [ ] Implementation of basic Zoom/Pan functionality.

#### Phase 2: Persistence & Interaction
- [ ] SQLite Database Schema Design.
- [ ] "Click-to-Label" interaction logic.
- [ ] Save/Load session functionality (Waveforms + Annotations).
- [ ] Custom QSS Theme implementation.

#### Phase 3: Advanced Features & Optimization
- [ ] Downsampling algorithms for extremely large datasets (>1M points).
- [ ] Exporting annotated data to JSON/CSV.
- [ ] Multi-threading for smooth UI during heavy DB operations.

### Architecture Plan
The project will follow a modular structure:
*   `core/`: Database logic and file handling.
*   `ui/`: PySide6 widgets and QSS styling.
*   `plots/`: PyQtGraph configuration and custom plot items.
*   `utils/`: Data processing and math helpers.
