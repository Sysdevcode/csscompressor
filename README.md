# CSS Compressor Utility v3

A modern, feature-rich CSS compression and formatting tool built as a single HTML file application. This utility allows you to optimize, format, and compress CSS with advanced control over output style.

## Features

### 🚀 Core Compression
- **Multiple compression modes**: From minified to readable output
- **Smart formatting**: Automatic line wrapping based on breakpoints
- **Property optimization**: Color shortening, value optimization, and property sorting
- **Comment preservation**: Option to preserve important comments (`/* */`)

### 🎨 Output Modes
- **Highest (Minified)**: Ultra-compressed single-line output
- **High (Compact)**: One rule per line, minimal whitespace
- **Standard (Smart)**: Intelligent line wrapping based on column limit
- **Low (Pretty)**: Readable, well-indented formatting

### 🔧 Advanced Features
- **Undo/Redo history**: Track up to 50 changes
- **Auto-compress**: Real-time optimization as you type
- **Preset configurations**: One-click settings for common use cases
- **Clipboard integration**: Paste from and copy to clipboard
- **File download**: Export optimized CSS as a `.css` file
- **Validation**: Detects common CSS errors and warnings

### ⌨️ Keyboard Shortcuts
- `Ctrl+Enter`: Compress CSS
- `Ctrl+Z`: Undo
- `Ctrl+Y`: Redo
- `Ctrl+S`: Download output (when in output panel)

## Usage

### Quick Start
1. Open `compressor.html` in any modern web browser
2. Paste your CSS into the "Input CSS" panel
3. Select your preferred compression settings
4. Click "Compress" or press `Ctrl+Enter`
5. Copy or download the optimized output

### Settings Explained

#### Compression Mode
- **Highest**: Maximum compression, removes all whitespace and comments
- **High**: One CSS rule per line, minimal whitespace
- **Standard**: Smart formatting with configurable line length
- **Low**: Readable, multi-line formatting with full indentation

#### Options
- **Indent**: Number of spaces for indentation (0-8)
- **Breakpoint**: Line length before wrapping (20-200 characters)
- **Soft Newline**: Enable smart line wrapping
- **Optimize Colors**: Convert colors to shortest form (e.g., `#ffffff` → `#fff`)
- **Optimize Values**: Simplify values (e.g., `0px` → `0`, `margin: 10px 20px 10px 20px` → `margin: 10px 20px`)
- **Sort Properties**: Alphabetize CSS properties
- **Preserve /*! */ Comments**: Keep important comments during compression
- **Auto-compress**: Automatically compress on input changes

#### Presets
- **Minify**: Maximum compression for production
- **Compact**: Small file size with some readability
- **Standard**: Balanced compression and readability
- **Readable**: Developer-friendly formatting

## Technical Details

### How It Works
The application uses a custom CSS tokenizer and parser that:
1. Replaces comments with placeholders for processing
2. Tokenizes CSS into rules, at-rules, and declarations
3. Applies optimizations based on selected options
4. Formats output according to the chosen mode
5. Restores comments from placeholders

### File Size Handling
- **Small files**: Instant processing
- **Large files (>50KB)**: Shows progress bar with asynchronous processing
- **Memory efficient**: Processes files without blocking the UI

### Browser Compatibility
Works in all modern browsers with ES6 support:
- Chrome 60+
- Firefox 55+
- Safari 11+
- Edge 79+

## Error Handling
The utility provides helpful feedback for:
- Unmatched braces
- Empty property values
- Parsing errors
- Clipboard permission issues

## Version History

### v3 Improvements
- ✅ Fixed comment handling in all compression modes
- ✅ Removed trailing semicolons in declarations
- ✅ Improved edge case support for complex CSS
- ✅ Enhanced property sorting with logical categories
- ✅ Better handling of nested at-rules and media queries

## Project Structure
The application is contained in a single HTML file with:
- **HTML**: Semantic structure with accessibility considerations
- **CSS**: Modern CSS with CSS Custom Properties for theming
- **JavaScript**: Modular, commented code with clear separation of concerns

## License
Copyright 2025 Sysdevcode

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
- The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Support
- For feature requests, please leave a message.
- For issues, please check the browser console for error messages and ensure your CSS syntax is valid.

---

**Note**: This is a client-side application. Your CSS is processed entirely in your browser - no data is sent to any server.
