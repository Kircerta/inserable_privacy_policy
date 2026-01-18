# Inserable Privacy Policy

[Click Here to View the Webpage](https://kircerta.github.io/inserable_privacy_policy/)

# Inserable User Manual
### Beta Version 1.0.0

Inserable is an image management and Markdown editing tool designed specifically for Hugo static blogs. It helps you automatically standardize image naming, manage the association between images and articles, and streamline your blog writing workflow.

---

## Table of Contents

1. [Quick Start](#quick-start)
2. [Core Concepts](#core-concepts)
3. [Interface Introduction](#interface-introduction)
4. [Basic Operations](#basic-operations)
5. [Advanced Features](#advanced-features)
6. [Settings Description](#settings-description)
7. [Frequently Asked Questions](#frequently-asked-questions)

---

## Quick Start

### Step 1: Configure Root Folders

1. Open Inserable and click the **SETTINGS** button at the bottom.
2. Set **Image Root Folder**: Select the folder where images are stored in your Hugo site (usually `static/images`).
3. Set **Markdown Root Folders**: Click **Add** to include your article directories (usually `content/posts`).

### Step 2: Create or Import a Session

- **Drag and Drop Images**: Drag images or image folders directly into the left list to automatically create a Session.
- **One-Tap Mapping**: Click **UTILITY** → **One-Tap Mapping** to import existing image folders with one click.

### Step 3: Bind Markdown Files

1. Select a Session.
2. The application will automatically detect Markdown files matching the Session name.
3. Click to confirm the binding and start editing.

---

## Core Concepts

### Session

A Session is the core unit of Inserable, representing a combination of an article and its related images:

- Each Session corresponds to a folder under the Image Root.
- Folder naming format: `article_name_session_folder`.
- A Session can be bound to one Markdown file.

### Standardized Naming

Inserable automatically renames images into a unified format:

```
article_name_001.png 
article_name_002.png 
article_name_003.png
```

Benefits:
- Images are arranged in sequence.
- Easy to reference in Markdown.
- Avoids issues caused by Chinese or special characters.

### Two-way Binding

Once a binding is established between a Session and a Markdown file:
- Edits in Inserable are synchronized to the Markdown file.
- Pasting images automatically inserts the correct reference path.

---

## Interface Introduction

### Left Side: Session List

- Displays all Sessions grouped by folder hierarchy.
- Click a row to expand or collapse folders.
- Green icons indicate a bound Markdown file.
- Gray icons indicate no binding.

### Right Side: Detail Panel

Two view modes (switch via the rotation icon next to the title):

**Images View**
- Displays all images in the Session.
- Supports drag-and-drop to add new images.
- Double-click the title to rename the Session (this synchronizes image filenames and URLs in Markdown).

**Markdown View**
- Displays and allows editing of the bound Markdown content.
- Supports syntax highlighting.
- Double-click the title to rename the Markdown file.
- Supports direct image pasting (Cmd+V).

### Bottom Bar

- **IN SYNC**: Data synchronization status indicator.
- **SETTINGS**: Opens the settings panel.
- **COPY**: Copies the content of the current view.

---

## Basic Operations

### Adding Images to a Session

**Method 1: Drag and Drop**
1. Select the target Session.
2. Drag images into the right panel.
3. Images are automatically standardized and added to the Session.

**Method 2: Paste (Recommended)**
1. Switch to Markdown View.
2. Place the cursor where you want to insert the image.
3. Copy an image or screenshot and press Cmd+V.
4. The image is automatically saved and the reference is inserted.

### Renaming

**Rename Session (Images View)**
- Double-click the title to enter edit mode.
- Enter the new name and press Enter.
- Automatically updates: folder name, all image filenames, and URL paths in Markdown.

**Rename Markdown File (Markdown View)**
- Double-click the title to enter edit mode.
- Enter the new name and press Enter.
- Only renames the Markdown file itself.

### Delete Session

1. Select the Session.
2. Right-click or use the delete button.
3. Confirm deletion (the folder will be moved to the Trash).

---

## Advanced Features

### One-Tap Mapping

Automatically migrate existing image folders to Inserable management:

1. Click **UTILITY** → **One-Tap Mapping**.
2. The application scans all folders under the Image Root.
3. Automatically matches image references in Markdown files.
4. Completes migration and binding with one click.

### Batch Standardization

Process unstandardized Sessions in batches:

1. Click **UTILITY** → **Standardize All**.
2. All unstandardized Sessions will be processed automatically.

### TextBundle Import

Supports importing from TextBundle format:

1. Click **IMPORT TEXTBUNDLE**.
2. Select the .textbundle file.
3. Automatically extracts images and Markdown content.

---

## Settings Description

### Image Root Folder

The root directory containing all Session image folders.

Recommended to set as the `static/images` directory of your Hugo site.

### Markdown Root Folders

The root directories containing Markdown articles. Supports adding multiple folders (for multi-language sites).

Recommended to set as the `content/posts` directory of your Hugo site.

### Appearance

- **Dark Mode**: Switch between dark and light themes.
- **Background Effect**: Toggle dynamic background effects.

### General

- **Delete original images**: Whether to delete original images after processing.
- **Delete original folders**: Whether to delete original folders after processing.

---

## Frequently Asked Questions

### Q: No response when pasting images?

A: Ensure:
1. A Session is selected.
2. You are currently in Markdown View.
3. The cursor is within the text editing area.

### Q: Image URL displayed in red?

A: Indicates the image file does not exist. Possible reasons:
- Image was manually deleted.
- Session was renamed but Markdown was not synchronized.

Solution: Click **Standardize** to re-synchronize.

### Q: How to handle existing blog images?

A: Use the **One-Tap Mapping** feature for one-click migration.

### Q: What image formats are supported?

A: Supports PNG, JPG, JPEG, GIF, and WebP. All images will be automatically converted to PNG format.

### Q: Where is the data stored?

A: 
- Images are stored in your configured Image Root Folder.
- Session metadata is stored within the application sandbox.
- Markdown files are stored in your configured Markdown Root Folders.

---

## Keyboard Shortcuts

| Shortcut | Function |
|----------|----------|
| Cmd+V | Paste image (Markdown View) |
| Cmd+Z | Undo |
| Cmd+Shift+Z | Redo |
| Enter | Confirm renaming |
| Esc | Cancel renaming |

---

## Contact and Feedback

For questions or suggestions, please contact via:

- Email: kircerta@gmail.com

Thank you for using Inserable!
