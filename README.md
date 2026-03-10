# Application-level-Insertion-Sort-program-5


# Insertion Sort Program - Sorting Company Names

companies = ["TCS", "Infosys", "Wipro", "HCL", "Accenture"]

# Insertion Sort
for i in range(1, len(companies)):
    key = companies[i]
    j = i - 1

    while j >= 0 and companies[j] > key:
        companies[j + 1] = companies[j]
        j -= 1

    companies[j + 1] = key

print("Sorted Company Names:")
for company in companies:
    print(company)



Sorted Company Names:
Accenture
HCL
Infosys
TCS
Wipro
