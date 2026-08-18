
def find_peaks(numbers):
    peaks = []

    for index in range(1, len(numbers) - 1):
        if numbers[index] > numbers[index - 1] and numbers[index] > numbers[index + 1]:
            peaks.append(numbers[index])

    return peaks


if __name__ == "__main__":
    values = [2, 7, 4, 9, 3, 8, 5]

    print(f"Numbers: {values}")
    print(f"Peak values: {find_peaks(values)}")
