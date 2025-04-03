- **Shortcut Categorization:**

    - Are we grouping them by function (e.g., navigation, window management, text editing), frequency of use, or another metric?
    - 
- **General Shortcuts** 
-     This category includes everyday commands that most users perform regularly. For clarity, we can subdivide them into smaller, manageable groups:
#### **Windows 10 General Shortcuts**
```dataviewjs
const rows = [
  ["File menu", "Alt+F, or F10 then F"],
  ["Edit menu", "Alt+E"],
  ["View menu", "Alt+V"],
  ["Undo the last operation", "Ctrl+Z, or Alt+← Backspace"],
  ["Redo the last operation", "Ctrl+Y, or Alt+Shift+Backspace"],
  ["Cut the selection and store it in the clipboard", "Ctrl+X, or ⇧ Shift+Del"],
  ["Copy the selection into the clipboard", "Ctrl+C, or Ctrl+Ins"],
  ["Paste contents of clipboard at cursor", "Ctrl+V, or ⇧ Shift+Ins"],
  ["Paste special", "⊞ Win+V"],
  ["Select all in focused control or window", "Ctrl+A"],
  ["Cycle through installed keyboard languages / input methods", "Alt+⇧ Shift, Ctrl+⇧ Shift, ⊞ Win+Space, ⊞ Win+⇧ Shift+Space"],
  ["Print", "Ctrl+P"],
  ["Open Help Menu", ""],
  ["Windows Mobility Center", "Windows 7: ⊞ Win+X; Windows 10: ⊞ Win+X then B"],
  ["PowerUser (WinX) Menu", "Windows 10: ⊞ Win+X"],
  ["Restart Video Driver", "Windows 10: Ctrl+⇧ Shift+⊞ Win+B"]
];

const headers = ["Action", "Windows 10 Shortcut"];

const container = dv.el("table", null, { cls: "dataview" });
const thead = container.createEl("thead");
const tbody = container.createEl("tbody");

// Create header row
const headerRow = thead.createEl("tr");
headers.forEach(header => {
  const th = headerRow.createEl("th");
  th.textContent = header;
});

// Populate rows
rows.forEach(row => {
  const tr = tbody.createEl("tr");
  row.forEach(cell => {
    const td = tr.createEl("td");
    td.textContent = cell;
  });
  tbody.appendChild(tr);
});

container.appendChild(thead);
container.appendChild(tbody);
dv.container.appendChild(container);

```

---

#### System navigation
```dataviewjs
const rows = [
  ["Lock desktop", "⊞ Win+L"],
  ["Log out user", "N/A"], // No standard shortcut provided in the list
  ["Switch active user", "⊞ Win+L [notes 3]"],
  ["Applications menu", "⊞ Win or Ctrl+Esc"],
  ["Run application", "⊞ Win+R, enter executable name"],
  ["Search", "⊞ Win, enter executable name or ⊞ Win+S or F3"],
  ["Show desktop", "⊞ Win+D"],
  ["Access SysTray", "⊞ Win+B"],
  ["Switch window (next/previous)", "Alt+Tab / Shift+Alt+Tab"],
  ["Switch window without dialog", "Alt+Esc / Shift+Alt+Esc"],
  ["Task manager", "Ctrl+Shift+Esc or Ctrl+Alt+Delete"],
  ["File manager", "⊞ Win+E"],
  ["New folder", "Ctrl+Shift+N"],
  ["Rename object", "F2"],
  ["Show hidden files", "Alt+V, then H, then H again"],
  ["Cycle through installed keyboard languages / input methods", "Alt+⇧ Shift, Ctrl+⇧ Shift, ⊞ Win+Space, ⊞ Win+⇧ Shift+Space"],
  ["Print", "Ctrl+P"],
  ["Open Help Menu", "N/A"],
  ["Windows Mobility Center", "Windows 10: ⊞ Win+X then B"],
  ["PowerUser (WinX) Menu", "Windows 10: ⊞ Win+X"],
  ["Restart Video Driver", "Windows 10: Ctrl+Shift+⊞ Win+B"]
];

const headers = ["Action", "Windows 10 Shortcut"];

const container = dv.el("table", null, { cls: "dataview" });
const thead = container.createEl("thead");
const tbody = container.createEl("tbody");

// Create header row
const headerRow = thead.createEl("tr");
headers.forEach(header => {
  const th = headerRow.createEl("th");
  th.textContent = header;
});

// Populate rows
rows.forEach(row => {
  const tr = tbody.createEl("tr");
  row.forEach(cell => {
    const td = tr.createEl("td");
    td.textContent = cell;
  });
  tbody.appendChild(tr);
});

container.appendChild(thead);
container.appendChild(tbody);
dv.container.appendChild(container);

```

---

#### Power Management
```dataviewjs
const rows = [
  ["Place computer into sleep/standby mode", "⊞ Win+X > U > S"],
  ["Shut down computer", "⊞ Win+X > U > U"],
  ["Restart computer", "⊞ Win+X > U > R"],
  ["Force shutdown", "Power (Hold for several seconds)"]
];

const headers = ["Action", "Windows 10 Shortcut"];

const container = dv.el("table", null, { cls: "dataview" });
const thead = container.createEl("thead");
const tbody = container.createEl("tbody");

// Create header row
const headerRow = thead.createEl("tr");
headers.forEach(header => {
  const th = headerRow.createEl("th");
  th.textContent = header;
});

// Populate rows
rows.forEach(row => {
  const tr = tbody.createEl("tr");
  row.forEach(cell => {
    const td = tr.createEl("td");
    td.textContent = cell;
  });
  tbody.appendChild(tr);
});

container.appendChild(thead);
container.appendChild(tbody);
dv.container.appendChild(container);

```

---
#### Screenshots

```dataviewjs
const rows = [
  ["Save screenshot of entire screen as file", "⊞ Win+Print Screen"],
  ["Copy screenshot of entire screen to clipboard", "⊞ Win+Print Screen or Print Screen"],
  ["Copy screenshot of active window to clipboard", "Alt+Print Screen"],
  ["Copy screenshot of arbitrary area to clipboard (Snip)", "⊞ Win+⇧ Shift+S"]
];

const headers = ["Action", "Windows 10 Shortcut"];

const container = dv.el("table", null, { cls: "dataview" });
const thead = container.createEl("thead");
const tbody = container.createEl("tbody");

// Create header row
const headerRow = thead.createEl("tr");
headers.forEach(header => {
  const th = headerRow.createEl("th");
  th.textContent = header;
});

// Populate rows
rows.forEach(row => {
  const tr = tbody.createEl("tr");
  row.forEach(cell => {
    const td = tr.createEl("td");
    td.textContent = cell;
  });
  tbody.appendChild(tr);
});

container.appendChild(thead);
container.appendChild(tbody);
dv.container.appendChild(container);

```

---

#### Text Editing

```dataviewjs
const rows = [
  ["Delete char to the right of cursor", "Del or Fn+← Backspace"],
  ["Delete word to the right of cursor", "Ctrl+Del"],
  ["Delete word to the left of cursor", "Ctrl+← Backspace"],
  ["Go to start of line", "Home or Fn+←"],
  ["Go to end of line", "End or Fn+→"],
  ["Go to start of document", "Ctrl+Home"],
  ["Go to end of document", "Ctrl+End"],
  ["Go to previous word", "Ctrl+← or Ctrl+/"],
  ["Go to next word", "Ctrl+→"],
  ["Go to previous line", "↑"],
  ["Go to next line", "↓"],
  ["Go to previous line break (paragraph)", "Ctrl+↑"],
  ["Go to next line break", "Ctrl+↓"],
  ["Move cursor down viewport length", "Page Down"],
  ["Move cursor up viewport length", "Page Up"],
  ["Find", "Ctrl+F"],
  ["Go to next search result", "F3"],
  ["Go to previous search result", "⇧ Shift+F3"],
  ["Search and replace", "Ctrl+H"],
  ["Emoji Picker", "⊞ Win+. or ⊞ Win+;"]
];

const headers = ["Action", "Windows 10 Shortcut"];

const container = dv.el("table", null, { cls: "dataview" });
const thead = container.createEl("thead");
const tbody = container.createEl("tbody");

// Create header row
const headerRow = thead.createEl("tr");
headers.forEach(header => {
  const th = headerRow.createEl("th");
  th.textContent = header;
});

// Populate rows
rows.forEach(row => {
  const tr = tbody.createEl("tr");
  row.forEach(cell => {
    const td = tr.createEl("td");
    td.textContent = cell;
  });
  tbody.appendChild(tr);
});

container.appendChild(thead);
container.appendChild(tbody);
dv.container.appendChild(container);

```

---
#### Text formatting
```dataviewjs
const data = [
  { action: "Bold", windows: "Ctrl+B" },
  { action: "Underline", windows: "Ctrl+U" },
  { action: "Italic", windows: "Ctrl+I" },
  { action: "Uppercase / Lowercase", windows: "Ctrl+⇧ Shift+A" },
  { action: "Superscript", windows: "Ctrl+⇧ Shift+=" },
  { action: "Subscript", windows: "Ctrl+=" },
  { action: "Selected text larger/smaller", windows: "Ctrl+>, Ctrl+<" },
  { action: "Selected text Bullets or Numbered Items", windows: "Ctrl+⇧ Shift+L" },
  { action: "Insert Linebreak/Newline", windows: "Ctrl+↵ Enter" },
  { action: "Insert Unicode", windows: "Alt+X + character codepoint" }
];

let table = dv.table(["Action", "Windows 10"], 
  data.map(row => [row.action, row.windows])
);

```

---

#### Browser, Go Menu

```dataviewjs
const shortcuts = [
  {
    action: "Go to Address Bar",
    windows: "Ctrl+L / F6 / Alt+D, Alt+C or Alt+E (depending on language)"
  },
  {
    action: "Go to the previous location in history",
    windows: "Alt+← or ← Backspace"
  },
  {
    action: "Go to the next location in history",
    windows: "Alt+→ or ⇧ Shift+← Backspace (web browser only)"
  },
  {
    action: "Go up one level in the navigation hierarchy",
    windows: "Alt+↑ (Vista, 7, 8, or 10 only) or ← Backspace (Windows Explorer)"
  },
  {
    action: "Go to the starting page defined by the user or application",
    windows: "Alt+Home"
  }
];

dv.table(
  ["Action", "Windows"],
  shortcuts.map(s => [s.action, s.windows])
);

```

---
#### Web Browser

```dataviewjs
const shortcuts = [
  {
    action: "Bookmarks menu",
    windows: "Ctrl+B"
  },
  {
    action: "URL Shortcuts (Adds www. + .com)",
    windows: "Ctrl+↵ Enter"
  },
  {
    action: "URL Shortcuts (Adds www. + .org)",
    windows: "⇧ Shift+↵ Enter"
  },
  {
    action: "URL Shortcuts (Adds www. + .net)",
    windows: "⇧ Shift+↵ Enter"
  },
  {
    action: "Add bookmark for current page",
    windows: "Ctrl+D"
  },
  {
    action: "Add bookmark for current link",
    windows: "Meta+a"
  },
  {
    action: "Manage bookmarks",
    windows: "Ctrl+⇧ Shift+O (Microsoft Edge) or Ctrl+B (Internet Explorer)"
  },
  {
    action: "Move focus to Web search bar",
    windows: "Ctrl+E"
  },
  {
    action: "Move focus to address bar",
    windows: "Ctrl+L or F6 or Alt+D"
  },
  {
    action: "Refresh a webpage",
    windows: "Fn+F5 or Ctrl+R"
  },
  {
    action: "Refresh a webpage ignoring cache",
    windows: "Ctrl+F5 or Ctrl+⇧ Shift+R"
  },
  {
    action: "Open a new window",
    windows: "Ctrl+N"
  },
  {
    action: "Zoom Options (zoom in / zoom out / zoom 100%)",
    windows: "Ctrl++ / Ctrl+- / Ctrl+0"
  }
];

dv.table(
  ["Action", "Windows"],
  shortcuts.map(s => [s.action, s.windows])
);

```

---
#### Tab Management
```dataviewjs
const tabManagementShortcuts = [
  {
    action: "New tab",
    windows: "Ctrl+T"
  },
  {
    action: "Close tab",
    windows: "Ctrl+W"
  },
  {
    action: "Close all tabs but the current one",
    windows: "⌘ Cmd+⌥ Opt+T (Safari)"
  },
  {
    action: "Go to next tab",
    windows: "Ctrl+Tab ↹"
  },
  {
    action: "Go to previous tab",
    windows: "Ctrl+⇧ Shift+Tab ↹"
  },
  {
    action: "Go to tab-n",
    windows: "Ctrl+n[notes 9] (Chrome, Firefox, Internet Explorer)"
  },
  {
    action: "Go to last tab",
    windows: "Ctrl+9"
  },
  {
    action: "Move a tab to the left",
    windows: "Ctrl+⇧ Shift+Page Up (Chrome, Firefox)"
  },
  {
    action: "Move a tab to the right",
    windows: "Ctrl+⇧ Shift+Page Down (Chrome, Firefox)"
  },
  {
    action: "Open a previously closed tab",
    windows: "Ctrl+⇧ Shift+T"
  },
  {
    action: "Open a previously closed window",
    windows: "Ctrl+⇧ Shift+N (Firefox)"
  },
  {
    action: "Close the current internet tab",
    windows: "Ctrl+W"
  }
];

dv.table(
  ["Action", "Windows"],
  tabManagementShortcuts.map(s => [s.action, s.windows])
);

```

---
#### Windows

```dataviewjs
const windowManagementShortcuts = [
  {
    action: "Force window mode (Application requires functionality for set action)",
    windows: "0+↵ Enter"
  },
  {
    action: "Pop up window menu",
    windows: "Alt+Space"
  },
  {
    action: "Close the focused window",
    windows: "Alt+F4 or Alt+Space then C"
  },
  {
    action: "Close all windows of current application",
    windows: "Ctrl+⇧ Shift+W"
  },
  {
    action: "Restore the focused window to its previous size",
    windows: "Alt+Space then R"
  },
  {
    action: "Move the focused window",
    windows: "Alt+Space then M then Arrow Keys"
  },
  {
    action: "Resize the focused window",
    windows: "Alt+Space then S then Arrow Keys"
  },
  {
    action: "Keep window always on top",
    windows: "Ctrl+Alt+Esc (toggles on/off)"
  },
  {
    action: "Hide the focused window",
    windows: "⌘ Cmd+H"
  },
  {
    action: "Hide all except the focused window",
    windows: "⌘ Cmd+⌥ Option+H"
  },
  {
    action: "Put the focused window furthest back",
    windows: "Alt+Esc"
  },
  {
    action: "Minimize the focused window",
    windows: "Alt+Space then N or ⊞ Win+↓"
  },
  {
    action: "Maximize the focused window",
    windows: "Alt+Space then X or ⊞ Win+↑"
  },
  {
    action: "Maximize horizontally",
    windows: "Available, but no default"
  },
  {
    action: "Maximize vertically",
    windows: "⊞ Win+⇧ Shift+↑"
  },
  {
    action: "Minimize all",
    windows: "⊞ Win+M or ⊞ Win+D"
  },
  {
    action: "Minimize all non focused windows",
    windows: "⊞ Win+Home"
  },
  {
    action: "Undo minimize all",
    windows: "⊞ Win+⇧ Shift+M"
  },
  {
    action: "Switch fullscreen/normal size",
    windows: "F11 or ⊞ Win+⇧ Shift+↵ Enter"
  },
  {
    action: "Show the window in full screen mode",
    windows: "Depends on application"
  },
  {
    action: "Rollup/down window",
    windows: "Win+D"
  },
  {
    action: "Show all open windows",
    windows: "⊞ Win+Tab ↹"
  },
  {
    action: "Show all windows of current application",
    windows: "⊞ Win+Tab ↹"
  },
  {
    action: "Show all workspaces",
    windows: "⊞ Win+Tab ↹ (Windows 10)"
  },
  {
    action: "Move window to left/right/up/down workspace",
    windows: "⊞ Win+←/→"
  },
  {
    action: "Move window between multiple monitors",
    windows: "⊞ Win+⇧ Shift+←/→"
  },
  {
    action: "Move window to workspace n",
    windows: "Available, but no default"
  },
  {
    action: "Switch to next/previous workspace list",
    windows: "Available, but no default"
  },
  {
    action: "Go to workspace n",
    windows: "Ctrl+n"
  },
  {
    action: "Go to left/right/up/down workspace",
    windows: "Ctrl+← / Ctrl+→ / Ctrl+↑ / Ctrl+↓"
  },
  {
    action: "Quit application of current window",
    windows: "Alt+F4 or Ctrl+F4"
  },
  {
    action: "Close dialog",
    windows: "Esc or ⊞ Win+↓+F4"
  },
  {
    action: "Open/Focus pinned program on the taskbar",
    windows: "⊞ Win+(#)"
  },
  {
    action: "Open new program window of pinned program in Quick Launch",
    windows: "⊞ Win+(#)"
  },
  {
    action: "Open new program window of the pinned program on the taskbar",
    windows: "⊞ Win+⇧ Shift+(#)"
  },
  {
    action: "Focus the first taskbar entry",
    windows: "⊞ Win+T, then ←→"
  },
  {
    action: "Peek at the desktop",
    windows: "⊞ Win+Space or ⊞ Win+Comma"
  },
  {
    action: "Bring gadgets to the front of the Z-order",
    windows: "⊞ Win+G"
  },
  {
    action: "External display options",
    windows: "⊞ Win+P"
  }
];

dv.table(
  ["Action", "Windows"],
  windowManagementShortcuts.map(s => [s.action, s.windows])
);

```

---

#### User interface navigator

```dataviewjs
const uiNavigationShortcuts = [
  {
    action: "Moves keyboard focus to next/previous control",
    windows: "Tab ↹ / ⇧ Shift+Tab ↹"
  },
  {
    action: "Pop up tooltip for currently focused control",
    windows: "⇧ Shift+F1"
  },
  {
    action: "Show context-sensitive help for currently focused window or control",
    windows: "⇧ Shift+F1"
  },
  {
    action: "Give focus to next/previous pane",
    windows: "Ctrl+F6 / Alt+F5"
  },
  {
    action: "Give focus to splitter bar in paned window",
    windows: "F8"
  },
  {
    action: "Give focus to window's menu bar",
    windows: "F10 or Alt"
  },
  {
    action: "Pop up contextual menu for currently selected objects (aka context menu)",
    windows: "⇧ Shift+F10 or ≣ Menu"
  },
  {
    action: "Toggle selected state of focused checkbox, radio button, or toggle button",
    windows: "Space"
  },
  {
    action: "Activate focused button, menu item etc.",
    windows: "↵ Enter"
  },
  {
    action: "Expand a drop-down list",
    windows: "F4 or Alt+↓"
  },
  {
    action: "Select/move to first/last item in selected widget",
    windows: "Home / End"
  },
  {
    action: "Scroll selected view by one page up/left/down/right",
    windows: "PageUp / PageDown"
  },
  {
    action: "Scroll selected view to top/bottom",
    windows: "Home / End"
  },
  {
    action: "Switch focus to the next/previous tab/view within a window",
    windows: "Ctrl+Tab ↹"
  },
  {
    action: "Switch focus to the next/previous panel on the desktop",
    windows: "Ctrl+Alt+Tab ↹ / Ctrl+Alt+⇧ Shift+Tab ↹"
  },
  {
    action: "Switch focus to the next/previous panel (without dialog)",
    windows: "Ctrl+Alt+Esc / Ctrl+Alt+⇧ Shift+Esc"
  }
];

dv.table(
  ["Action", "Windows"],
  uiNavigationShortcuts.map(s => [s.action, s.windows])
);

```