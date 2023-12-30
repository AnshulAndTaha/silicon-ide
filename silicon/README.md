# Silicon IDE
An IDE built to empower productivity and speed. Built with Rust.


## File Hierarchy
```
silicon/
├── src/
│   ├── main.rs                     # Entry point of the application
│   ├── app.rs                      # Core application logic
│   ├── gui/                        # GUI-related modules
│   │   ├── mod.rs                  # Exports the GUI modules
│   │   ├── window.rs               # Window handling and settings
│   │   ├── widgets/                # Custom widgets specific to your IDE
│   │   │   ├── mod.rs              # Exports the custom widgets
│   │   │   ├── editor.rs           # Text editor widget
│   │   │   ├── toolbar.rs          # Toolbar widget
│   │   │   └── ...                 # Other custom widgets
│   │   └── themes/                 # GUI themes and styling
│   │       ├── mod.rs              # Exports the theme modules
│   │       └── default.rs          # Default theme
│   ├── core/                       # Core functionality of the IDE
│   │   ├── mod.rs                  # Exports the core modules
│   │   ├── editor_state.rs         # State and logic of the code editor
│   │   ├── project.rs              # Project management
│   │   └── ...                     # Other core functionalities
│   ├── utils/                      # Utility functions and helpers
│   │   ├── mod.rs                  # Exports the utility modules
│   │   └── file_io.rs              # File input/output operations
│   └── config/                     # Configuration management
│       ├── mod.rs                  # Exports the config modules
│       └── settings.rs             # Application settings
├── resources/                      # Resources like images, fonts, etc.
├── tests/                          # Integration and unit tests
└── Cargo.toml                      # Rust project manifest
```
```
main.rs : The entry point of your application. This is where you set up the egui context and the main event loop.
app.rs  : Contains the primary application logic and orchestrates different components of your IDE.
gui/ : Dedicated to the graphical interface. This includes the main window setup, event handling, and custom widget definitions.
window.rs: Handles the creation and settings of the application window.
widgets/: Custom widgets that are specific to your IDE, like a text editor widget, a toolbar, etc.
themes/: Theming and styling related files.
core/: The backbone of your IDE, containing core functionalities like the editor state, project management, etc.
utils/: Utility functions and helpers that can be used across the application.
config/: Manages configuration and settings for the application.
resources/: Contains static resources like images, fonts, or other assets.
tests/: Contains your test suites, ensuring your IDE's functionality works as expected.
```