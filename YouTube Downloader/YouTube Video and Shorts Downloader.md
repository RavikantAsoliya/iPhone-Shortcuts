# Creating Your Own YouTube Video and Shorts Downloader Shortcut

In this tutorial, you'll learn how to create your own iPhone shortcut for downloading YouTube videos and shorts directly to your device.

## Prerequisites

- An iPhone with the Shortcuts app installed.
- Basic familiarity with the Shortcuts app interface.

## Phase 1: Getting Started

1. Open the Shortcuts app on your iPhone.

2. Tap on the "+" icon to create a new shortcut.

## Phase 2: Adding Actions

### Step 1:

1. Tap on "Add Action".

2. Search for "Match Text".

3. Select "Match Text" from the list of actions.

4. Replace the default pattern with the following pattern:

   ```regex
   (?:youtu\.be\/|youtube(?:-nocookie)?\.com\/(?:[^\/\n\s]+\/\S+\/|(?:v|e(?:mbed)?)\/|\S*?[?&]v=|\S*?[?&]vi=|shorts\/))([\w-]{11})
   ```

5. In the "Text" placeholder, select "Shortcut Input".

### Step 2:

After completing step 1, you will see that a block starting with "Receive" has been added.

1. Clear all received items and choose only "Safari Web Pages" and "URL".

2. Click on "Continue" and replace it with the "Get Clipboard" option.

3. In the "NowWhere" section, select "Share Sheet".