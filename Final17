array = input("введите числа через пробел: ")
array_valid = []
for elem in array.split():
    if elem.isdigit():
        array_valid.append(int(elem))

def sort_func(num_list):
    """Сортировка списка пузырьком"""
    for i in range(len(num_list)):
        for j in range(len(num_list) - i - 1):
            if num_list[j] > num_list[j + 1]:
                num_list[j], num_list[j + 1] = num_list[j + 1], num_list[j]
    return num_list


a = sort_func(array_valid)
print(a)  # отсортированный список
b = int(input("введите число для поиска:"))


def poisk(a, b):
    for i in range(0, len(a) - 1):
        if a[i] < b and b <= a[i + 1]:
            return i


if poisk(a, b) == None:
    print(f"число {b}  за пределами списка")

print(poisk(a, b))
