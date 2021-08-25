# Voz-do-Google-python
Este código faz que você escreva algo e assim que escrever  o "python" irá ler sua mensagem.

"""PROJECT SPEAK"""
import androidhelper

droid = androidhelper.Android()
message = droid.dialogGetInput('ESCREVA AQUI', 'O que você quer que eu escreva?').result
droid.ttsSpeak(message)
