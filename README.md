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
