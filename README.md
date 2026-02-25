# Span — The File Explorer Windows Deserved

**A blazing-fast Miller Columns file explorer for Windows, built for power users who refuse to compromise.**

Span reimagines file navigation on Windows. Inspired by the elegance of macOS Finder's column view and supercharged with features Windows Explorer never had — multi-tab, split view, async operations, and keyboard-driven workflows that make file management feel effortless.

> **Why settle for Windows Explorer when you can fly?**

---

## Why Span?

| | Windows Explorer | Span |
|---|---|---|
| **Miller Columns** | No | Yes — hierarchical 3-pane navigation |
| **Multi-Tab** | Windows 11 only (basic) | Full tabs with tear-off, duplication, session restore |
| **Split View** | No | Dual-pane with independent view modes |
| **Preview Panel** | Basic | 10+ file types — images, video, audio, code, hex, fonts, PDF |
| **Keyboard Navigation** | Limited | 30+ shortcuts, type-ahead search, full keyboard-first design |
| **Batch Rename** | No | Regex, prefix/suffix, sequential numbering |
| **Undo/Redo** | Limited | Full operation history (configurable depth) |
| **Custom Themes** | No | Dracula, Tokyo Night, Catppuccin, Gruvbox + Light/Dark |
| **File Operations** | Modal, blocking | Async with pause/resume/cancel per operation |
| **Git Integration** | No | Branch, status, commits at a glance |
| **Remote Connections** | No | FTP, FTPS, SFTP with saved credentials |
| **Cloud Status** | Basic overlay | Real-time sync badges (OneDrive, iCloud, Dropbox) |
| **Startup Speed** | Slow on large directories | Async loading with cancellation — zero lag |

---

## Features

### Miller Columns — See Everything at Once

The signature feature. Navigate deep folder hierarchies without losing context. Each column represents one level — click a folder and its contents appear in the next column. You always see where you are and where you came from.

- Draggable column separators for custom widths
- Auto-equalize columns (Ctrl+Shift+=) or auto-fit to content (Ctrl+Shift+-)
- Smooth horizontal scrolling to keep the active column visible

### Four View Modes

Switch instantly between the view that fits your workflow:

- **Miller Columns** (Ctrl+1) — Hierarchical navigation, Span's signature
- **Details** (Ctrl+2) — Sortable table with name, date, type, size columns
- **List** (Ctrl+3) — Dense multi-column layout for scanning large directories
- **Icons** (Ctrl+4) — Grid view with 4 size options up to 256x256 thumbnails

### Multi-Tab with Full Session Restore

- Open unlimited tabs, each with its own path, view mode, and history
- **Tab tear-off**: Drag a tab out to create a new window — full state preserved
- **Tab duplication**: Clone a tab with its exact path and settings
- Session auto-save: Close the app, reopen it — every tab exactly where you left it

### Split View — True Dual-Pane

- Side-by-side file browsing with independent navigation per pane
- Each pane can use a different view mode (Miller left, Details right)
- Separate preview panels for each pane
- Ctrl+Tab to switch active pane
- Drag files between panes for copy/move operations

### Preview Panel — Know Before You Open

Press Space for Quick Look or toggle the persistent preview panel:

- **Images**: JPEG, PNG, GIF, BMP, WebP, TIFF with resolution and metadata
- **Video**: MP4, MKV, AVI, MOV, WEBM with playback controls
- **Audio**: MP3, AAC, M4A with artist, album, duration info
- **Text & Code**: 30+ extensions with syntax display
- **PDF**: First page preview
- **Fonts**: Glyph samples with metadata
- **Hex Binary**: Raw byte view for developers
- **Folders**: Size, item count, attributes at a glance

### Keyboard-First Design

30+ keyboard shortcuts for users who keep their hands on the keyboard:

| Shortcut | Action |
|----------|--------|
| Arrow Keys | Navigate columns and items |
| Enter | Open folder or execute file |
| Space | Quick Look preview |
| Backspace | Go up one level |
| Ctrl+L / Alt+D | Edit address bar |
| Ctrl+F | Search |
| Ctrl+C / X / V | Copy / Cut / Paste |
| Ctrl+Shift+V | Paste as shortcut |
| Ctrl+D | Duplicate |
| Ctrl+Z / Y | Undo / Redo |
| Ctrl+Shift+N | New folder |
| F2 | Rename (batch rename if multi-select) |
| Ctrl+T / W | New tab / Close tab |
| Ctrl+N | New window |
| Ctrl+1-4 | Switch view mode |
| Ctrl+E | Toggle split view |
| Ctrl+P | Toggle preview panel |
| A-Z, 0-9 | Type-ahead search |
| Delete | Move to Recycle Bin |
| Shift+Delete | Permanent delete |
| Alt+Enter | Properties |
| F5 | Refresh |

### Async File Operations — Never Freeze Again

Every file operation runs asynchronously with real-time feedback:

- **Progress tracking**: Speed (MB/s), time remaining, file count
- **Pause / Resume / Cancel**: Per-operation controls
- **Concurrent operations**: Copy in one tab while moving in another
- **Conflict resolution**: Auto-rename with smart suffixes
- **Full Undo/Redo**: Revert copy, move, rename, and delete operations

### Batch Rename

Select multiple files, press F2:

- **Find & Replace** with regex support
- **Add prefix or suffix** to all selected files
- **Sequential numbering** with custom patterns
- Live preview before applying

### Smart Search

- **Type-ahead**: Start typing in any column to filter instantly
- **Structured queries**: `type:image`, `size:>100MB`, `date:today`, `ext:.pdf`
- **Live filtering** with auto-scroll to matched items

### Address Bar — Breadcrumb + Direct Edit

- **Breadcrumb mode**: Click any path segment to jump directly
- **Edit mode** (Ctrl+L): Type or paste any path — local, network, or UNC
- Seamless toggle between modes

### Themes & Customization

- **Themes**: Light, Dark, System, Dracula, Tokyo Night, Catppuccin, Gruvbox
- **Density**: Compact, Comfortable, Spacious
- **Icon Packs**: Remix Icon (default), Phosphor Icons, Tabler Icons
- **Font**: Configurable font family
- Instant theme switching — no restart required

### Sidebar — Everything Within Reach

- **Local Drives**: HDD, SSD, USB with capacity bars
- **Cloud Storage**: OneDrive, iCloud, Dropbox auto-detection
- **Network Drives**: Mapped drives with status
- **Favorites**: Drag folders to pin, reorder by drag, custom colors
- **Recent Folders**: Last 20 visited locations
- **USB Hotplug**: Drives appear and disappear in real-time

### Cloud Storage Integration

Native Windows Cloud Files API support:

- **Sync status badges**: Cloud-only, Synced, Pending Upload, Syncing
- **Smart thumbnails**: Uses cached previews only — never triggers unwanted downloads
- **OneDrive, iCloud, Dropbox** detection out of the box

### Git Integration

Optional, toggleable git status for developers:

- **Branch name** and repository status
- **File status**: Modified, Added, Deleted, Untracked, Staged
- **Recent commits** with hash, message, and timestamp
- Auto-detection of git.exe installation

### Remote Connections

Connect to remote servers directly from Span:

- **FTP / FTPS / SFTP** with saved connection profiles
- **SSH key authentication** support
- **Encrypted credential storage** via Windows ProtectedData

### Context Menu — Full Windows Shell Compatibility

- 100% native Windows shell extension support — every context menu item works
- Additional Span items: Open Terminal, Copy Path, Pin to Favorites, Compress/Extract
- Toggleable sections: Shell extras, Copilot items, Developer menu
- Full Korean and Japanese shell verb translation

### Drag & Drop

- **Internal**: Drag between Span columns, tabs, and panes
- **External**: Drag to/from Windows Explorer and Desktop
- **Modifier keys**: Hold Ctrl to copy, Shift to move
- **Favorites**: Drag folders to sidebar to pin them
- Visual feedback with operation caption overlay

### Sorting & Grouping

- **Sort by**: Name, Date Modified, Type, Size — ascending or descending
- **Group by**: None, Name, Type, Date, Size — with visual group headers
- Consistent across all view modes
- Accessible from toolbar and context menu

### Localization

- English, Korean (한국어), Japanese (日本語)
- System language auto-detection
- Full UI translation including context menus

---

## Performance

Span is engineered for speed. Every interaction is designed to feel instant.

- **Async I/O everywhere**: File listing, thumbnails, previews — nothing blocks the UI thread
- **Cancellation tokens**: Navigate away and stale operations are cancelled immediately
- **Batch property updates**: Thousands of items load with minimal UI overhead
- **Debounced selection**: Smart 150ms delay prevents redundant work during rapid navigation
- **Per-tab caching**: Switch tabs instantly — content is preserved, not reloaded
- **Drive timeout protection**: Unresponsive drives are skipped after 500ms
- **Concurrent thumbnail loading**: Up to 6 simultaneous loads with SemaphoreSlim throttling
- **Instant tab switching**: Show/Hide pattern — no re-rendering on tab change

---

## System Requirements

- **OS**: Windows 10 version 1809 or later
- **Recommended**: Windows 11 for full visual experience (Mica backdrop, rounded corners)
- **Architecture**: x64, x86, ARM64

---

## Links

- [Privacy Policy](PRIVACY.md)
- [Open Source Licenses](LICENSES.md)
- [Bug Reports & Feedback](https://github.com/kangjinkyu/Span/issues)

---

## License

Copyright (c) 2026 LumiBear Studio. All rights reserved.

Span is proprietary software developed by LumiBear Studio. This repository hosts documentation only.
