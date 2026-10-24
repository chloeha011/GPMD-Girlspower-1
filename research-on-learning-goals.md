
"""
Learning Algorithms, Data Structures, and Connectionist AI
A beginner-friendly project.

Install the neural network dependency:
python -m pip install scikit-learn
"""

from collections import deque

# ==================================================
# 1. ALGORITHMS: BUBBLE SORT
# ==================================================

def bubble_sort(numbers):
    """Sort numbers from smallest to largest."""
    result = numbers.copy()

    for i in range(len(result)):
        for j in range(len(result) - 1 - i):
            if result[j] > result[j + 1]:
                result[j], result[j + 1] = (
                    result[j + 1],
                    result[j],
                )

    return result


def find_largest(numbers):
    """Find the largest number in a list."""
    if not numbers:
        return None

    largest = numbers[0]

    for number in numbers:
        if number > largest:
            largest = number

    return largest


# ==================================================
# 2. DATA STRUCTURES
# ==================================================

def data_structures_demo():
    print("\n--- DATA STRUCTURES ---")

    # Lists store multiple items.
    students = ["Alex", "Sam", "Jordan"]
    students.append("Taylor")
    print("Student list:", students)

    # Dictionaries store information using keys.
    ages = {
        "Alex": 18,
        "Sam": 20,
        "Jordan": 19,
    }
    print("Sam's age:", ages["Sam"])

    # Stacks follow Last In, First Out (LIFO).
    stack = []
    stack.append("Book 1")
    stack.append("Book 2")
    print("Stack removes:", stack.pop())

    # Queues follow First In, First Out (FIFO).
    queue = deque()
    queue.append("Person 1")
    queue.append("Person 2")
    print("Queue removes:", queue.popleft())

    # A simple tree represented by nested dictionaries.
    tree = {
        "name": "Root",
        "children": [
            {"name": "Child A", "children": []},
            {"name": "Child B", "children": []},
        ],
    }
    print("Tree root:", tree["name"])
    print(
        "Tree children:",
        [child["name"] for child in tree["children"]],
    )


# ==================================================
# 3. CONNECTIONIST AI: NEURAL NETWORK
# ==================================================

def neural_network_demo():
    print("\n--- NEURAL NETWORK ---")

    try:
        from sklearn.neural_network import MLPClassifier

        # Examples: two inputs, followed by the correct output.
        # This is the XNOR pattern.
        X = [
            [0, 0],
            [0, 1],
            [1, 0],
            [1, 1],
        ]

        y = [1, 0, 0, 1]

        # Create a small neural network.
        model = MLPClassifier(
            hidden_layer_sizes=(8,),
            activation="tanh",
            solver="lbfgs",
            max_iter=2000,
            random_state=42,
        )

        # Train the network using examples.
        model.fit(X, y)

        # Test the trained network.
        predictions = model.predict(X)

        for inputs, prediction in zip(X, predictions):
            print(
                f"Input: {inputs} -> "
                f"Predicted output: {prediction}"
            )

        print("\nThe network learned from example data.")
        print("Training is a process of adjusting model parameters.")

    except ImportError:
        print("Neural network library is not installed.")
        print("Install it using: python -m pip install scikit-learn")


# ==================================================
# 4. BEGINNER EXERCISES
# ==================================================

def exercises():
    print("\n--- BEGINNER EXERCISES ---")

    numbers = [4, 9, 2, 7, 1]

    print("Original numbers:", numbers)
    print("Sorted numbers:", bubble_sort(numbers))
    print("Largest number:", find_largest(numbers))

    # Exercise: Try changing the numbers.
    # Exercise: Add another student to the list.
    # Exercise: Change the inputs used by the neural network.


# ==================================================
# 5. LEARNING GOALS
# ==================================================

def learning_goals():
    print("\n--- PROJECT LEARNING GOALS ---")

    goals = [
        "Understand what an algorithm is.",
        "Learn lists, dictionaries, stacks, queues, and trees.",
        "Understand how a neural network learns from examples.",
        "See how algorithms and data structures support AI.",
        "Run and modify simple Python programs.",
        "Build confidence and practice teamwork using GitHub.",
    ]

    for number, goal in enumerate(goals, start=1):
        print(f"{number}. {goal}")


# ==================================================
# 6. MAIN PROGRAM
# ==================================================

def main():
    print("=" * 55)
    print("LEARNING ALGORITHMS, DATA STRUCTURES, AND AI")
    print("=" * 55)
    print("Welcome! This project is designed for beginners.")

    while True:
        print("\nChoose a topic:")
        print("1. Learn algorithms")
        print("2. Explore data structures")
        print("3. Try a neural network")
        print("4. Practice beginner exercises")
        print("5. View learning goals")
        print("0. Exit")

        choice = input("\nEnter your choice: ").strip()

        if choice == "1":
            numbers = [5, 2, 9, 1, 3]
            print("\nOriginal numbers:", numbers)
            print("Sorted numbers:", bubble_sort(numbers))
            print("Largest number:", find_largest(numbers))

        elif choice == "2":
            data_structures_demo()

        elif choice == "3":
            neural_network_demo()

        elif choice == "4":
            exercises()

        elif choice == "5":
            learning_goals()

        elif choice == "0":
            print("\nThank you for learning with us!")
            print("Keep practicing and exploring computer science.")
            break

        else:
            print("Invalid choice. Please enter a number from 0 to 5.")


if __name__ == "__main__":
    main()
