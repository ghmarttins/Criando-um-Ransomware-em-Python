# Criando-um-Ransomware-em-Python

📌 Objetivo

Este projeto tem como finalidade estudar conceitos de criptografia e sua aplicação prática em Python.
Ele demonstra como arquivos podem ser protegidos com uma chave e, posteriormente, recuperados, de forma didática e controlada.

----
⚠️ Aviso Importante:
Este projeto não deve ser usado com intenção maliciosa.
O código é apenas para fins educacionais e simulação em ambientes controlados.

---
📂 Estrutura do Projeto

encrypter.py → Script responsável por criptografar arquivos, removendo a versão original e criando um novo arquivo com extensão .ransomwaretroll.
decrypter.py → Script responsável por descriptografar arquivos previamente criptografados, restaurando o arquivo original.

Exemplo de fluxo:

```bash
arquivo.txt → [encrypter.py] → arquivo.txt.ransomwaretroll  
arquivo.txt.ransomwaretroll → [decrypter.py] → arquivo.txt
```
---
⚙️ Requisitos

Python 3.x

Biblioteca 
```bash
pyaes
```
---
Para instalar o pyaes, utilize:
```bash
pip install pyaes
```
🚀 Como Executar
1. Preparar um arquivo de teste

Crie um arquivo simples, por exemplo:
```bash
echo "Conteúdo de teste" > teste.txt
```
2. Criptografar o arquivo

Execute o script de criptografia:
```bash
python encrypter.py
```
Isso irá:

- ler o arquivo ```bash teste.txt```
- remover o arquivo original
- criar o arquivo criptografado ```bash teste.txt.ransomwaretroll```
---
3. Descriptografar o arquivo

  Execute o script de descriptografia:
```bash python decrypter.py```

  Isso irá:

- ler o arquivo ```bash teste.txt.ransomwaretroll```
- restaurar o arquivo original ```bash teste.txt```
- remover o arquivo criptografado
---

  📚 Conceitos Envolvidos

- criptografia simétrica: a mesma chave é usada para criptografar e descriptografar.
- AES (Advanced Encryption Standard) no modo CTR (Counter).
- manipulação de arquivos binários em Python.
- segurança ofensiva e defensiva em ambientes controlados.
