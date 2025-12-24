# 🎵 Singer Recommendation Expert System

A Rule-Based Expert System developed using Python that acts as a digital music consultant. The system analyzes user preferences (genre, tempo, era, etc.) to recommend the most suitable singer from a knowledge base of over 90 Egyptian and American artists.

## 💡 Project Idea
The main idea behind this project is to simulate the reasoning of a human music critic. Instead of randomly searching for songs, the user provides specific criteria defining their current mood or taste. The system then uses **Artificial Intelligence (Logic-Based Approach)** to match these inputs against a set of predefined rules to infer the perfect singer match.

## 🚀 Key Features
- **Interactive GUI:** User-friendly interface built with Tkinter for easy data entry.
- **Visual Results:** Displays not just the name, but also a photo of the recommended singer.
- **Smart Inference:** Uses a Forward Chaining inference engine to navigate through ~96 logic rules.
- **Dual Input Mode:** Supports GUI inputs with a fallback to Console inputs if data is missing.
- **Customizable UI:** Supports background images for a better user experience.

## 🛠️ Technologies & Libraries Used
The project is built entirely in **Python** using the following libraries:

| Library | Purpose |
| :--- | :--- |
| **Experta** | The core Knowledge Engine (Rule-Based System library for Python). |
| **Tkinter** | Used for building the Graphical User Interface (GUI). |
| **Pillow (PIL)** | Used for image processing (handling background and singer photos). |
| **Collections** | patched for Python 3.10+ compatibility. |

## ⚙️ How It Works (Working Method)
The system follows the **Forward Chaining** methodology of Expert Systems:

1.  **Fact Gathering:** The system starts by collecting "Facts" from the user via the GUI (e.g., *Century: 21st*, *Tempo: Fast*, *Nationality: Egyptian*).
2.  **Pattern Matching:** The Inference Engine monitors the "Knowledge Base". It checks if the current set of facts matches the conditions (LHS) of any defined Rule.
3.  **Rule Firing:** Once a rule's conditions are met (e.g., *IF Egyptian AND Modern AND Fast AND Romance*), the rule "fires".
4.  **Action/Conclusion:** The system declares a new fact (The Singer's Name) and triggers the result window to display the name and photo.

## 📂 Project Structure
```text
├── main.py              # The main source code
├── background.jpg       # The background image for the main menu
├── README.md            # Project documentation
├── requirements.txt     # List of dependencies
└── [Singer Name].jpg    # Images for each singer (e.g., Amr Diab.jpg, Adele.jpg)
