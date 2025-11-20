# Creature Battle Project (OOP + Git Branching Practice)

This project is designed to help me learn **object-oriented programming (OOP)** in Python — especially **inheritance** — while also practicing key **Git concepts** like branching, merging, conflict resolution, and version history.

I will begin with a base class (`Creature`) and create additional subclasses on separate Git branches to simulate a real development workflow.

---

## Learning Objectives

### Python / OOP
- Understand and implement **classes**
- Use **inheritance** to extend behaviors
- Override and extend methods (e.g., `attack()`)
- Practice writing simple test code in `main`

### Git / Version Control
- Create and switch branches
- Merge branches into `main`
- Resolve merge conflicts
- View commit history (`git log --graph --all`)

---

## Project Structure
oop_creature_code/
│
├── creature_simulation.py # Base class + subclasses (Creature, SwimmingCreature, FlyingCreature, FireCreature)
└── README.md

---

## How to Test and Run

1. Open the file `creature_simulation.py`.
2. Run the program using Python 3:
python creature_simulation.py
3. Observe the console output to see the behavior of each creature, including attacks and special abilities.

---

## Git Workflow Summary

### 1. Create a new branch for a subclass
git checkout -b fire_creature

### 2. Implement and test the subclass  
Modify `creature_simulation.py` and add your new class.

### 3. Commit your changes
git add creature_simulation.py
git commit -m "Add FireCreature subclass with fire_level and attack override"

### 4. Merge the branch into main
git checkout main
git merge fire_creature

### 5. Add and commit the README, then push to GitHub
git add README.md
git commit -m "Add project README.md"
git push origin main

