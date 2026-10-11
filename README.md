# SpinWheel sharing and importing

## Install

Replace the contents of Models.swift and WheelLibraryView.swift in your existing Xcode project with the included files. Keep one copy of each definition. Press Command-R. No new app source file or project settings are needed. Checks is excluded from the app target.

## Share

Open your wheel library. Tap + → Share current wheel, or long-press a saved wheel and choose Share wheel. The iOS share sheet offers available destinations such as AirDrop, Messages, Mail and Save to Files. SpinWheel produces a portable SpinWheel.json file. It sends nothing until you choose a destination and complete the share flow.

## Import

Save a received SpinWheel.json file to Files. In SpinWheel open the library, tap + → Import wheel, and choose the file. Review its name, entries, colours and weights, then tap Save imported wheel. The imported wheel is a new selected copy with fresh IDs. Existing wheels/history remain saved. Cancel preview leaves the library unchanged; Undo can remove the newly imported copy.

Tapping a received file does not directly open SpinWheel in this version. Import it through the app's Files picker. This is file sharing, not web-link sharing or cloud collaboration; recipients need SpinWheel with this update. Generic third-party spinner files and raw wheels.json archives are not accepted.

## Included data

Entries, colours, weights, spin duration, sound/haptic preferences and the no-repeat setting are included. Current round picks are omitted; an imported wheel starts fresh. Winner history, challenge progress and global challenge-mode preferences are not shared. Valid files are versioned and limited to 1 MB and 1,000 entries. Invalid or incompatible files show an error before any wheel is saved.

The files are based on your current Desktop project and preserve no-repeat rounds, Undo, templates and the rest of the app. Desktop files are not modified by this download. Visual/device testing of the native share sheet and Files picker remains.

Validation: Xcode 27 iOS Simulator Debug build passed. Checks passed for setting/colour/weight round-trips, fresh IDs and rounds, malformed files, file-size limits, unsupported versions, invalid settings and empty wheels.
