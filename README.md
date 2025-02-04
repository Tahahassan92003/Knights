# Knights
Knights and Knaves Puzzle

Here's a project description for your logic-based reasoning system:  

---

### **Knights and Knaves Logic Solver**  

#### **Overview**  
This project is a logic-based reasoning system that models and solves *Knights and Knaves* puzzles. In these puzzles, characters (Knights and Knaves) make statements about themselves or others. Knights always tell the truth, while Knaves always lie. The system determines the truthfulness of statements using propositional logic and evaluates whether a given knowledge base entails a query.  

#### **Key Features**  
- **Logical Representation:** Uses propositional logic to define statements and constraints.  
- **Symbolic Logic Processing:** Implements logical operations including *AND*, *OR*, *NOT*, *Implication (=>)*, and *Biconditional (<=>)*.  
- **Model Checking:** Utilizes a truth-table method to verify logical entailment.  
- **Puzzle Solutions:** Provides solutions to *Knights and Knaves* puzzles by modeling characters and their statements.  
- **Custom Sentence Representation:** Defines classes for logical expressions like `Symbol`, `Not`, `And`, `Or`, `Implication`, and `Biconditional`.  

#### **How It Works**  
1. **Define Symbols**: Each character (A, B, C, etc.) is represented by two symbols (e.g., `AKnight` and `AKnave`).  
2. **Build Logical Constraints**:  
   - A character can either be a Knight or a Knave, but not both.  
   - A Knight’s statement must be true, and a Knave’s statement must be false.  
3. **Formulate Statements**: Statements made by characters are encoded into logical formulas.  
4. **Check Logical Consistency**: The system checks if the knowledge base logically entails the given query using model checking.  

#### **Example Puzzle (Puzzle 0)**  
- A says: *"I am both a knight and a knave."*  
- Logical Representation:  
  - A cannot be both a Knight and a Knave: `Not(And(AKnight, AKnave))`  
  - A must be either a Knight or a Knave: `Or(AKnight, AKnave)`  
  - If A is a Knight, then their statement must be true: `Implication(AKnight, And(AKnight, AKnave))`  
  - If A is a Knave, their statement must be false: `Implication(AKnave, Not(And(AKnight, AKnave)))`  

#### **Applications**  
- Automated theorem proving  
- AI-based logic puzzles and reasoning systems  
- Educational tool for learning propositional logic  
- Artificial intelligence and knowledge representation  

This project demonstrates the power of propositional logic in solving logical deduction problems and serves as a foundational system for AI-based reasoning.
