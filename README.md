# interactive_quiz
# Declare a list of questions and their corresponding answers
questions = [
    {
        "question": "What is the capital of France?",
        "answer": "Paris"
    },
    {
        "question": "What is the currency of Japan?",
        "answer": "Yen"
    },
    {
        "question": "What is the highest mountain in the world?",
        "answer": "Mount Everest"
    }
]

# Set the score to 0
score = 0

# Iterate over the questions
for q in questions:
    # Ask the question
    user_answer = input(q["question"] + " ")
    # Check if the answer is correct
    if user_answer.lower() == q["answer"].lower():
        # If the answer is correct, increment the score by 1
        score += 1
        print("Correct!")
    else:
        # If the answer is incorrect, print a message
        print("Incorrect. The correct answer is:", q["answer"])

# Print the final score
print("You scored", score, "points out of", len(questions))
