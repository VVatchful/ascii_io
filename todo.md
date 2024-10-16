├── cmd/                    # Main entry point
│   └── main.go             # Main program logic, server initialization
│
├── internal/               # Core project functionality
│   ├── ascii/              # ASCII conversion logic
│   │   ├── converter.go    # Converts media (image, gif, video frames) to ASCII
│   │   ├── image.go        # Functions to convert images to ASCII
│   │   ├── gif.go          # Functions to handle GIF to ASCII
│   │   ├── video.go        # Frame extraction and conversion for video to ASCII
│   │   └── utils.go        # Helper functions (e.g., brightness calculation)
│   │
│   ├── handlers/           # API handlers for handling media uploads
│   │   ├── uploadHandler.go # Processes user uploads and calls converters
│   │   └── convertHandler.go # Handles conversion logic and returns ASCII results
│   │
│   ├── gui/                # Frontend logic for GUI
│   │   ├── webview.go      # GUI logic (if using webview for GUI)
│   │
│   │
│   └── server/             # HTTP server logic
│       └── server.go       # Server setup, routes, and middleware
│
├── assets/                 # Static files for GUI (e.g., images, stylesheets)
│   └── css/                # Stylesheets (if using web-based frontend)
│
├── tests/                  # Test files
│   ├── ascii_test.go       # Unit tests for ASCII conversion
│   ├── image_test.go       # Unit tests for image conversion
│   ├── gif_test.go         # Unit tests for GIF handling
│   └── video_test.go       # Unit tests for video frame extraction
