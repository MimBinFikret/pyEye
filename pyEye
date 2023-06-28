import os

def combine_python_files(directory):
    # Hedef dosyanın adı ve yolu
    output_file = "combined_files.txt"
    output_path = os.path.join(directory, output_file)

    # Hedef dosyayı aç ve içini temizle
    with open(output_path, "w") as combined_file:
        # Klasördeki tüm dosyaları gez
        for filename in os.listdir(directory):
            if filename.endswith(".py"):  # Sadece .py dosyalarını işle
                file_path = os.path.join(directory, filename)
                # .py dosyasını aç ve içeriğini oku
                with open(file_path, "r") as python_file:
                    file_contents = python_file.read()
                    # İçeriği hedef dosyaya yaz
                    combined_file.write(file_contents)
                    combined_file.write("\n\n")  # Dosyalar arasına boşluk bırak

    print("Tüm .py dosyaları başarıyla birleştirildi.")


# Mevcut klasördeki .py dosyalarını birleştir
current_directory = os.getcwd()
combine_python_files(current_directory)
