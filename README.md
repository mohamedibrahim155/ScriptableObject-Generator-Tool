# 🧩 Unity ScriptableObject Generator

A  Unity Editor tool to **quickly create ScriptableObject scripts and assets** with custom fields, types, and collections — all from a clean UI.

---

## 🚀 Features

* 🔹 Generate ScriptableObject **scripts + assets** in one click
* 🔹 Support for:

  * Primitive types (int, float, string, bool)
  * Unity types (GameObject, Sprite, AudioClip, etc.)
  * Custom classes
  * Enums
* 🔹 Collection support:

  * List<T>
  * Arrays
* 🔹 Smart **type picker popup** (search + keyboard navigation)
* 🔹 Field validation with real-time preview
* 🔹 Auto-create missing folders (with confirmation popup)
* 🔹 Automatic asset creation after script compilation
* 🔹 Clean, scalable architecture (UI → Service → Validator → Generator)

---

## 📸 Preview

> <img width="450" height="700" alt="image" src="https://github.com/user-attachments/assets/4a5c34f2-8bc5-46a5-8126-eedf48e165a5" />

Field Types
> <img width="300" height="400" alt="image" src="https://github.com/user-attachments/assets/dfba6b71-78db-444b-9e23-97890900a5d0" />



---

## 🛠 Installation


### Option 1 — Git Clone

```bash
git clone https://github.com/mohamedibrahim155/ScriptableObject-Generator-Tool.git
```

Then place the folder inside:

```text
Packages/
```

---


## 📂 Folder Structure

```text
SOGenerator/
├── Editor/
│   ├── Windows/
│   │   └── ScriptableObjectCreator.cs
│   │   └── TypeSearchPopUpEditor.cs
│   ├── Services/
│   │   └── PendingScriptableObjectAssetCreatorService.cs
│   │   ├── SOCodeGeneratorService.cs
│   │   ├── SOGeneratorService.cs
│   │   └── SOValidator.cs
│   │   └── TypeSearchService.cs
│   ├── Models/
│   │   └── FieldDefinition.cs
│   │   └── SORequestData.cs
│   ├── Settings/
│   │   └── SOGeneratorSettings.cs
```

---

## 🧑‍💻 How to Use

1. Open the Unity project:

```text
Tools → Scriptable Object Generator
```

<img width="858" height="130" alt="image" src="https://github.com/user-attachments/assets/75536d81-e169-40d7-a4af-d09a2fea9324" />


2. Fill in:

* Class Name
* Namespace (optional)
* Script Folder
* Asset Folder

3. Add fields:

* Choose type
* Set name
* Pick custom class / enum if needed
* Add collections if required

4. Click:

```text
Create ScriptableObject
```

5. The tool will:

* Generate `.cs` file
* Compile scripts
* Automatically create `.asset` file

---

## 🧠 Architecture

This tool follows a clean separation of concerns:

```text
EditorWindow → UI only
SOGeneratorService → orchestration
SOValidator → validation rules
SOCodeGenerator → script generation
PendingAssetCreator → post-compilation asset creation
```

---

## ⚠️ Requirements

* Unity 2021+ (recommended)
* Editor-only tool (not included in builds)

---

## 🔮 Future Improvements

* Batch generation (CSV / JSON)
* Template system (WeaponData, EnemyData, etc.)
* Inline ScriptableObject editing
* Drag & drop support
* Addressables integration

---

## 🤝 Contributing

Contributions are welcome!

Feel free to:

* Open issues
* Suggest features
* Submit pull requests

---

## 📜 License

MIT License *(or whatever you choose)*

---

## 💡 Author

Mohamed Ibrahim
Game Programmer | Unity & Unreal Developer

GitHub: https://github.com/mohamedibrahim155
Portfolio: https://ibrahimportfolio.framer.website

---
