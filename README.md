# Daily Stand-up Manager

A single-page web application designed to streamline your team's daily stand-up meetings. Manage speaker time, track team members, and organize discussion topics all in one place.

![Stand-up Manager](https://img.shields.io/badge/version-1.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

## Quick Start

### Running the App

1. **Download** the `standup-manager.html` file from this repository
2. **Double-click** the file to open it in your default web browser
3. **Start using** immediately - no installation required!

**Alternative methods:**

- Right-click the file → "Open with" → Choose your preferred browser
- Drag and drop the file into an open browser window
- From browser: File → Open → Select the HTML file

### First Time Setup

1. **Add your team members:**

   - Click the gear icon (⚙️) next to the team names area
   - Either type names manually or upload a `.txt` file with one name per line
   - Sample team file format:
     ```
     Alice
     Bob
     Charlie
     ```

2. **You're ready to go!** Select a team member and start your stand-up

## Features

### 🎯 Timer Management

- **1-minute countdown timer** that starts from 01:00
- Timer continues into negative values to track overtime
- **Start, Pause, and Reset** controls
- Visual feedback with red display for negative time
- Dynamic greeting messages that change based on timer state:
  - "Hi [Name], it's your turn!" (when timer > 10 seconds)
  - "It's time to wrap up [Name]!" (when timer ≤ 10 seconds)
  - "Time's up [Name]!" (when timer goes negative)

### 👥 Team Member Management

- Horizontal display of team member names with click-to-select functionality
- **Single active selection** - only one team member can be selected at a time
- **Smart timer protection** - switching members while timer is running triggers a confirmation dialog
- **Manage team names** via sliding drawer interface:
  - Add individual team members
  - Remove individual members
  - **Load names from text file** (one name per line)
  - **Bulk import** with options to replace or append to existing names
  - **Remove all names** with confirmation
  - Automatic duplicate detection

### 📝 Discussion Items Panel

- Track items that need further discussion after stand-up
- Each item includes:
  - Auto-incrementing serial number
  - Person's name
  - Topic/title
- **Add items** via simple form inputs
- **Remove items** with × button and confirmation
- **Discussion Topics guide** for common stand-up discussion points

### 📋 Stand-up Guidelines

- Built-in reference for standard stand-up questions:
  - What did you accomplish yesterday?
  - What will you work on today?
  - Are there any blockers or impediments?
  - Keep it brief - aim for 1 minute per person

## How to Use

### Setting Up Your Team

1. Click the **gear icon (⚙️)** on the right side of the team names section
2. Choose one of the following methods:
   - **Manual Entry**: Type names one by one and click "Add Name"
   - **File Upload**: Upload a `.txt` file with one name per line
   - Sample format for text file:
     ```
     Alice
     Bob
     Charlie
     Diana
     ```

### Running a Stand-up

1. **Select a team member** by clicking their name
2. **Start the timer** when they begin speaking
3. Watch for the greeting message to change:
   - Purple message = Going well
   - Red message = Time to wrap up (≤10 seconds) or overtime
4. **Pause** if needed for clarifications
5. **Switch to next person** - you'll get a confirmation if timer is running
6. **Reset** timer for each new speaker

### Managing Discussion Items

1. During stand-up, add items to discuss later
2. Enter the person's name and topic in the right panel
3. Click "Add Item" or press Enter
4. Remove items by clicking the × button when discussed
5. Reference the "Discussion Topics" guide for ideas

## File Structure

```
├── standup-manager.html     # Main application file
├── sample-team-names.txt    # Example team names file
└── README.md               # This file
```

## Browser Compatibility

Works on all modern browsers:

- ✅ Chrome/Edge (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Opera

## Tips & Best Practices

- **Keep stand-ups focused**: Use the 1-minute timer guideline
- **Prepare your team list**: Load names from a file before the meeting
- **Track blockers**: Use the discussion items panel for follow-up topics
- **Visual cues**: The greeting message changes color and text to help keep timing on track
- **Timer flexibility**: Timer continues into negative time so no one gets cut off abruptly

## Technical Details

- **Framework**: Pure vanilla JavaScript (no dependencies)
- **File size**: ~50KB (single HTML file)
- **Storage**: All data stored in memory (resets on page reload)
- **Responsive**: Adapts to different screen sizes

## Future Enhancements

Potential features for future versions:

- Way for parctipants to add items to discuss later remotely
- Sound notification

## Contributing

Contributions are welcome! Feel free to:

- Report bugs
- Suggest new features
- Submit pull requests

## License

MIT License - Feel free to use and modify for your team's needs.

## Support

If you encounter any issues or have questions:

1. Check the Discussion Topics guide in the app
2. Review this README
3. Open an issue on GitHub

---

**Made for teams who want efficient, focused stand-ups** 🚀
