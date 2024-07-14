from cryptography.fernet import Fernet

# chave = Fernet.generate_key()

# with open('filekey.key','wb') as file:
#     file.write(chave)

with open('filekey.key','rb') as file:
    chave = file.read()
    
key = Fernet(chave)

# with open('SPSLab.py','rb') as arq:
#     code = arq.read()
    
# Crypt_Code = key.encrypt(code)
    
# with open('SPSLab_cpt.txt','wb')  as file_crypt:
#     file_crypt.write(Crypt_Code)
    
with open('SPSLab_cpt.txt','rb')  as file_crypt:
    code = file_crypt.read()

code_decrypt = key.decrypt(code)

with open('SPSLab_decrypt.txt', 'wb') as decrypt_content:
    decrypt_content.write(code_decrypt)
