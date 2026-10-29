# TeachIT Addons Repository

Official game addons and educational catalog for **TeachIT Educational Game Launcher**.

This repository hosts pre-packaged, offline-ready educational games compliant with the TeachIT Game Package Contract (`@teachit/shared`).

## 🎮 Available Games

| Game | Category | Difficulty | Version | Package Size |
| :--- | :--- | :--- | :--- | :--- |
| **Binary Switch Circuit** | Logic | Beginner | `v1.0.0` | `packages/binary-switch-v1.0.0.zip` |
| **Falling Letters** | General | Beginner | `v1.0.0` | `packages/falling-letters-v1.0.0.zip` |
| **Mouse Master** | General | Beginner | `v1.0.0` | `packages/mouse-master-v1.0.0.zip` |
| **Sorting Algorithm Arena** | Algorithms | Intermediate | `v1.0.0` | `packages/sort-arena-v1.0.0.zip` |

---

## 🚀 How to Use with TeachIT

1. Open **TeachIT** and authenticate as Teacher / Administrator.
2. Navigate to **Administration Dashboard** > **Galerie des Jeux**.
3. In the catalog source URL field, enter:
   ```text
   https://github.com/MouadALLAOUI/teachit-addons
   ```
   *(TeachIT automatically resolves this to the raw GitHub catalog).*
4. Click **Charger le catalogue** (or **Actualiser**).
5. All 4 games appear with their preview thumbnails, learning objectives, and single-click **Installer** buttons.

---

## 🔒 Security & Integrity

All packages include SHA-256 cryptographic digests declared in `catalog.json`. TeachIT automatically validates the checksum before extracting any package into the student environment. Prohibited executables, scripts, and path traversal vectors are strictly blocked.

---

## 📂 Repository Structure

```text
teachit-addons/
├── catalog.json              # Main catalog index parsed by TeachIT
├── packages/                 # Standalone game ZIP archives
│   ├── binary-switch-v1.0.0.zip
│   ├── falling-letters-v1.0.0.zip
│   ├── mouse-master-v1.0.0.zip
│   └── sort-arena-v1.0.0.zip
├── thumbnails/               # High-contrast game preview icons
│   ├── binary-switch.svg
│   ├── falling-letters.svg
│   ├── mouse-master.svg
│   └── sort-arena.svg
└── README.md                 # Documentation
```
