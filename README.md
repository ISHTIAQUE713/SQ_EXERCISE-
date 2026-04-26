def compute_leibniz_series(n=100000):
    total_sum = 0
    for i in range(1, n + 1):
        # Calculate the numerator: (-1)^(i+1)
        numerator = (-1)**(i + 1)
        # Calculate the denominator: 2i - 1
        denominator = 2 * i - 1
        total_sum += numerator / denominator
        
    return 4 * total_sum

# Calculate the result
result = compute_leibniz_series()
print(f"The result is: {result}")
