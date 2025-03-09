def cek_digit_belakang(a, b, c):
    """
    Fungsi ini memeriksa apakah minimal dua dari tiga parameter memiliki digit paling kanan yang sama.
    """
    digit_a = a % 10
    digit_b = b % 10
    digit_c = c % 10

    if digit_a == digit_b or digit_a == digit_c or digit_b == digit_c:
        return True
    else:
        return False

# Membaca input dari pengguna
a = int(input("Masukkan bilangan pertama: "))
b = int(input("Masukkan bilangan kedua: "))
c = int(input("Masukkan bilangan ketiga: "))

# Memanggil fungsi dan mencetak hasilnya
hasil = cek_digit_belakang(a, b, c)
print("Output:", hasil)

# Test-case yang diberikan
print("Test-case:")
print("Input = 30, 20, 18. Output =", cek_digit_belakang(30, 20, 18))
print("Input = 145, 5, 100. Output =", cek_digit_belakang(145, 5, 100))
print("Input = 71, 187, 18. Output =", cek_digit_belakang(71, 187, 18))
print("Input = 1024, 14, 94. Output =", cek_digit_belakang(1024, 14, 94))
print("Input = 53, 8900, 658. Output =", cek_digit_belakang(53, 8900, 658))
