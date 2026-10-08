# Win: A Practical Guide to Windows

An introductory resource for learning to use, maintain, and troubleshoot Windows. It is intended for learners using a personal Windows 10 or Windows 11 PC; exact menus and features can vary by edition and release.

## Learning path

Work through the sections in order, or use the topics as a reference. You do not need administrator access for most activities.

1. **Get oriented:** identify your Windows version, find Settings, and learn how to get help.
2. **Manage files:** navigate folders, organize documents, and understand file extensions.
3. **Use applications and settings:** install trusted apps, manage updates, and configure everyday options.
4. **Learn the command line:** practice safe PowerShell commands for navigating and inspecting your own files.
5. **Maintain and troubleshoot:** check updates, storage, and system health before making changes.
6. **Build good security habits:** protect your account, recognize scams, and keep backups.

## 1. Get oriented

Windows is an operating system: it manages the computer's hardware and provides the desktop, settings, and services that applications use.

- Open **Settings** with **Windows key + I**. Use its search box when you do not know where an option is.
- Find your edition and version under **Settings → System → About**. To check for updates, open **Settings → Windows Update**.
- Use **Start** to find apps and search for settings or files. Use **Taskbar** for pinned and open apps.
- Press **Windows key + L** to lock your PC when stepping away.
- If you need help, search [Microsoft Support](https://support.microsoft.com/windows) using the exact wording of the issue and your Windows version.

**Try it:** Open About, note the Windows edition and version, then return to Settings without changing anything.

## 2. Files and folders

Files contain information; folders group files. File extensions (such as `.txt`, `.pdf`, or `.jpg`) indicate the file type and often which app opens it. The same file may appear in different locations, so check its full path before moving or deleting it.

- Open **File Explorer** with **Windows key + E**.
- Common personal folders include **Documents**, **Downloads**, **Pictures**, and **Desktop**. Their locations may vary if OneDrive or an organization manages the PC.
- Use the address bar to see where you are. Search within a folder when you cannot find a file.
- Copy a file to duplicate it; move it to relocate it. The Recycle Bin may let you restore recently deleted local files, but it is not a backup.
- Avoid deleting unfamiliar files from `C:\Windows`, `C:\Program Files`, or other system and application folders.

**Try it:** In Documents, make a folder named `Windows practice`, create a text file in it with Notepad, and then find it using File Explorer search.

## 3. Apps and everyday settings

- Prefer Microsoft Store or the software publisher's official website when installing applications. Check the publisher and requested permissions before proceeding.
- Uninstall apps you recognize and no longer need through **Settings → Apps → Installed apps**. Do not remove unfamiliar system components.
- Windows Update provides operating-system updates. Save your work before restarting, and do not interrupt an update that is in progress.
- Use **Settings → System → Display** to review display scaling and resolution, and **Settings → System → Sound** to choose audio devices.
- If an app stops responding, try closing and reopening it. Save work first when possible; ending a task can discard unsaved changes.

## 4. PowerShell basics

PowerShell is a command-line shell and scripting language included with Windows. Open **Windows Terminal** or search Start for **PowerShell**. Start with commands that only inspect information:

```powershell
Get-Location
Get-ChildItem
Get-Help Get-ChildItem
```

`Get-Location` shows the current folder; `Get-ChildItem` lists its contents; `Get-Help` provides command help. To explore your practice folder, use:

```powershell
Set-Location "$HOME\Documents\Windows practice"
Get-ChildItem
```

Commands can change or delete data. Read a command before running it, especially when copied from the internet. Avoid running unknown scripts, commands that request administrator access, or commands that download and immediately execute code.

**Try it:** Run the commands above in your practice folder and compare the listing with File Explorer. You can close the terminal without changing anything.

## 5. Basic troubleshooting

When something goes wrong, start with the least disruptive checks:

1. Write down the exact error message and what you were doing when it appeared.
2. Check whether the issue affects one app or the whole PC. Close and reopen the affected app.
3. Check network, power, available storage, and **Windows Update** status.
4. Restart the PC after saving your work, if it is safe to do so.
5. Search the exact error on Microsoft Support or the software publisher's support site. Be wary of unsolicited support calls and pop-ups.

Do not disable security protections, edit the registry, reset the PC, or delete system files as an early troubleshooting step. Back up important files and understand the consequences before attempting recovery or reset options. For a work or school device, contact its IT support before changing managed settings.

## 6. Security and backups

- Keep Windows and applications updated, and leave Windows Security protections enabled.
- Use a strong, unique password and multi-factor authentication where available. Lock the screen when you leave.
- Treat unexpected links, attachments, QR codes, and requests for passwords or payment as suspicious. Verify through a known, independent contact method.
- Download software only from sources you trust. Do not grant administrator permission unless you understand why the app needs it.
- Keep another copy of important files, such as on an external drive or a trusted cloud service. A synced folder is useful, but deletion or account problems can sync too; keep a separate backup when files matter.
- Never share recovery keys, passwords, one-time codes, or personal files with someone who contacts you unexpectedly.

## Further learning

- [Windows help and learning](https://support.microsoft.com/windows) — user guides and troubleshooting from Microsoft.
- [Windows Update: FAQ](https://support.microsoft.com/windows/windows-update-faq-8a903416-6f45-0718-f5c7-375e92dddeb2) — update information and common questions.
- [Windows Security](https://support.microsoft.com/windows/stay-protected-with-windows-security-2ae0363d-0ada-c064-8b56-6a39afb6a963) — built-in security features.
- [PowerShell documentation](https://learn.microsoft.com/powershell/) — official command and scripting references.

## Contributing

Found a broken link or an unclear instruction? Open an issue with the section name, what should change, and (when relevant) your Windows version. Do not include passwords, recovery keys, or other private information.
