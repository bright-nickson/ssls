# File Share Hub

A modern, responsive web application for uploading, managing, and sharing files. Built with HTML, CSS, and JavaScript using TailwindCSS for styling.

## Features

### 📤 File Upload
- **Drag & Drop**: Simply drag files onto the upload area
- **Click to Browse**: Traditional file selection via button
- **Multiple Files**: Upload multiple files simultaneously
- **Progress Tracking**: Visual progress bar for uploads
- **File Validation**: Automatic validation for file types and sizes

### 📁 File Management
- **Preview**: Quick preview for images, PDFs, and text files
- **Download**: One-click download for any uploaded file
- **Delete**: Remove unwanted files with confirmation
- **Search**: Find files by name instantly
- **Filter**: Filter by file type (PDF, Word, PowerPoint, Excel, Images, Other)
- **Sort**: Sort files by date, name, or size

### 💾 Storage
- **Local Storage**: Files are stored in browser's localStorage
- **Persistent**: Files remain available even after page refresh
- **Capacity**: Supports up to 50MB per file

### 🎨 User Interface
- **Modern Design**: Clean, professional interface using TailwindCSS
- **Responsive**: Works perfectly on desktop, tablet, and mobile
- **Animations**: Smooth transitions and hover effects
- **File Icons**: Color-coded icons for different file types
- **Toast Notifications**: Non-intrusive feedback messages

## Supported File Types

### Documents
- PDF (.pdf)
- Microsoft Word (.doc, .docx)
- Microsoft PowerPoint (.ppt, .pptx)
- Microsoft Excel (.xls, .xlsx)
- Plain Text (.txt)

### Images
- JPEG (.jpg, .jpeg)
- PNG (.png)
- GIF (.gif)
- WebP (.webp)

### Other
- ZIP archives (.zip)

## Getting Started

1. **Open the Application**: Open `index.html` in your web browser
2. **Upload Files**: 
   - Drag and drop files onto the upload area, or
   - Click "Browse Files" to select files from your device
3. **Manage Files**: 
   - Use the search bar to find specific files
   - Filter by file type or sort by different criteria
   - Click the eye icon to preview files
   - Click the download icon to save files
   - Click the trash icon to delete files

## Technical Details

### File Storage
- Files are stored as base64 encoded data in localStorage
- Maximum file size: 50MB per file
- Storage limit depends on browser's localStorage capacity

### Browser Compatibility
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

### Security Considerations
- Files are stored locally in the browser only
- No server-side storage or processing
- Files are not transmitted to any external service

## File Structure

```
slidess/
├── index.html          # Main HTML file
├── styles.css          # Custom CSS styles
├── script.js           # JavaScript functionality
└── README.md           # This documentation
```

## Usage Tips

1. **Large Files**: For very large files, consider the browser's localStorage limits
2. **Backup**: Important files should be backed up elsewhere as localStorage can be cleared
3. **Mobile**: The interface is fully responsive and works great on mobile devices
4. **Keyboard Navigation**: Use Tab key to navigate through the interface

## Troubleshooting

### Common Issues

**"Storage quota exceeded" error**
- Clear some files or use a different browser
- localStorage has limited capacity (usually 5-10MB)

**File not uploading**
- Check if file type is supported
- Ensure file size is under 50MB
- Try refreshing the page and uploading again

**Files disappear after browser restart**
- Some browsers clear localStorage when closed
- Check your browser's storage settings

**Preview not working**
- Preview is only available for images, PDFs, and text files
- Other file types will show a download option instead

## Development

### Customization
- Modify `styles.css` to change the appearance
- Update `script.js` to add new features
- Edit `index.html` to modify the layout

### Adding New File Types
1. Add the MIME type to the `allowedTypes` array in `script.js`
2. Update the `getFileIcon` method to include an icon
3. Add the file type to the filter dropdown in `index.html`

## License

This project is open source and available under the MIT License.
