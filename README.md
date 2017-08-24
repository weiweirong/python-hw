# python-hw
def encipher(char):
    cipherchar=chr(ord(char)+5)
    if ord(cipherchar)>ord('z'):
        newcipher=chr(ord('a')+(ord(cipherchar)-123))
        return newcipher
    elif ord(cipherchar) in range (96,123):
        return cipherchar
    else:
        return char

def enciphertext(text):
    for letter in text:
      return encipher(letter)


    text = input("輸入你想加密的文字:  ")
    print(enciphertext(text))
