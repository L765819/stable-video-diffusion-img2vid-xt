word_to_code = {
    'Дубе': '001',
    'ясене': '002',
    'дубе': '003',
    'зелене': '004',
    # Додайте інші слова і їх коди тут
}

# Перетворення рядка слів у код
words = "Дубе, дубе, ясене дубе, Дубе, дубе, зелене дубе."
words_list = words.split()
encoded_message = " ".join([word_to_code[word.strip(',.')] for word in words_list])
print(encoded_message)