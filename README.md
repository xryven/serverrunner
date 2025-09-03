# ServerRunner

A lightweight Windows Forms application for managing and launching server projects from a centralized location.
Can be used for simple Minecraft Servers or any other server

## Features

- **Clean, Modern UI**: Dark theme with a minimalist design
- **Automatic Discovery**: Scans your `.server` folder for projects with `start.bat` or `run.bat` files
- **Quick Launch**: Double-click any server project to run it instantly
- **Borderless Design**: Sleek window without traditional borders, featuring a dotted outline
- **Drag Support**: Move the window by dragging anywhere on the interface

## Usage

### Setup Your Server Projects

1. Create a `.server` folder in your Documents directory:
   ```
   %USERPROFILE%\Documents\.server\
   ```

2. Organize your server projects in subfolders:
   ```
   Documents/
   └── .server/
       ├── my-web-server/
       │   ├── start.bat
       │   └── [other project files]
       ├── api-server/
       │   ├── run.bat
       │   └── [other project files]
       └── game-server/
           ├── start.bat
           └── [other project files]
   ```

### Running ServerRunner

1. Download and run ServerRunner.exe
2. The application will automatically scan your `.server` folder
3. All valid server projects will appear in the list
4. Double-click any project to launch it

### Example Batch Files

**start.bat** (Node.js server):
```batch
@echo off
npm start
pause
```

**run.bat** (Python server):
```batch
@echo off
python app.py
pause
```

## Requirements

- Windows OS
- .NET Framework 4.7.2 or later

That's it!
