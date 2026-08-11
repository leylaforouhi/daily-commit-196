def calculate_word_frequency(sentence):
    frequency = {}

    for word in sentence.lower().split():
        frequency[word] = frequency.get(word, 0) + 1

    return frequency


if __name__ == "__main__":
    text = "coding daily improves coding skills every day"

    print(f"Text: {text}")
    print(f"Frequency: {calculate_word_frequency(text)}")
