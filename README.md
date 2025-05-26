# UnInspector for Omni Networking
A modern, extensible Inspector and serialization toolkit for Unity — **unofficial fork of Tri-Inspector, maintained and evolved for the Omni Networking ecosystem**.

---

## 🚀 Overview
**UnInspector** is an advanced fork of [Tri-Inspector](https://github.com/codewriter-packages/Tri-Inspector), specifically updated for use with the [Omni Networking](https://github.com/RuanCardoso/Omni-Networking-for-Unity) framework.

Supercharge your Unity Inspector and serialization with new attributes, native support for observable/serializable dictionaries, and various bug fixes for high-performance multiplayer projects.

---

## ✨ Key Features
- **Official Omni Networking Integration**  
  Optimized workflow for multiplayer and networked projects with Omni.

- **Bug Fixes & Stability Improvements**  
  Enhanced compatibility for Unity 2021+ and modern .NET versions.

- **New Inspector Attributes**  
  Exclusive attributes for network data and observable collections.

- **Serializable ObservableDictionary**  
  Full support for observable dictionaries with serialization and runtime change events.

---

## 📚 Usage Examples
#### Serializable Observable Dictionary
```csharp
using Omni.Inspector;
using Omni.Collections;
using UnityEngine;

public class PlayerStats : MonoBehaviour
{
    public ObservableDictionary<string, int> Stats = new();
}
```

---

## 📝 Important Note
**UnInspector works independently** - you can download and use it in any Unity project without requiring Omni Networking. While it's optimized for Omni Networking projects, all features work perfectly in standalone Unity projects.

---

## 🎯 Auto Anchors Tool

UnInspector includes a powerful Auto Anchors editor tool that automatically sets UI anchors based on current positions and sizes, making responsive UI design effortless.

### Features
- **Smart Anchor Calculation** - Automatically calculates anchor points based on current position relative to parent
- **Scale Handling** - Properly handles scaled objects by converting scale to size
- **Layout Group Detection** - Safely ignores objects controlled by Layout Groups
- **Undo Support** - Full undo/redo support for all operations

### Keyboard Shortcuts
- **F1** - Auto anchor selected GameObjects
- **F2** - Auto anchor all RectTransforms in scene  
- **F3** - Match selected objects to parent size and auto anchor

### Usage
1. Select UI elements in the hierarchy
2. Press **F1** to automatically set anchors based on current position
3. Use **F3** to stretch elements to fill parent and set anchors
4. Press **F2** to process all UI elements in the scene at once

Perfect for converting absolute-positioned UI elements to responsive anchored layouts!

## 🔧 Core Attributes

**Display & Validation**
- `[ShowInInspector]` - Show non-serialized properties
- `[Required]` - Mark required fields  
- `[ReadOnly]` - Make fields non-editable
- `[ValidateInput]` - Custom validation
- `[InfoBox]` - Display info messages

**Styling**
- `[Title]`, `[HideLabel]`, `[LabelText]`
- `[GUIColor]`, `[Indent]`, `[PropertySpace]`
- `[InlineEditor]`, `[InlineProperty]`

**Conditionals**
- `[ShowIf]`, `[HideIf]`, `[EnableIf]`, `[DisableIf]`
- `[ShowInPlayMode]`, `[HideInEditMode]`

**Collections**
- `[ListDrawerSettings]` - Customize list display
- `[TableList]` - Display collections as tables
- `[Dropdown]` - Dropdown selection

**Groups**
- `[Group]` - Group properties together
- `[DeclareBoxGroup]`, `[DeclareFoldoutGroup]`
- `[DeclareTabGroup]`, `[DeclareHorizontalGroup]`

**Buttons**
- `[Button]` - Add method buttons
- `[EnumToggleButtons]` - Toggle button enums

---

## 📄 License
UnInspector is MIT licensed.

**Credits:**  
https://github.com/codewriter-packages/Tri-Inspector
