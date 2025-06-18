# ✅ Clean Code Principles: Concise and Practical

---

## 🧱 SOLID (OOP Design)

| Principle                | Core Idea                                  | Explanation                                              |
|--------------------------|--------------------------------------------|----------------------------------------------------------|
| S — Single Responsibility | One reason to change                      | A class/function should do only one thing               |
| O — Open/Closed           | Open for extension, closed for modification | Extend behavior without modifying existing code         |
| L — Liskov Substitution   | Subtypes must replace base types          | Subclasses shouldn't break the logic of base class      |
| I — Interface Segregation| Prefer small, focused interfaces           | Don't force a class to implement what it doesn't use    |
| D — Dependency Inversion  | Depend on abstractions, not concretions   | Classes should rely on interfaces, not concrete classes |

---

## ⚙️ GRASP (Architectural Roles)

| Principle             | Core Idea                              | Example                                         |
|----------------------|-----------------------------------------|-------------------------------------------------|
| Controller           | Coordinates interaction between objects | Angular controller / service                    |
| Creator              | Who creates objects                     | The one who owns or uses most of it creates it  |
| Information Expert   | Logic belongs where data is             | Object knows its own behavior                   |
| Low Coupling         | Minimal dependencies                    | Classes should not be tightly coupled           |
| High Cohesion        | Focused responsibility                  | Object does one job and does it well            |
| Polymorphism         | Behavior selection via subclasses       | Use interfaces or abstract classes              |
| Indirection          | Through a mediator                      | e.g., DI / Service to decouple dependencies     |
| Pure Fabrication     | Artificial object for separation of logic | A service that is neither model nor controller |
| Protected Variations | Shield from change                      | Abstract away unstable parts of the system      |

---

## 🔨 KISS, DRY, YAGNI, SoC, SRP (Universal Principles)

| Principle                         | Core Idea                        | Meaning                                             |
|----------------------------------|----------------------------------|-----------------------------------------------------|
| KISS — Keep It Simple, Stupid    | The simpler — the better         | Avoid overengineering                               |
| DRY — Don't Repeat Yourself      | Avoid code duplication           | Extract reusable logic into functions/components    |
| YAGNI — You Aren’t Gonna Need It | Don’t write unused features      | Avoid premature optimization                        |
| SoC — Separation of Concerns     | Separate responsibilities        | UI ≠ logic ≠ API, etc.                              |
| SRP — Single Responsibility       | One clear responsibility         | One module = one concern                            |

---

## 🚫 Code Smells (What Instantly Reveals Bad Code)

| Smell                | Symptom                                | Explanation                                         |
|----------------------|-----------------------------------------|-----------------------------------------------------|
| Long Function / Class| 100+ lines? Time to split               | One file = one responsibility                       |
| Duplicated Code      | Copy-paste everywhere                   | Extract into shared utilities                       |
| God Object           | One object does everything              | Split into smaller ones                             |
| Switch Hell          | Too many if/else/switch statements      | Use polymorphism or strategy pattern                |
| Shotgun Surgery      | One change affects multiple places      | Violates SRP/SoC                                    |
| Feature Envy         | One class accesses internals of another | Breaks encapsulation                                |
| Primitive Obsession  | Raw strings/numbers over real types     | Create a Value Object                               |
| Comments Overload    | Comments explain unclear code           | Make code self-explanatory                          |

---

## 📌 How to Use This?

- 🔁 When writing code — review this list.
- 🧠 During code reviews — ask yourself: *“Did I break any of these?”*
- 💡 Before adding new code — think: *“Will this harm the architecture?”*
