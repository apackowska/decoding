# decoding



def main():

    print("This program decodes a series of Unicode numbers ")
    print(" and converts a string of text that it represents. \n")

    inString = input("Give the Unicode-encoded message>")
    chars = []
    for numStr in inString.split():
        codeNum = int(numStr) # convert digits to a number
        chars.append(chr(codeNum)) # accumulate new character

    message = "".join(chars)
    print("The decoded message is>>", message, chars)



main()
