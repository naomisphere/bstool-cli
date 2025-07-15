# Commands
### Set prop values from ```bluestacks.conf```
```
$ bstool conf bst.feature.ai_chat 1
[*] Changed bst.feature.ai_chat to 1
```

### Verify kernel/initrd integrity
```
$ bstool verify initrd /Users/satomi/bstk/boot
  _         _              _ 
 | |__  ___| |_ ___   ___ | |
 | '_ \/ __| __/ _ \ / _ \| |
 | |_) \__ \ || (_) | (_) | |
 |_.__/|___/\__\___/ \___/|_|
                             
[^] initrd directory appears valid

$ bstool verify kernel
  _         _              _ 
 | |__  ___| |_ ___   ___ | |
 | '_ \/ __| __/ _ \ / _ \| |
 | |_) \__ \ || (_) | (_) | |
 |_.__/|___/\__\___/ \___/|_|
                             
[*] Verifying /Applications/BlueStacks.app/Contents/img/kernel_hvf
[^] Kernel appears valid
```

### Extract initrd from initrd_hvf.img
```
$ bstool unpack initrd
  _         _              _ 
 | |__  ___| |_ ___   ___ | |
 | '_ \/ __| __/ _ \ / _ \| |
 | |_) \__ \ || (_) | (_) | |
 |_.__/|___/\__\___/ \___/|_|
                             
[*] Extracting initrd img to /Users/satomi/bstk/boot
[^] Done
```

### Replace kernel/initrd with given file
```
$ bstool write initrd /Users/satomi/bstk/boot
  _         _              _ 
 | |__  ___| |_ ___   ___ | |
 | '_ \/ __| __/ _ \ / _ \| |
 | |_) \__ \ || (_) | (_) | |
 |_.__/|___/\__\___/ \___/|_|
                             
[*] Compressing /Users/satomi/bstk/boot
[*] Writing files
[*] Setting permissions
[^] Done
```

### Backup management
```
$ bstool backup
  _         _              _ 
 | |__  ___| |_ ___   ___ | |
 | '_ \/ __| __/ _ \ / _ \| |
 | |_) \__ \ || (_) | (_) | |
 |_.__/|___/\__\___/ \___/|_|
                             
[*] Writing backup
[^] Backup completed successfully
[*] Saved to /Users/satomi/.bstk/backups

$ bstool backup apply
  _         _              _ 
 | |__  ___| |_ ___   ___ | |
 | '_ \/ __| __/ _ \ / _ \| |
 | |_) \__ \ || (_) | (_) | |
 |_.__/|___/\__\___/ \___/|_|
                             
[*] Applying backup...
[*] Restoring /Applications/BlueStacks.app
[*] Setting permissions
[*] Restoring /Users/Shared/Library/Application Support/BlueStacks
[*] Setting permissions
[^] Backup applied successfully

$ bstool backup delete
  _         _              _ 
 | |__  ___| |_ ___   ___ | |
 | '_ \/ __| __/ _ \ / _ \| |
 | |_) \__ \ || (_) | (_) | |
 |_.__/|___/\__\___/ \___/|_|
                             
[*] Deleting backup...
[^] Backup deleted successfully
```
