n = int(input("Введите длину квадрата:"))
R = int(input("Введите радиус бублика:"))
for i in range(n):
    line = []
    for j in range(n):
        if (1.6*(i-n/2)**2 + (j-n/2)**2) <= R**2:
            if (1.6 * (i - n / 2) ** 2 + (j - n / 2) ** 2) <= R ** 2 // 4:
                line.append(". ")
            else:
                line.append("# ")
        else:
            line.append(". ")
    print(''.join(line))
input()
