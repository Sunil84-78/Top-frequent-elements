from collections import Counter

def k_most_frequent(nums, k):
    return [item[0] for item in Counter(nums).most_common(k)]

# Taking user input
nums = list(map(int, input("Enter integers separated by space: ").split()))
k = int(input("Enter the value of k: "))
print(k_most_frequent(nums, k))
