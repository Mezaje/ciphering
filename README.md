# ciphering
simple encrypt code of  python

lf = input('type yes for encrypt and no for descrypt :')

lf.lower()
cipher = ('abcdefjhijklmnopqrstuvwxyz')
plain = ('*&%02`~^?"]_)(#+-$TO%%;@><')
if lf == 'yes':
    pl = input('plain text: ')
    for n in pl:
        if n in cipher:
            s = cipher.index(n)
            print(plain[s], end='')

if lf == 'no':
    pl = input('enter the cipher text: ')
    pl.lower()
    for n in pl:
        if n in plain:
            s = plain.index(n)
            print(cipher[s], end='')
